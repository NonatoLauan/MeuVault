Loops em PHP são ==estruturas essenciais para repetir blocos de código com base em condições, automatizando tarefas como percorrer arrays ou manipular dados==. Os quatro tipos principais são **for** (número específico de vezes), **foreach** (elementos de um array), **while** (enquanto a condição for verdadeira) e **do...while** (pelo menos uma vez).

---

### Tipos de Loop em PHP

**`for`**: Ideal quando se sabe  quantas vezes o bloco deve ser executado.
exemplo:
```php
for ($i = 0; $i < 5; $i++) {
	echo "contagem: $i <br>";
}
```

**`foreach`**: Especializado para percorrer arrays e objetos, sendo o mais comum para listas de dados.
exemplo:
```
$cores = array("azul", "verde", "vermelho");
foreach ($cores as $cor) {
    echo "$cor <br>";
}
```
**`while`**: Executa o código repetidamente enquanto a condição for verdadeira.
exemplo: 
``` php
$i = 0;
while ($i < 5) {
    echo "Número: $i <br>";
    $i++;
}
```
**`do...while`**: Garante que o código seja executado pelo menos uma vez, antes de verificar a condição.
exemplo: 
``` php
$i = 0;
do {
    echo "Número: $i <br>";
    $i++;
} while ($i < 5);
```