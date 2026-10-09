# Git Arcade

Jogo de Git no navegador, feito para o minicurso **"Entendendo Git: um guia de versionamento"** na Semana de Tecnologia da Unisanta.

Você digita comandos Git num terminal simulado e vê, a cada comando, os ponteiros (branches e HEAD) andando no grafo de commits e os objetos (blob, tree, commit) sendo criados dentro da `.git`. Os hashes são SHA-1 de verdade.

## Como jogar

1. Abra o jogo, digite seu nome (ele vai para o ranking e para o certificado) e aperte **PRESS START**.
2. São **2 mundos e 16 fases**, liberadas em sequência:
   - **Mundo 1:** commit, stage seletivo, branch, fast-forward, merge de 3 vias, detached HEAD, reset, reflog e o **BOSS** do conflito de merge.
   - **Mundo 2:** stash, revert, `commit --amend`, cherry-pick, cat-file, rebase e os **GÊMEOS DO REBASE**.
3. **Limite de 30 minutos.** Se o tempo acabar, os bosses vencem e o jogo termina.
4. **Dicas** são compradas: cada uma soma +1:00 ao tempo e aponta o caminho, sem dar o comando pronto.
5. **Pular fase:** até 2 vezes (boss não), e a fase pulada vale 0 pontos. Também dá para **desistir**.
6. Pontuação: 1000 por fase, menos 150 por comando além do par. Comandos de consulta (`status`, `log`, `reflog`, `cat`, `ls`) são grátis.
7. São dois certificados, com nome, tempo e código de verificação, prontos para o LinkedIn: o do **Mundo 1** sai ao derrotar o primeiro boss, e o **final** ao derrotar os dois dentro do tempo.
8. **Pausa entre os mundos:** ao derrotar o primeiro boss, o relógio **para**, o resultado entra no **ranking do Mundo 1** e o certificado do Mundo 1 é liberado. O jogador escolhe se encara o Mundo 2: ao continuar, o relógio volta a correr de onde parou, e só entra no **ranking final** quem vence os dois bosses dentro dos 30 minutos.

Digite `help` no terminal para ver todos os comandos aceitos. Há 23 segredos escondidos, uma sala secreta com pistas e um tesouro dentro de uma `.git` que você explora pelo endereço do site.

## Arquivos

- `index.html`: o jogo.
- `admin.html`: painel do palestrante (login Google, acesso restrito).
- `img/`: sprites dos bosses, foto e ícones.
- `firestore.rules`: regras de segurança do Firestore (ranking final, ranking do Mundo 1 em `ranking1`, telemetria e avaliações). Publique de novo sempre que este arquivo mudar.

---

Feito por Guilherme Gongora · Semana de Tecnologia · Unisanta

## Modo palco

Abra `…/GitArcade/?palco` para um terminal livre com o Git do jogo (repositório vazio, sem cronômetro e sem ranking), útil para demonstrações ao vivo. O painel `admin.html` traz o mesmo terminal na seção TERMINAL AO VIVO.
