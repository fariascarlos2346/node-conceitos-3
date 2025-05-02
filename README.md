<h1>Iniciando Projento Com NodeJS</h1>
<p>Entendedo conceitos de Servidores, criando um projeto BeckEnd utilizando Node e criando uma API.</p>
<p>Primeiro passo e Baixar o Node em nossa maquina, versão LTS para o sistema operacional da sua maquina. </p>
<p>Nesta projeto apredi os Conceitos de Front-End e Back-End além de Full-Stack</p>
<p>NPM  -> Ferramenta do JavaScript, gerenciador de pacotes do Node, Bibliotecas para nos ajudar nos Projetos.</p>
<p>Criando projeto com Express e fazendo sua estalação abrindo o terminal, no terminal com o comando 'npm init -y', criando nosso arquivo PACKAGE.JSON onde fica todas as informações do Projeto, a ficha dele, nome, versão, descrição, main, scripts como rodar o projeto e muitos mais.  Além da estalação do Express com o comando "npm i express", criando o  PACKAGE-LOCK.JSON  com muitas informações que nunca vamos mexer nele, e a outra pasta a NODE_MODULES onde o EXPRESS foi estalado e muitas outras coisas, pastas e suas Dependecias, sem estas pastas o sistema não roda.</p>
<h2>Subindo nosso servidor após as estalações</h2>
<p>Temos dois jeitos de subir o servidor
<br>
jeito antio => const express = requere("express")
<br>
jeito novo => import express from 'express'
<br>
para rodar no terminal => node server.js, Para rodar esta forma nova, no PACKAGE.JSON temos que colocar "type": "module".
</p>
<h2>Protocolos HTTP e seus Padrões de Rotas, suas formas de Comunicação</h2>
<p>Verbos HTTP => Get=listar, Post=criar, Put=editar vários, Patch=editar um e Delete=deletar</p>
<p>
  Query Params(GET) para consulta
  <br>
  Route Params (GET, PUT, DELETE) buscar, deletar ou editar algo específico
  <br>
  Body Params (POST E PUT) Para enviar ou buscar muitas informações { "nome": "Carlos", "id": "23" }
  <br>
  <h3>Codigos HTTP</h3>
  <p>Confirmação / Sucesso = 2xx</p>
  <p>Erro do Cliente (Front-End) = 4xx</p>
  <p>Erro no servidor (falha ao concluir solicitação) = 5xx</p>
</p>
<h2>Criando nossa Primeira rota Get</h2>
<p>
  app.get('/usuarios)', (req, res) => {res.send("Olá, Mundo!")}
  <br>
  Batento no localhost:3000 no nosso Navegador representando o Front-End.
  <br<>
  Temos uma extenção no VScode o Thunder Client para simular o Front-End onde vamos criar nossas Rotas e fazer os Testes.
</p>
<h2>Criando nosso Banco de Dados para Persistir nossos Dado Profissionalmente, pois não podemos guardar dados em uma Variável</h2>
<br>
<p>Usando o Banco de Dados MongoDB de forma Gratuita</p>
<p>Mais uma Biblioteca para conectar o banco de dados. O Prisma, estalando com 'npm install prisma --save-dev', sera estalado como devDependecies, so em desenvolvimento. Depois o comando npx prisma init para criar alguns Arquivos para nós, o .gitignore, .env e schema.prisma. O Prisma e o Intermediario do nosso Banco de Dados com uma Interface Grafica.
<br>
Mais este comando para estalar e avisar ao Banco quais dados serão Salvos. npm install @prisma/client, para Consolidar os Dados com o comando 'npx prisma db push'. Com o comando "npx prisma studio". nos conseguimos visualizar no navegador o Dados do Banco.
</p>


