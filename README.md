# TutorialGit

CRIAR REPOSITÓRIO DO 0 E UPAR O PROJETO DA MÁQUINA LOCAL

1. git init
2. git add .
3. git commit -m "mensagem"
4. git branch -M "main"
5. git remote add origin linkdorepositorio
6. git push -u origin main

* o "." no final da linha 2 faz com que todos os arquivos sejam adicionados. Para adicionar apenas um, basta botar o nome
* a linha 4 serve para mudar o nome da branch de MASTER para MAIN
* a linha 5 serve para fazer a conexão do repositório local com o github

-------

UPAR AS ALTERAÇÕES LOCAIS NO REPOSITÓRIO

1. git add .
2. git commit -m "mensagem"
3. git push origin main

* não precisa da linha 4 e 5 do código anterior, nem do "-u" da linha 6

-------

CRIAR UMA BRANCH E UPAR AS ALTERAÇÕES

1. git checkout -b "nomedanovabranch"
2. git add .
3. git commit -m "mensagem"
4. git push origin nomedanovabranch

* na linha 1, o "checkout" serve para trocar de branch, e o "-b" serve para criar uma nova 

-------

ALTERNAR ENTRE AS BRANCHES

1. git checkout main
2. git checkout nomedanovabranch

* como as branches já estão criadas, não precisa do "-b"

-------

PASSAR A BRANCH CRIADA PARA A BRANCH PRINCIPAL(MAIN)

1. git checkout main
2. git merge nomedanovabranch
3. git push origin main

* é necessário ir para a branch main e dar o merge da branch que deseja upar 

-------

PEGAR OS ARQUIVOS DO PROJETO PELA PRIMEIRA VEZ

1. git clone linkdorepositorio

* esse comando só serve na primeira vez, porque ele pega todos os arquivos existentes no projeto, e não apenas as futuras alterações

-------

PEGAR AS NOVAS ALTERAÇÕES DO PROJETO DEPOIS DE CLONAR

1. git checkout main
2. git pull

-------

COMANDOS IMPORTANTES (BÔNUS)

git status
clear
cd pasta

* os conceitos de fork e pull request também são importantes, porém se faz pelo próprio github

-------

fontes:
https://github.com/rafaballerini/GitTutorial
https://youtu.be/DqTITcMq68k
https://youtu.be/UBAX-13g8OM
