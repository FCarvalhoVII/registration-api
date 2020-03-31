## API para cadastro, autenticação de usuários e recuperação de senha

### Tecnologias usadas: NodeJS, Express e MongoDB.

#### Descrição
Trata-se de uma *API-REST* para cadastro, autenticação, recuperação de senha, cadastro de projetos e tarefas do usuário, com o banco de dados do Usuário relacionado, para pesquisa, com os demais bancos (Projetos e Tarefas), sendo utilizados para este fim MongoDB e Mongoose.
As senhas são encriptadas por meio do *bcryptjs* e guardadas no banco de dados do usuário, a autenticação é feita por meio de token gerado pelo *jasonwebtoken (jwt)*. A recuperação de senha é feita por email utilizando a ferramenta *nodemailer*, onde será enviado um email com uma chave de acesso gerada por meio do *crypto*, essa chave expira em uma hora.

#### Build
Para utilizar essa API você ira precisar do MongoDB rodando em sua máquina para as operações no bando de dados, para iniciar a aplicação basta executar o comando ```npm start``` no diretório raíz da aplicação.