MVC é um padrão de arquitetura utilizado para organizar sistemas.

Ele separa o sistema em 3 responsabilidades diferentes, evitando bagunça no código.

MVC ( Model, View, Controller): Cada parte faz uma função.

### Model -- Dado e Regras:
O *model* representa:
-  banco de dados
-  regras de negócio 
-  validações
-  relacionamentos

Exemplo: 
-   tabela *users*
-   classe *Users*

O model é quem: 
-  Busca dados
-   Salva dados 
-   valida dados
Ele conversa com o banco

*OBS: Regra de negócio fica no Model.*


### View -- A Tela
A **View** é o que o usuário vê.

- HTML
- interface
- exibição de dados

Ela apenas mostra informações

Exemplo: index.ctp; add.ctp; edit.ctp.