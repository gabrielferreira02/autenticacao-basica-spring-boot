# autenticacao-basica-spring-boot

Projeto de estudo aplicando spring-security com autenticação e autorização baseada em roles. 

Contém apenas três rotas a aplicação que seguem abaixo:
- "/free": acesso permitido para todos
- "/user": acesso permitido para quem tem a role USER
- "/admin": acesso permitido para quem tem a role ADMIN

Para executar a aplicação é necessário clonar o repositório
  ```bash
  git clone https://github.com/gabrielferreira02/autenticacao-basica-spring-boot.git
  ```

Acesse o diretório criado
  ```bash
  cd autenticacao-basica-spring-boot
  ```
Para iniciar o projeto possuem duas maneiras:
  - Inicializar pela propria IDE que irá utilizar ou inicializar com a imagem docker

Para inicializar com a imagem docker siga os seguintes passos
  ```bash
  docker build -t <nome-da-imagem>:<tag> .
  ```

Agora basta inicializar um container com a imagem criada
  ```bash
  docker run -p 8080:8080 <nome-da-imagem>:<tag>
  ```

Agora com a aplicação inicializada, no projeto tem uma pasta postman com um arquivo json
- Abra o postman
- Aperte em <strong>import</strong>
- Selecione o arquivo json

Com a collection importada já tem endpoints com dados de request para testar a aplicação
