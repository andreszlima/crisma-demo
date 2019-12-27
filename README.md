# Crisma
### Aplicação gerenciamento de de presenças e registros de pagamento

### Demonstração
Caso queira testar o aplicativo online, vá para o link: [https://crismacr.herokuapp.com](https://crismacr.herokuapp.com) - O primeiro carregamento deve demorar um pouco, já que o aplicativo hiberna após 30 min de inatividade. Caso ele não abra depois de algum tempo carregando me envie um e-mail que colocarei em funcionamento novamente.<br>

### Parte externa do site
- Página inicial estática, para fazer inscrição de usuários
  - Aqui é utilizado Recaptcha, do Google, para impedir bots de fazerem inscrições.
- Pode ser feito um acompanhamento de presenças e pagamentos de cada crismando através de um botão colocado na página inicial. Essa exibição pode ser feita digitando o nome completo do crismando.
- Um outro botão, para catequistas, é utilizado para entrar na parte fechada do sistema.

### Parte interna do site
- Adicionar crismandos/catequistas
- Criar temas para serem explorados em formações. Esses temas terão campos de título, data, grupo (jovens ou adultos) e um campo para descrição, que pode ser escrito como em um caderno de anotações, pra ser consultado posteriormente
- Criar listas de presença para cada tema criado. As listas de presença terão todos os crismandos já registrados no sistema. Caso algum crismando entre depois da criação da lista, é possível atualizar a lista para incluir essa pessoa
- Mostrar em uma tabela a quantidade de faltas de todos os crismandos, separados por grupo (jovens ou adultos), contando todos os encontros de formação. Caso algum crismando tenha entrado após algum encontro de formação, será contada falta para ele naquele dia
- Criar registros de pagamentos, com informaçes de origem de pagamento, destino de pagamento, categoria (mostradas abaixo), forma de pagamento, valor e um campo para escrever alguma observação que seja pertinente
- É possível criar registros de valor a ser pago nas seguintes categorias:
  - Crismandos Jovens
    - Inscrição
    - Celebração
  - Crismandos Adultos
    - Inscrição 
    - Celebração
  - Catequistas
    - Camisa
    - Aprofundamento
- Com esses valores pré-determinados, é possível filtrar e ver quais crismandos/catequistas pagaram cada um desses valores
- É possível também ver, no perfil de cada crismando registrado no sistema, todas as presenças ou faltas em cada dia de formação de acordo com seu grupo de formação e todos os pagamentos que fez. Além disso é possível ver todas as informações cadastradas, como telefone, idade ou turma, por exemplo
- No caso de catequistas é possível ver todos os pagamentos feitos e recebidos
- São consolidados em uma página todos os valores em caixa com cada catequista

### Informações adicionais de segurança:
- As senhas dos usuários também são criptografadas. Nem administrador nem quem tem acesso ao banco de dados tem acesso às senhas, que são armazenadas através do que é chamado de "hash". Um exemplo é a senha '123456', que está armazenada no banco de dados como "$2a$11$NRgCPQZWSI5gU64FB/aJ2uHYWIcetg6oLTxYYX.02B8S6CPDE59la". Isso é muito importante para a segurança das informações.

#### Dados técnicos

Linguagens de programação: Ruby, HTML5, CSS3, SCSS, Javascript<br>
Framework: Ruby on Rails<br>
Banco de dados utilizado: PostgreSQL<br>

## Para mais informações: 

* Autor: André de Souza Lima
* E-mail: andre.szlima1@gmail.com
* Instagram: www.instagram.com/andreszlima
* Twitter: www.twitter.com/andreszlima
