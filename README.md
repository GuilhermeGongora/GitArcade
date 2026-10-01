# Git Arcade

Jogo de Git no navegador, feito para a palestra **"Entendendo Git: um guia de versionamento"** na Semana de Tecnologia da Unisanta.

Você digita comandos Git num terminal simulado e vê, a cada comando, os ponteiros (branches e HEAD) andando no grafo de commits e os objetos (blob, tree, commit) sendo criados dentro da `.git`. Os hashes são SHA-1 de verdade.

## Como jogar

1. Abra o jogo, digite seu nome e aperte **PRESS START**. O cronômetro começa aí.
2. São 9 fases liberadas em sequência: commit, stage seletivo, branch, fast-forward, merge de 3 vias, detached HEAD, reset, reflog e o **BOSS**: um conflito de merge.
3. Você tem **3 dicas** para o jogo inteiro.
4. Pontuação: 1000 por fase, menos 150 por comando além do par. Comandos de consulta (`status`, `log`, `reflog`, `cat`, `ls`) são grátis.
5. Derrotou o boss? O cronômetro para e você ganha um certificado de lembrança com seu nome, tempo e um código de verificação.

Digite `help` no terminal para ver todos os comandos aceitos.

## Ranking

Nesta versão o ranking fica salvo no próprio navegador. Para entrar no ranking da sala, mostre o certificado ao palestrante.

## Rodar localmente

É um arquivo HTML único, sem build e sem dependências: abra o `index.html` no navegador.

---

Feito por Guilherme Gongora · Semana de Tecnologia · Unisanta
