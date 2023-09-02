# Docker Todo List

A [Trybe](https://www.betrybe.com/) é uma escola de tecnologia com foco em formação de Desenvolvedores Web e o projeto Docker Todo List foi proposto como atividade de aprimoramento dos estudos sobre desenvolvimento back-end com foco criar aplicações dockerizadas. 

## Objetivo

O projeto Docker Todo List é uma aplicação Full Stack dockerizada que permite ao usuário criar sua própria lista de tarefas adicionando, editando e removendo items. O principal desafio desse projeto foi dockerizar a aplicação, criando as imagens e o docker-compose.

## Tecnologias e Ferramentas
<div>
   <img src='https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white' alt='HTML' />
    <img src='https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white' alt='CSS3' />
    <img src='https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black' alt='JavaScript' />
    <img src='https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB' alt='ReactJS' />
    <img src='https://img.shields.io/badge/eslint-3A33D1?style=for-the-badge&logo=eslint&logoColor=white' alt='ESlint' />
    <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="NodeJS"/>
    <img src="https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white" alt="Docker"/>
    <img src="https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express"/>
</div>

<br>

Na elaboração deste projeto utilizou-se as seguintes ferramentas:

### Front-end
- HTML
- CSS
- [ReactJS](https://pt-br.reactjs.org/)

### Back-end
- [NodeJS](https://nodejs.org/en/)
- [Express](https://expressjs.com/pt-br/)
- [Docker](https://www.docker.com/)
- Arquitetura Model-Service-Controller

### Alinhamento de código
- [ESlint](https://eslint.org/)

**Obs.:** Os arquivos presentes na pasta todo-app foram disponibilizados pela [Trybe](https://www.betrybe.com/) para a realização deste projeto.

## ⚙️ Execução

Para executar a aplicação inicie realizando o clone deste repositório com o comando abaixo.

    git clone git@github.com:cleciopinheiro/docker-todo-list.git
    
Navegue até o diretório **docker** do projeto.

    cd docker-todo-list/docker

<details>
   <summary><strong>Rodando a aplicação com o Docker</strong></summary> 
  </br>
  
  <strong>Obs:</strong> Para rodar a aplicação dessa forma você deve ter o [Docker](https://www.docker.com/) instalado na sua máquina.
  
  </br>
  
  Instale as depedências do projeto na pasta back-end, fornt-end e tests rodando o comando abaixo em cada pasta

        npm install
  
  Na pasta docker do projeto, suba o container <strong>todofront</strong>, <strong>todoback</strong> e <strong>todotests</strong> utilizando o docker-compose.yml. Utilize o comando abaixo.

        docker-compose up -d

Entre no terminal do container de back-end

        docker exec -it todoback bash

Dentro do terminal, inicie o servidor

        npm run dev
        
 Entre no terminal do container de front-end
    
        docker exec -it todofront bash
        
 Inicie a aplicação react com o comando abaixo dentro do terminal do container
    
        npm start

</details>

---

Desenvolvido por [Clécio Pinheiro](https://www.linkedin.com/in/cleciopinheirodev), © 2023.
