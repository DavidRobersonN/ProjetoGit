COMO FAZER O PRIMEIRO PUSH NO GITHUB

    o primeiro passo é criar o repositorio no git, entao dentro da pasta do projeto sera digitado
no terminal do gitbash, o seguinte codigo:

    git init

    Dentro da pasta do nosso projeto, precisa ter o arquivo Readme.md, o proximo passo sera digitar o seguinte codigo na linha de comando:

    git add Readme.md

    este comando coloca os arquivos na area de Staging
    O proximo passo sera fazer o commit, com a seguinte linha de codigo:

    git commit -m "Primeiro commit"

A proxima etapa, seria fazer o push do nosso codigo, mas como é primeira vez que estamos conectando para o git hub, precisamos fazer algumas coisas...
    o seguinte codigo, ira mudar o nome da nossa branch de master para "main", o que é uma boa pratica em programação

    git brach -M "main"

    Precisa criar o repositorio no gitHub, onde o codigo sera hospedado, é bem simples, é feito no site do github mesmo, lá tmb tera o link, para ser feito a conexao no gitBash
    
    Voltando para o gitbash, vamos digitar o seguinte codigo para fazer a coneção entre o gitHub e a nossa maquina.

    git remote add origin https://github.com/DavidRobersonN/ProjetoGit.git

    Finalmente faremos o push

    git push -u origin main

    esta feito!
    Caso seja feito alguma alteração no codigo, a seguinte linha de comando adiciona as alterações no git hub

    git add . (O espaço depois do ponto, indica para add tudo que esta no diretorio, ou seja, na só a ultima alteração)

    git commit "detAlhes da alteração"

    git push origin main

CRIANDO UMA NOVA BRANCH

O conceito de criar uma nova branch, é criar uma nova ramificação do projeto, ou seja, tudo que for feito dali em diante, nao altera o codigo principal do projeto