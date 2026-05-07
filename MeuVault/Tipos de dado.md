O PHP suporta diversos tipos de dados, divididos principalmente entre escalares (simples), compostos e especiais. Os principais tipos são: **String** (texto), **Integer** (inteiro), **Float** (número decimal), **Boolean** (true/false), **Array** (lista), **Object** (objeto), **NULL** (vazio) e **Resource** (recurso externo)

1. Tipos Escalares (Simples)

- **String:** Cadeia de caracteres alfanuméricos, definida por aspas simples (`'`) ou duplas (`"`). ```$messagem = 'olá mundo';```
- **Integer (int):** Números inteiros, positivos ou negativos, sem ponto decimal (ex: `10`, `-5`). ``` $idade = 18;```
- **Float (ou Double):** Números reais com ponto decimal ou notação científica (ex: `10.5`, `3.14`). ```$pi = 3.14;```
- **Boolean (bool):** Representa valores de verdade, podendo ser `true` (verdadeiro) ou `false` (falso). ```$ativo = true;```

---

2. Tipos Compostos

- **Array:** Uma estrutura que armazena múltiplos valores em uma única variável, podendo ser um mapa ou vetor indexado. ```$numeros = [1, 2, 3, 4, 5];```
- **Object (Objeto):** Instância de uma classe, que armazena dados e informações sobre como processá-los. 
```php
class Pessoa {
    public $nome = "Lauan";
    public $idade = 18;
}

$pessoa = new Pessoa();
echo $pessoa->nome;
```
- **Callable:** Refere-se a funções que podem ser chamadas como callbacks.
```
function saudacao() {
    return "Olá!";
}

$func = "saudacao";
echo $func();
```
- **Iterable:** Um tipo que aceita qualquer array ou objeto que possa ser percorrido.
```
function listar(iterable $items) {
    foreach ($items as $item) {
        echo $item . "\n";
    }
}

$listas = ["A", "B", "C"];
listar($listas);
```