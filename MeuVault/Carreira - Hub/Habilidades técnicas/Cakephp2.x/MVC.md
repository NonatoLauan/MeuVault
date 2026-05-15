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
### Controller  -  Direcionamento
O **Controller** (Controlador) ==é o cérebro da arquitetura MVC==. Ele atua como o intermediário que recebe as solicitações do usuário, processa a lógica de negócios, interage com o **Model** (dados) e determina qual **View** (interface gráfica) deve ser exibida.