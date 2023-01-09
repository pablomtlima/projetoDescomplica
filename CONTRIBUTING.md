# CONTRIBUTING

Este documento tem o objetivo de esclarecer o fluxo para contribuir para o projeto.

## BRANCHES 

- main: código estável para implantação
- dev: código de desenvolvimento. As branches de features são originadas deste repositório
- issue-x/ feature-x: código relacionado a uma issue/feature específica. Sua criação é local. Só pode ser enviada para o servidor quando concluída e para abertura de pull request. Após PR ela é excluída do repositório remoto

## WORKFLOW

1. Identificar a issue que irá trabalhar e se inteirar sobre ela. Caso seja um tema novo, abrir uma issue para permitir contribuições sobre o tema
2. Clonar o repositório para o seu computador: ```git clone https://github.com/pablomtlima/projetoDescomplica.git```
3. Acessar o diretório de trabalho ```cd projetoDescomplica```
4. Acessar o branch dev: ```git checkout dev```
5. Criar um branch local de trabalho: ```git checkout -b issue-1```
6. while coffee: codificar e commitar (pequenos commits, baby steps)
7. Concluída a feature, realizar o fetch do repositório e rebase do branch da feature: ```git fetch & git rebase origin/dev``` (* decidir futuramente se convém usar squash no rebase para não poluir tanto o código final com os commits de interesse local apenas)
8. Realizar o push do branch: ```git push origin issue-1```
9. Após enviado para o servidor o branch local issue-1 não deve mais ser utilizado, até o resultado da PR. (alerta: não deve ser feito rebase em um branch que já foi enviado para um servidor remoto!)
10. Abrir um Pull(merge) Request no Github para apreciação de outros colaboradores
11. Os colaboradores que avaliarem o PR fazem o merge com o branch dev e removem o branch temporário da issue/feature (aqui teria mais coisa pois os colaboradores podem corrigir algo ou solicitar que seja corrigido.)

_Obs.: Este documento está em fase de construção e não representa o modelo de fluxo a ser seguido atualmente._