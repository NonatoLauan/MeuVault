Operadores são símbolos usados para realizar operações em valores e variáveis.  
  
---  
  
# 1.  Operadores Aritméticos  
  
Usados para cálculos matemáticos.  
  
```php  
$a = 10;  
$b = 5;  
  
echo $a + $b; // Soma → 15  
echo $a - $b; // Subtração → 5  
echo $a * $b; // Multiplicação → 50  
echo $a / $b; // Divisão → 2  
echo $a % $b; // Módulo (resto) → 0  
```  
  
💡 Usado em cálculos e lógica numérica.  
  
---  
  
# 2.  Operadores de Comparação  
  
Comparam valores e retornam true ou false.  
  
```php id="cmp1"  
$a = 10;  
$b = 5;  
  
var_dump($a == $b); // igual  
var_dump($a != $b); // diferente  
var_dump($a > $b); // maior  
var_dump($a < $b); // menor  
var_dump($a >= $b); // maior ou igual  
var_dump($a <= $b); // menor ou igual  
```  
  
💡 Usado em if/else e decisões.  
  
---  
  
# 3. Operadores Lógicos  
  
Usados para combinar condições.  
  
```php id="logic1"  
$idade = 18;  
$temCarteira = true;  
  
var_dump($idade >= 18 && $temCarteira); // AND → ambos verdadeiros  
var_dump($idade >= 18 || $temCarteira); // OR → um verdadeiro já basta  
var_dump(!$temCarteira); // NOT → inverte valor  
```  
  
💡 Essencial para regras de negócio.  
  
---  
  
# 4.  Operadores de Atribuição  
  
Usados para atribuir valores.  
  
```php id="assign1"  
$a = 10;  
  
$a += 5; // $a = $a + 5 → 15  
$a -= 2; // 13  
$a *= 2; // 26  
$a /= 2; // 13  
```  
  
💡 Usado para atualizar variáveis rapidamente.  
  
---  
  
# 5.  Operador de Incremento e Decremento  
  
```php id="inc1"  
$a = 10;  
  
echo $a++; // pós-incremento  
echo ++$a; // pré-incremento  
  
echo $a--; // pós-decremento  
echo --$a; // pré-decremento  
```  
  
💡 Usado em loops.  
  
---  
  
#  RESUMO  
  
- + - * / % → Matemáticos  
- == != > < → Comparação  
- && || ! → Lógicos  
- += -= *= → Atribuição  
- ++ -- → Incremento  
```