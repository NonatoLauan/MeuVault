No PHP, as estruturas if, else e elseif são usadas para controlar o fluxo do código com base em condições lógicas.

---
1. Estrutura básica `if` e `else`
	O bloco `if` executa um código se a condição for verdadeira. O `else` (opcional) executa um código alternativo se a condição for falsa.
	
	```php
	$idade = 18;

	if ($idade >= 18) {
	    echo "Você é maior de idade.";
	} else {
	    echo "Você é menor de idade.";
	}
	```
2. Múltiplas condições com `elseif`
	Para testar mais de dois cenários, utiliza-se o `elseif` entre o `if` e o `else`. No PHP, você pode escrever `elseif` (junto) ou `else if` (separado), e ambos funcionam da mesma forma na sintaxe de chaves `{}`.
	```
	$hora = 14;

	if ($hora < 12) {
	    echo "Bom dia!";
	} elseif ($hora < 18) {
	    echo "Boa tarde!";
	} else {
    echo "Boa noite!";
	}
	```
3. Sintaxe Alternativa (ideal para HTML)
	O PHP oferece uma sintaxe que usa `:` e `endif;`, muito útil para manter o código limpo quando misturado com tags HTML.  
	**Atenção:** Nesta sintaxe, você **deve** usar a palavra `elseif` (junta); o uso de `else if` (separado) causará um erro de compilação.
