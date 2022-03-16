# Comandos Básicos para GIT :spiral_notepad:

:point_right: O git possui diversas funcionalidades que são acessadas por comandos específicos! Para quem está começando agora, pode ser difícil memorizar tudo, então, segue um guia de comandos básicos!

##### git config

Define seu nome de usuário e e-mail, que estarão presentes nos commits feitos. Se utilizarmos --global, como mostrado a baixo, será necessário realizar o processo apenas uma vez.

> git config --global user.email seuemail@exemplo.com.br
>
> git config --global user.name "Seu Nome"    

#### git init

Inicializa um repositório em um diretório já existente. Para isso, basta ir ao diretório desejado e digitar o comando, criando então um diretório oculto denominado .git. 

> git init

#### git clone

Outro modo de obter um projeto, é clonando um repositório git a partir de outro servidor. Para isso, você precisa da url do servidor que deseja clonar, como no exemplo a baixo.

> git clone git@github.com:yagobenner/desafio-dio-primeiro-repositorio.git

#### git add

Quando um repositório é iniciado através do git init, ele ainda não está sendo monitorado. Já quando clonamos um repositório, ele está sendo monitorado, pois nenhuma alteração ainda foi feita. Para começarmos a monitorar o repositório novo ou monitorar alterações feitas nos demais repositórios, utilizamos o mesmo comando.

> git add *

Caso você deseje neste momento monitorar apenas o arquivo readme, podemos especificar isso através do comando

> git add README

Estes arquivos farão parte do seu próximo commit.

#### git status

Este comando permite que você veja se existem arquivos novos ou alterados que não estejam sendo monitorados ainda, ou que possam estar sendo monitorados, mas ainda não foram enviados (commited).

> git status

#### git commit

Após os novos arquivos estarem sendo monitorados, vamos então armazenar o conteúdo atual em seu repositório, utilizando o commit, junto com uma mensagem que fale o que está sendo alterado neste commit.

> git commit -m "Adição do arquivo x"

#### git push

Envia os commits de seu repositório local para o remoto. Para isso, vamos utilizar o nome do nosso repositório remoto, seguido do nome da nossa branch.

> git push origin(rep remoto) main(branch)

#### git pull

Repositórios remotos permitem que estes arquivos sejam alterados simultaneamente. Caso uma alteração seja feita e enviada ao repositório por outra pessoa, vamos precisar incorporar estas alterações em nossa branch antes de enviarmos as atualizações feitas por nós.

> git pull origin(rep remoto) main(branch)