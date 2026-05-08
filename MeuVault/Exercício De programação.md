#  Problemas de Lógica em PHP

Treine resolvendo problemas usando:
- [[Variáveis]]
- [[Tipos de dado]]
- [[Operadores]]
- [[If e Else]]
- [[Switch]]
- [[Loops]]

---

# 🟢 Nível 1 — Fundamentos

## 1. Par ou Ímpar
Peça um número e diga se ele é par ou ímpar.

💡 Usa:
- Operadores (%)
- If e Else

``` php
1.Peça um número e diga se ele é par ou ímpar.

echo "Olá, seja bem-vindo! \n";
$n = readline("Digite um número: ");
echo "você digitou o número $n \n";
echo "irei verificar se ele é par ou impar... \n";
if ($n %2 == 0) {
echo "O número $n é par \n";
} else {
echo "O número $n é impar \n";

}
```
---

## 2. Maior de idade
Dado uma idade, verifique se é maior ou menor de idade.

💡 Usa:
- Variáveis
- If e Else
- Operadores relacionais

``` php
2. Maior de idade
Dado uma idade, verifique se é maior ou menor de idade.

echo "Seja bem-vindo! \n";
sleep(2);

$nome = readline("Digite seu nome: \n");
echo "Vejamos ... \n";
sleep(2);

echo "$nome. \n" ;
sleep(2);

echo "É um belo nome. \n";
sleep(3);

echo "Ok, $nome, agora me diga sua idade: \n";
sleep(3);

$idade = readline("Digite sua idade: \n");
echo "hmmmm \n";
sleep(2);

echo "...\n";
sleep(2);

echo "$idade né? \n";
sleep(3);

if ($idade < 18) {
echo "Desculpe $nome, mas você não pode entra aqui. \n";
} else {
echo "Tudo bem, acho que você pode passar.\n";
}
```

---

## 3. Soma simples
Some dois números e mostre o resultado.

💡 Usa:
- Variáveis
- Operadores matemáticos
``` php
 3. Soma simples
 Some dois números e mostre o resultado.

echo "Olá, seja bem-vindo! \n";
sleep(2);

  

$n1 = readline("Digite o primeiro número:");
$n1 = (int) $n1;

$n2 = readline("Agora, digite o segundo número:");
$n2 = (int) $n2;

$n3 = $n1 + $n2;
$n3 = (int) $n3;

  

echo "Ok, calculando a soma de $n1 e $n2 \n";
sleep(2);

echo "O resultado da soma de $n1 e $n2 é $n3 \n";
```
---

## 4. Tipo de número
Verifique se um número é:
- positivo
- negativo
- zero

💡 Usa:
- If e Else
- Operadores

``` php
4. Tipo de número
Verifique se um número é:
- positivo
- negativo
- zero 

echo "Olá, seja bem-vindo! \n";
sleep(2);

  

$n = readline("Por favor, digite um número: ");
$n = (int) $n;
sleep(2);

  

if ($n > 0) {
echo "O número $n é positivo \n";
} elseif ($n < 0) {
echo "O número $n é negativo \n";
} else {
echo "O número $n é zero \n";
}
```
---

# 🟡 Nível 2 — Controle de fluxo

## 5. Classificação de nota
Dada uma nota:
- 0 a 4 → Reprovado
- 5 a 6 → Recuperação
- 7 a 10 → Aprovado

💡 Usa:
- If e Else
- Operadores de comparação

``` php
5. Classificação de nota
Dada uma nota:
- 0 a 4 → Reprovado
- 5 a 6 → Recuperação
- 7 a 10 → Aprovado 

echo "Bem-vindo \n";
sleep(2);

echo "Como devo te chamar? \n";
  
$nome = readline("");
sleep(2);

echo "$nome, perfeito \n";
sleep(1);

echo "Agora \n";
sleep(1);

$materia = readline("Por favor, me diga o nome da matéria \n");
sleep(1);

echo "Perfeito \n";

$nota1 = readline("Agora me diga a sua primeira nota:\n");
$nota1 = floatval($nota1);
sleep(1);

  

$nota2 = readline("Agora me diga a sua segunda nota:\n");
$nota2 = floatval($nota2);
sleep(1);

$media = ($nota1 + $nota2) / 2;
  
if ($media >= 0 && $media <= 4) {
echo "Na matéria de $materia, sua média foi de $media\n";
sleep(1);

echo "Portanto, você foi reprovado \n";

} elseif ($media >= 5 && $media <= 6) {
echo "Na matéria de $materia, sua média foi de $media \n";
sleep(1);

echo "Portanto, você está em recuperação \n";
} else {
echo "Na matéria de $materia, sua média foi de $media \n";
sleep(1);

echo "Portanto, você foi aprovado \n";
}
```

---

## 6. Dia da semana (Switch)
Dado um número de 1 a 7, mostre o dia da semana.

💡 Usa:
- Switch
- Variáveis

``` php
6. Dia da semana (Switch)
Dado um número de 1 a 7, mostre o dia da semana. 

echo "Bem-vindo \n";
sleep(2);

$n = readline("Digite um número de 1 a 7 para saber o dia da semana correspondente: \n");
$n = intval($n);
sleep(1);

switch ($n) {
case 1:
echo "O número $n corresponde a Domingo \n";
break;

case 2:
echo "O número $n corresponde a Segunda-feira \n";
break;
case 3:
echo "O número $n corresponde a Terça-feira \n";
break;

case 4:
echo "O número $n corresponde a Quarta-feira \n";
break;

case 5:
echo "O número $n corresponde a Quinta-feira \n";
break;

case 6:
echo "O número $n corresponde a Sexta-feira \n";
break;

case 7:
echo "O número $n corresponde a Sábado \n";
break;

default:
echo "Número inválido. Por favor, digite um número de 1 a 7. \n";

}
```
---

## 7. Calculadora simples
Faça uma operação com:
- +, -, *, /

💡 Usa:
- Switch
- Operadores
- Variáveis

``` php
7. Calculadora simples
Faça uma operação com:
- +, -, *, / */

echo "Calculadora Simples\n";
sleep(1);

$n1 = readline("Digite o primeiro número: \n");
sleep(1);

$n2 = readline("Digite o segundo número \n");
sleep(1);

echo "Perfeito \n";
sleep(1);

$operacao = readline("Digite a operação que deseja realizar (+, -, *, /): \n");
sleep(1);

switch ($operacao) {

case '+':
$resultado = $n1 + $n2;
echo "O resultado da soma é: " . $resultado . "\n";
break;

case '-':
$resultado = $n1 - $n2;
echo "O resultado da subtração é: " . $resultado . "\n";
break;

case '*':
$resultado = $n1 * $n2;
echo "O resultado da multiplicação é: " . $resultado . "\n";
break;

case '/':
if ($n2 != 0) {
$resultado = $n1 / $n2;

echo "O resultado da divisão é: " . $resultado . "\n";

} else {
echo "Erro: Divisão por zero não é permitida.\n";
}
break;

default:
echo "Operação inválida. Por favor, escolha entre +, -, *, /.\n";
}
```
---

# 🔵 Nível 3 — Loops

## 8. Contagem de 1 a 10
Exiba números de 1 a 10.

💡 Usa:
- Loop (for ou while)
``` php
 8. Contagem de 1 a 10
Exiba números de 1 a 10.

echo "Contagem de 1 a 10 \n";
sleep(1);

$i = 0;

while ( $i <= 10) {
echo "$i \n";
sleep(1);

$i++;
}
```
---

## 9. Soma de 1 a N
Peça um número N e some todos os valores até ele.

💡 Usa:
- Loop
- Variáveis
- Operadores

``` php
 9. Soma de 1 a N
Peça um número N e some todos os valores até ele. 

echo "Soma de 1 a N \n";
sleep(1);

$n = readline("Digite um número : \n");
sleep(1);

$soma = 0;

for ($i = 1; $i <= $n; $i++) {
$soma += $i;
echo $i;

	if ( $i < $n) {
	echo " + ";
	}
	flush();
	sleep(1);
}

echo " = $soma\n";
```
---

## 10. Tabuada
Mostre a tabuada de um número.

💡 Usa:
- Loop
- Operadores

10. Tabuada

``` php
Mostre a tabuada de um número. */

echo " Tabuada \n";
sleep(1);

$n = readline("Escreva um número para ver a sua tabuada \n");
$n = floatval($n);
sleep(1);

echo"A tabuada de $n é:\n";

for ( $i = 0; $i <= 10; $i++ ) {
$multi = $n * $i;

echo "$n x $i = $multi \n";
sleep(1);
}
echo "Fim \n";

```
---

## 11. Contar pares
Mostre quantos números pares existem de 1 a 50.

💡 Usa:
- Loop
- Operador %

```php

echo "Contador de pares\n";
sleep(1);
  
$n = readline("Digite um número: ");
sleep(1);

$i = 1;
$totalPar = 0;

echo "Números pares: ";

while ($i <= $n) {
	if ($i % 2 == 0) {
		echo $i . " ";
		$totalPar++;
		sleep(1);
	}
$i++;
}
echo "\nTotal de números pares entre 1 e $n: $totalPar\n";
?>
```
---

# 🔴 Nível 4 — Misturando tudo

## 12. Sistema de login simples
- Usuário e senha fixos
- Verificar se está correto

💡 Usa:
- If e Else
- Variáveis
- Operadores

---

## 13. Média de notas
- Receber 3 notas
- Calcular média
- Dizer se passou ou não

💡 Usa:
- Variáveis
- Operadores
- If e Else

---

## 14. Menu de opções (Switch + Loop)
- Mostrar menu:
  1. Somar
  2. Subtrair
  3. Sair
- Repetir até sair

💡 Usa:
- Switch
- Loop
- Variáveis

---



