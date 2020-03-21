# AULA 01 - GIT

COPIE E COLE - NÃO RECORTE =)

AULA 01 - GIT | FULL STACK BLEND

PARTE 01

1) O que é o GitHub?
Git é a tecnologia, GitHub é uma 'hospedagem de repositórios', que usa o git. É um dos mais famosos, mas há outros, como o BitBucket.

2) Para que serve o versionamento?
Segurança, agilidade, back up, precaução, compartilhamento, colaboração, exposição, recrutamento...

3) Configurando nossa máquina para trabalhar com o github

Gerar chave SSH
https://help.github.com/en/enterprise/2.17/user/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

Observação: esse primeiro cifrão não deve ser copiado, ele indica que é uma linha de código no terminal (que deve ser digitado por vocês)

$ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

$ eval $(ssh-agent -s)

$ ssh-add ~/.ssh/id_rsa

Adicionar chave SSH à conta github
https://help.github.com/en/enterprise/2.17/user/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account

$ clip < ~/.ssh/id_rsa.pub

Colar no painel lá no github.com

4) Configurar usuário e senha na máquina:

Pelo gitbash, vamos digitar os seguintes comandos (trocando o que está entre aspas pelos seus dados). Atenção, se a máquina não for particular sua, não copie o '--global', assim o usuário fica atrelado apenas ao repositório, não à máquina.

$ git config --global user.name "Nome Sobrenome"

$ git config --global user.email "seuemail@examplo.com"


PARTE 02

1) Criar um repositório no github.com (remoto)

2) Clonar um repositório

$ git clone endereco-do-repositorio

3) Abrir no VS Code (definir terminal embutido padrão como Bash)

4) Puxar atualizações do repositório remoto

$ git pull

!!! IMPORTANTE SEMPRE DAR UM GIT PULL ANTES DE COMEÇAR A CODAR !!!

5) Alterar o arquivo README.md com MarkDown (dillinger.io)

6) Adicionar alterações (o ponto traz todas atualizações, ou podemos declarar uma pasta ou arquivo)

$ git add .
$ git add README.md
$ git add assets/*

7) Commitar as alterações - como fechar um pacote de updates

$ git commit -m 'descrição do commit'

8) Subir atualizações no repositório

$ git push

9) Verificar status do repositório

$ git status


PARTE 03

1)  Entender git flow

2) Criar uma branch nova a partir de uma existente

$ git checkout -b nome-da-branch

3) Atualizar a branch conforme passos anteriores, mas indicando a branch de origem

$ git add . && git commit -m 'mensagem' && git push origin nome-da-branch

4) Abrir um PR (Pull Request) e configurá-lo (definir para que branch irá, qual a atualização...)

5) Aprovar uma PR após Code Review

6) Voltar para a branch master e mergear a branch nova a partir dela

$ git checkout master

$ git merge nova-branch

7) Atualizar o repositório remoto

$ git push


PARTE 04

1) Criando repositório para começar o projeto do currículo

2) Apresentação do HTML
