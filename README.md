<p align="center">
  <img width="260" src="https://github.com/myTapp/front-end-test/blob/master/mytapp.png?raw=true">
</p>

- O teste consiste em criar uma aplicação:
  - em node.js
  - utilizando o banco de dados PostgreSQL
  - que expõe uma API REST de um CRUD simples de usuários
  
- E uma interface web:
  - para login
  - para consulta de dados de uma API externa
  
- O front-end deve ser simples e deve apresentar funcionalidades básicas como login, mensagens de usuário / senha incorretos, ...
- Depois de logado o usuário da aplicação deve poder consumir pela interface dados de uma das API's externas (da escolha do candidato) da listagem de [API's públicas](https://github.com/toddmotto/public-apis).
  - Uma das API's entrega [cervejas e não necessita autenticação](https://punkapi.com/)
  - Deve se apresentar os dados numa listagem simples com paginação e opcionalmente filtros
  - Os endpoints de consulta de dados devem todos ter autenticação por webtoken ou similar
  
- O CRUD não necessita interface, coloque os enpoints disponíveis no readme
  
- Pode ser utilizado qualquer ORM de preferência, aconselhamos o uso do [sequelize](https://github.com/sequelize/sequelize) ou [typeorm](https://github.com/typeorm/typeorm)
- Pode ser utilizado qualquer framework front-end de preferência, preprocessadores de css, task runners, bundlers, ... mas nenhum deles é obrigatório, quanto mais simples e direto ao ponto o código melhor (KISS) - se algum for utilizado, não se deve fazer o commit de pastas como node_modules, o projeto deve instalar suas dependências a partir do package.json
- Será julgado além do funcionamento a estrutura do código, o uso de boas práticas no js, html e css


- Deve ser entregue:
  - um repositório git (fork deste) contendo o projeto
  
- Opcional:
  - versão de build / produção do front-end


- Realizado a produçao do front-end e back-end
Dentro da pasta principal está a pasta do back-end.


# frontend

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
http://localhost:8080/
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint

Na pasta backend-server também README para execução do projeto.