# README

- Criar o DB
`rake db:create`

- Migrar o DB
`rake db:migrate`

- Definir Rotas no `/config/routes.rb`
```sh
- root to: 'home#index'

- get '/sobre', to: 'sobre#index'
```

- Criar os controllers (*Home* e *Sobre*) para as rotas (*root* e *sobre*)
```sh
- rails g controller Home

- rails g controller Sobre
```

- E para todo controller criado sempre configurar as ações dentro do controller `/app/controllers/home_controller.rb` e `/app/controllers/sobre_controller.rb` adicionando a rota correspondente a ação

- E nunca esquecer de também criar as views (*com o mesmo nome da ação*) dentro da pasta (*com o mesmo nome do controller*).. É nelas que irá ficar o conteúdo de cada rota