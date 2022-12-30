# linktreeClone
Clone do Linktree com Laravel 8

# Sistema
Multi-tenancy

# Tecnologias
Laravel 7
  -auth
  -migrations

# Funções
Link de página personalizável (atriostech.com.br/algumacoisa)
Facebook pixel
Fundo de página (imagem, cor fixa, cor degradê)
Cor do Texto
Histórico de views
Histórico de clicks em cada link

# layout da Página
imagem da página
título da página
descrição (bio)
links
  texto
  link
  cor do texto
  cor do fundo
  tipo de borda (quadrada, arredondada)
feito com amor pela atriostech

# Regra de negócio
1 Usuários
  N Tokens --> Tokens serão gerados e vendidos na loja | os cartões irão conter o link: atriostech.com.br/token_criado 
  N Páginas
    1 Token
    N Links

O usuário efetua login e ativa o token comprado na loja;
depois associa esse token a uma página;
cada página pode ser associada a um token;

# Criando Projeto
  instale o chocolatey
  instale a versão 7.2.5 do php
    choco install php --version=7.2.5 --force
  criar o projeto com o laravel 7 
    composer create-project --prefer-dist laravel/laravel:^7.0 tagbio
  criar as tabelas do banco de dados tagbio com migrations
    php artisan migrate
  
