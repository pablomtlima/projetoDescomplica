# CONTRIBUTING

Este documento tem o objetivo de esclarecer o fluxo para contribuir para o projeto.

## BRANCHES 

- main: c�digo est�vel para implanta��o
- dev: c�digo de desenvolvimento. As branches de features s�o originadas deste reposit�rio
- issue-x/ feature-x: c�digo relacionado a uma issue/feature espec�fica. Sua cria��o � local. S� pode ser enviada para o servidor quando conclu�da e para abertura de pull request. Ap�s PR ela � exclu�da do reposit�rio remoto

## WORKFLOW

1. Identificar a issue que ir� trabalhar e se inteirar sobre ela. Caso seja um tema novo, abrir uma issue para permitir contribui��es sobre o tema
2. Clonar o reposit�rio para o seu computador: ```git clone https://github.com/pablomtlima/projetoDescomplica.git```
3. Acessar o diret�rio de trabalho ```cd projetoDescomplica```
4. Acessar o branch dev: ```git checkout dev```
5. Criar um branch local de trabalho: ```git checkout -b issue-1```
6. while coffee: codificar e commitar (pequenos commits, baby steps)
7. Conclu�da a feature, realizar o fetch do reposit�rio e rebase do branch da feature: ```git fetch & git rebase origin/dev``` (* decidir futuramente se conv�m usar squash no rebase para n�o poluir tanto o c�digo final com os commits de interesse local apenas)
8. Realizar o push do branch: ```git push origin issue-1```
9. Ap�s enviado para o servidor o branch local issue-1 n�o deve mais ser utilizado, at� o resultado da PR. (alerta: n�o deve ser feito rebase em um branch que j� foi enviado para um servidor remoto!)
10. Abrir um Pull(merge) Request no Github para aprecia��o de outros colaboradores
11. Os colaboradores que avaliarem o PR fazem o merge com o branch dev e removem o branch tempor�rio da issue/feature (aqui teria mais coisa pois os colaboradores podem corrigir algo ou solicitar que seja corrigido.)

_Obs.: Este documento est� em fase de constru��o e n�o representa o modelo de fluxo a ser seguido atualmente._