# Mini-Projeto Linux sobre FHS (Filsysteme Hierarchy Standard)

Este repositorio documenta um exercicio pratico para entender a organizacao de arquivos no Linux de acordo com o **FHS**.

## Objetivo

Simular a "instalacao" manual de uma aplicacao de linha de comando ficticia (`infosis`) posicionando corretamente cada um de seus componentes (executavel, configuracao, manual) em uma estrutura de diretorios que espelha a hierarquia padrao do Linux.

## O Projeto

Foi criada uma aplicacao ficticia chamada `infosis` e uma estrutura de diretorios chamada `fhs_simulado`. 
Os arquivos da aplicacao foram movidos para seus locais corretos dentro desta estrutura demonstrando o entendimento dos seguintes diretorios padrao:

- `/usr/local/bin` - Para o binario executavel.
- `/etc` - Para o arquivo de configuracao.
- `/usr/local/share/man/man1` - Para a pagina de manual.
- `/var/log` - Diretorio reservado para logs da aplicacao.

## Estrutura Final

A estrutura final pode ser visualizada com o comando `tree`, demonstrando a correta aplicacao dos conceitos de FHS:

**fhs_simulado**
|___________etc

     |_____infosis.conf

|___________usr

     |_____local

        |_____bin

           |_____infosis

        |_____share

           |_____man

              |_____man1

                 |_____infosis.1

|___________var 

|___________log


