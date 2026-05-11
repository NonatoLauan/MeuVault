A estrutura `switch` no PHP compara uma única expressão com vários valores (`case`), executando o bloco de código correspondente ao primeiro valor coincidente. É uma alternativa organizada a múltiplos `if`s, utilizando `break` para evitar a execução de casos seguintes e `default` para tratar cenários não mapeados.

---

Sintaxe básica: 
``` php
switch ($expressao) {
    case $valor1:
        // Código se $expressao == $valor1
        break;
    case $valor2:
        // Código se $expressao == $valor2
        break;
    default:
        // Código se nenhum caso corresponder
}
```
exemplo: 
``` php
$cor = "vermelho";

switch ($cor) {
    case "azul":
        echo "A cor é azul.";
        break;
    case "vermelho":
        echo "A cor é vermelho.";
        break;
    default:
        echo "Cor desconhecida.";
}
// Saída: A cor é vermelho.
```
