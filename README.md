# Desafio do Felipão

O código abaixo define uma função chamada `calculadoraDePartidasRankeadas` que calcula o saldo de vitórias e determina o nível de um jogador com base no número de vitórias. A função recebe dois parâmetros: `vitorias` e `derrotas`.

#### Explicação do Código

1. **Cálculo do Saldo de Vitórias**:
   A variável `saldoVitorias` é calculada subtraindo o número de derrotas do número de vitórias.
   ```javascript
   const saldoVitorias = vitorias - derrotas;
   ```

2. **Determinação do Nível**:
   O nível do jogador é determinado com base no número de vitórias usando uma série de condicionais `if-else`.
   ```javascript
   if (vitorias < 10) {
       nivel = 'Ferro';
   } else if (vitorias <= 20) {
       nivel = 'Bronze';
   } else if (vitorias <= 50) {
       nivel = 'Prata';
   } else if (vitorias <= 80) {
       nivel = 'Ouro';
   } else if (vitorias <= 90) {
       nivel = 'Diamante';
   } else if (vitorias <= 100) {
       nivel = 'Lendário';
   } else {
       nivel = 'Imortal';
   }
   ```

3. **Exibição da Mensagem**:
   A função exibe uma mensagem no console com o saldo de vitórias e o nível do jogador.
   ```javascript
   console.log("O Herói tem de saldo de " + saldoVitorias + " está no nível de " + nivel);
   ```

4. **Exemplo de Uso**:
   A função é chamada com 100 vitórias e 10 derrotas como exemplo.
   ```javascript
   calculadoraDePartidasRankeadas(100, 10);
   ```

#### Tabela de Níveis

| Vitórias | Nível     |
|----------|-----------|
| < 10     | Ferro     |
| 11 - 20  | Bronze    |
| 21 - 50  | Prata     |
| 51 - 80  | Ouro      |
| 81 - 90  | Diamante  |
| 91 - 100 | Lendário  |
| > 100    | Imortal   |

#### Exemplo de Saída

```
O Herói tem de saldo de 90 está no nível de Lendário
```

🎮 **Divirta-se jogando e melhorando seu nível!** 🏆
