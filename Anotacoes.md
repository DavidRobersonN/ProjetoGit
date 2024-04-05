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

Ao criar uma nova feature, "alguma alteração no projeto"  precisamos antes criar uma nova branch, vamos ao passo. digite o seguinte codigo:

    git checkout -b "novo-botao"

    estamos criando uma branch nova, e ao mesmo tempo, saindo da branch main e entrando na brach novo-botao

    Apos fazer as alterações no codigo, precisa fazer os seguintes codigos:

    git add .

    git commit -m "alterações para novo-botao"

    git push origin novo-botao

Caso queira voltar para brach main, ultiliza-se o seguinte comando:

    git checkout main

COMO REALIZAR UM MERGE
    merge significa, juntar uma nova branch que foi criada, com o codigo principal
    o primeiro passo é voltar para a branch principal, no caso main
    usaremos o seguinte codigo:

    git merge novo-botao

    isso juntara a branch novo-botao, com a branch main, em seguida um push

    git push origin main

GIT CLONE
Um git clone, significa clonar um projeto para a sua maquina, muito simples.

    -primeiro copiamos o codigo no github do projeto
    -agora criamos um diretorio na nossa maquina, onde o projeto vai ficar salvo
    -abrimos o gitbash dentro deste diretorio e colocamos o seguinte codigo:
        git clone https://github.com/DavidRobersonN/fusion.git

GIT PULL
Fazer um git pull significa atualizar o codigo na nossa maquina, caso seja feito alguma alteração no projeto dentro do github, e o codigo na nossa maquina fique desatualizado
    muito simples, basta digitar o seguinte codigo no gitbash:

    git pull

FORK
Realizar um fork significa adicionar o projeto de outro perfil no github, e adicionar ao seu perfil, basta ir no projeto que deseja adicionar, e clicar na opção FORK

PULL REQUEST
Apos realizar um fork no projeto de alguem, vc pode fazer suas alterações e melhorias no codigo, e contribuir para esse projeto realizando um PULL REQUEST
    
    Primeiro realiza-se um commit, e depois finalmente, Open_pull_request
    (Open_pull_request fica na opção contribute no proprio github)

ACEITANDO UMA PULL REQUEST
Alguem pode tmb querer fazer uma alteração no nosso codigo, caso queira aceitar, na aba pull requests,  existe opção merge pull request, onde vc pode aceitar ou rejeitar uma pull request

