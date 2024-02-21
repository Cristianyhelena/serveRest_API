# Aprendizados do curso Dominando Postman
Testes de API Rest do manual ao CI/CD

## O que é?
Este repositorio foi criado fixar o aprendizado adiquirido com o curso Dominando Postman.

## Tecnologias utilizadas
- Postman versão web
- node versrion v18.14.2
- newman version 6.1.1
- newman-reporter-html

## Documentações

 - Doc da API [Consulte Swagger](https://serverest.dev/)

## Como instalar o ambiente

- Primeiro: instale o node em seu computador [Baixe aqui](https://nodejs.org/en/download)
- Segundo: realize a instalação do node de forma global [Baixe aqui a dependencia](https://www.npmjs.com/package/newman)
- 
  ...
  npm install -g newman
  ...
- Terceiro: realize a instalação da dependencia dos relatorios (opcional) [newman-reporter-html](https://www.npmjs.com/package/newman#html-rnpm i newmaneporter)

...
 npm install -g newman-reporter-html
 ...

## Como rodar os testes

### Pelo Postman web ou desktop
- Import a collection e o environment
- Execute os teste de forma manual ou automatizada
  
### Pelo newman
- Abra o console de preferência
- Execute a seguinte linha de comando para rodar os testes
```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli
```
- Execute os teste com relatório
```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli,htmlextra
```
### Report
Se você optou por rodar os teste com o report htmlextra, você gerou um arquivo html com o resultado dos testes e para verificar as validações

## Entre em contato
- cristiany.hp@gmail.com
