# Treinando nosso trabalho em equipe

Este repositório servirá para treinarmos nosso fluxo de trabalho em equipe usando git e o Github.

## 1. Clone

Clone o repositório para seu ambiente de desenvolvimento.

`git clone https://github.com/bcc-dw-20212/treino-fluxodetrabalho.git`

Visto que o repositório está marcado como público, não haverá pedido de credenciais. Porém, precisamos configurar seus usuários no ambiente para que a interação consiga acompanhar quem realizou cada tarefa.

`git config --global user.name "Seu Nome"`

`git config --global user.email "seuemail@ifce.edu.br"`

Visto que o repositório foi clonado, ele já possuirá uma referência para o mesmo na variável "origin". O branch principal é o branch "main".

## 2. Você está trabalhando no projeto

Crie um arquivo dentro do diretório local do projeto, com seu primeiro nome e a extensão txt e adicione qualquer conteúdo.

Sempre que algum arquivo novo for criado, ou alguma alteração for realizada em já existentes, é possível verificar se o git está a par das alterações com:

`git status`

Você observará que a resposta do comando indicará recomendações sobre o que fazer. Esses arquivos ainda não estão preparados para commit (consolidar as alterações) e envio ao repositório remoto. Você pode dizer que devem ser preparados com:

`git add nomedoarquivo`

É possível indicar vários ao mesmo tempo.

Registre as alterações que você fez neste "dia de trabalho" com:

`git commit -m "Tarefa tal e tal concluída"`

Para sincronizar, envie para o repsitório remoto com:

`git push origin main`

Caso necessário, entre suas credenciais.

## 3. Alguém alterou o repositório entre a última vez que você atualizou e agora (push)

Antes de enviar suas alterações,sempre é preciso garantir que seu repositório local reflete a última versão do repositório remoto como alicerce.

`git pull origin main`

Em geral este comando deve ser executado antes de iniciar suas tarefas do dia.

Em casos onde outra pessoa trabalhou no mesmo arquivo, talvez seja necessário resolver um conflito de conteúdo (digamos que a pessoa apagou um trecho que você queria manter).

## 4. Evitando conflitos ao implementar novas funcionalidades

Nunca trabalhe no main. O ideal é criar branches locais. Branches são cópias exatas de como o código estava em determinado momento, e nomeadas. É possível criar um branch com:

`git branch tarefa-exemplo` (para os teste dê um nome aleatório)

E você pode alterar entre o branch ativo com:

`git checkout tarefa-exemplo`

O que o git faz na prática é chavear entre os arquivos e suas versões.

Você pode enviar seu branch para o repositório remoto com:

`git push origin tarefa-exemplo`

## 5. Fiz uma alteração e ela precisa de discussão para ser levada a versão oficial do projeto

O Github possui a funcionalidade de pull request, onde você abre uma espécie de fórum de discussão e revisão, em que membros autorizados da equipe poderão acompanhar as alterações e realizar a fusão (merge), automática ou assistida.

Vamos praticar?
