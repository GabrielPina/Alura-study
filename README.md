<h1>ALURA STUDY</h1>

> Status do Projeto: Em desenvolvimento

Para rodar esse projeto na sua máquina, por favor digite:

```
node app.js
```

Comandos aprendidos no Curso da Alura, link do resumo -> https://guilhermeonrails.github.io/manual-do-git-e-github/

> Linhas de Comando utilizado durante o curso: 

Para clonar o projeto na máquina:
1° Ir no Projeto;
2° Clicar em CODE;
3° no HTTPS, clicar no botão de copiar;
4° Abrir o CMD;
5° escolher a pasta que gostaria de baixar o Projet;
6° digitar GIT CLONE (aqui o que foi copiado);
OBS.
Podemos realizar uma validação do que foi mexido no Projeto, utilizando a linha de comando:
CD (a pasta que se encontra o arquivo)
GIT LOG - esse comando informa quem mexeu no projeto.
GIT LOG --oneline (é um comando que usamos para ver os LOG em uma linha)

Para pegar uma versão atualizada do Projeto pelo CMD:
1° Ir no Projeto;
2° Clicar em CODE;
3° no HTTPS, clicar no botão de copiar;
4° Abrir o CMD;
5° Executamos o GIT PULL (linha de comando que valida se teve alguma atualização)
OBS. é uma atualização do projeto, ou seja, não puxamos o Projeto inteiro

Para mandar uma alteração do Projeto da sua máquina para o GitHub:
1° realizar a modificação do seu Projeto;
2° ir no terminal (tem como ir no terminal do VSCode, basta clicar em CTRL + J);
3° damos um GIT STATUS (no prompt de comando - CMD) para validar qualquer alteração e todo status do projeto;
4° para subir essa alteração do projeto damos o GIT COMMIT mandando apenas o arquivo que teve alteração identificada no 
GIT STATUS, no caso do curso da Alura iremos realizar o COMMIT no GIT COMMIT index.html, pois foi colocado a linha
do JavaScript (03-Trabalhando Localmente - aula 03 Git Status, commit e push).
5° para colocar uma mensagem nesse GIT COMMIT é só colocar o -m "AQUI A MENSAGEM".
6° o GIT PUSH vai ser a maneira como eu vou empurrar todos os COMMITs realizados na máquina LOCAL para o GITHUB 
(para deixar o mais atualizado, ou seja, a origem vai estar igual á sua máquina local).
7° GIT RESTORE é uma forma de voltar para um determinado momento da nossa aplicação
(pegando o ID que aparece antes do nome da alteração) 
Formato: git restore --source (numero da branch que vc quer voltar ou que foi commitada antes)

Aprendendo a usar o GIT ADD:
1° Quando usamos qualquer comando utilizando o PONTO, exemplo (GIT ADD .) nos estaremos adicionando todos os arquivos,
utilizar o PONTO tira o filtro.
FORMATO: git add (o que vc vai adicionar)
Como foi mostrado em aula:
1° usamos o GIT ADD .
2° usamos o GIT COMMIT -m "Criando uma pagina CONTATO"
3° usamos o GIT PUSH
4° validamos se a nova pasta foi criada no GitHub

Criar uma BRANCH:
1° no Prompt iremos digitar GIT CHECKOUT -b;
Formato: git checkout -b (nome da BRANCH).
OBS. ao executar o comando de criar um BRANCH nova, estaremos dentro dela, caso o DEV queira acessar a BRANCH do master ou 
até mesmo trocar para alguma outra, iremos usar o comando abaixo:
Formato: git switch (a BRANCH que vc quer entrar)
2° Fizemos uma alteração na BRANCH de desenvolvimento, como foi mostrado em aula:
1° usamos o GIT ADD .
2° usamos o GIT COMMIT -m "Adicionando o e-mail de contato"
3° usamos o GIT PUSH ORIGIN desenvolvimento (iremos dar um PUSH da alteração para a ORIGEM desenvolvimento e não mais para o main)

[MERGE] - Processo de passar as coisas (atualizações de código ou novas paginas) de BRANCH para outra/main:
GIT BRANCH -> é um comando que lista todas as BRANCHs disponiveis no projeto.
GIT MERGE desenvolvimento -> estamos juntando as BRANCHs de desenvolvimento com a main
Após o MERGE, temos que realizar o push.
GIT PUSH ORIGIN MAIN -> iremos enviar as alterações realizadas na BRANCH desenvolvimento para BRANCH main
Após o PUSH, poderemos validar a alteração no GitHub as alterações realizadas no MAIN
