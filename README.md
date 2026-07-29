# 🚀 DESAFIO 01 - A ARENA FAUNADEX (A CONSTRUÇÃO PASSO A PASSO)
## Engenharia de Software ULTRA DIDÁTICA | SaaS Smart Academy Reborn

> **🎯 OBJETIVO EXTRAORDINÁRIO:** Seu cérebro não aprende copiando um código gigante de uma vez. Ele aprende quebrando problemas grandes em pedacinhos minúsculos (Baby Steps). Vamos construir a Arena de Duelo do **Faunadex** (estilo Triple Triad do Final Fantasy 8) tijolo por tijolo. E a regra de ouro: A cada tijolo assentado, nós salvamos o jogo (Git Commit).
> **🎯 OBJETIVO EXTRAORDINÁRIO:** Seu cérebro não aprende copiando um código gigante de uma vez. Ele aprende quebrando problemas grandes em pedacinhos minúsculos (Baby Steps). Vamos construir a Arena de Duelo do **Faunadex** (estilo Triple Triad do Final Fantasy 8) tijolo por tijolo. E a regra de ouro: A cada tijolo assentado, nós salvamos o jogo (Git Commit) usando a própria interface visual do VSCode, sem dor de cabeça no terminal!

---

## 🆔 PASSO 0: PREPARANDO O SEU CRACHÁ

Antes de começar a programar, o VSCode precisa saber quem você é para assinar os seus salvamentos (commits). Se você não fizer isso, ele vai dar erro.

1. Abra o Terminal no VSCode (`Ctrl + '` ou `Menu Terminal > New Terminal`).
2. Digite os dois comandos abaixo (substituindo pelo seu nome e e-mail do GitHub) e aperte Enter:
```bash
git config  user.name "Seu Nome"
git config  user.email "seu@email.com"
```
*Pronto! Nunca mais você precisará fazer isso no seu computador.*

---

@@ -67,11 +81,10 @@ A primeira coisa é montar a estrutura HTML sem beleza nenhuma, apenas caixas va
```
Abra no navegador. Você verá as três divs empilhadas uma em cima da outra. Feio, não é? Vamos salvar e consertar isso.

💾 **O SAVE GAME OBRIGATÓRIO (No Terminal):**
```bash
git add .
git commit -m "Passo 1: Esqueleto HTML e fundo escuro criados"
```
💾 **O SAVE GAME OBRIGATÓRIO (Usando o Mouse no VSCode):**
1. Clique no ícone de **Source Control** (um desenho com três bolinhas conectadas) no menu esquerdo do VSCode.
2. Na caixinha de texto (Message), digite: `Passo 1: Esqueleto HTML e fundo escuro criados`.
3. Clique no botão azul **Commit**. Se ele perguntar se deseja fazer "stage" em todas as mudanças, clique em **Yes (Sim)**.

---

@@ -97,11 +110,10 @@ Vá na tag `<style>` do seu arquivo e **adicione/modifique** o CSS da classe `.a

Atualize o navegador (`F5`). **BUM!** Magicamente as três áreas estão uma do lado da outra perfeitamente alinhadas.

💾 **O SAVE GAME OBRIGATÓRIO (No Terminal):**
```bash
git add .
git commit -m "Passo 2: Implementado CSS Grid com 3 colunas principais"
```
💾 **O SAVE GAME OBRIGATÓRIO:**
1. Vá no **Source Control** do VSCode.
2. Digite a mensagem: `Passo 2: Implementado CSS Grid com 3 colunas principais`.
3. Clique em **Commit**.

---

@@ -136,7 +148,7 @@ Agora vamos focar nas pontas. O jogador precisa segurar 5 cartas uma embaixo da
        /* Transformando a Mão em um Grid de 5 linhas */
        .mao-aliado, .mao-inimigo {
            display: grid;
            grid-template-rows: repeat(5, 120px); /* 5 linhas de 120px de altura */
            grid-template-rows: repeat(5, 1fr); /* 5 linhas dividindo a altura por igual */
            gap: 15px;
            border: none; /* Tirando a borda feia do Passo 1 */
        }
@@ -160,14 +172,13 @@ Agora vamos focar nas pontas. O jogador precisa segurar 5 cartas uma embaixo da
Atualize o navegador. Suas 5 cartas verdes na esquerda e 5 vermelhas na direita nasceram!

💾 **O SAVE GAME OBRIGATÓRIO:**
```bash
git add .
git commit -m "Passo 3: Layout de 5 cartas criado para aliado e inimigo"
```
1. Vá no **Source Control** do VSCode.
2. Digite a mensagem: `Passo 3: Layout de 5 cartas criado para aliado e inimigo`.
3. Clique em **Commit**.

---

## 🎲 PASSO 4: O CAMPO DE BATALHA (A MESA 3x3)
## 🎲 PASSO 4: O CAMPO DE BATALHA E O GITHUB

O último desafio é o mais importante. O meio da mesa precisa ser uma matriz perfeita de 3x3. Como o `CSS Grid` faz isso de olhos fechados? Nós pedimos `repeat(3)`.

@@ -190,9 +201,9 @@ O último desafio é o mais importante. O meio da mesa precisa ser uma matriz pe
```css
        .tabuleiro {
            display: grid;
            /* Magia Pura: 3 colunas iguais, 3 linhas iguais */
            /* Magia Pura: 3 colunas iguais, 3 linhas fluidas iguais */
            grid-template-columns: repeat(3, 1fr); 
            grid-template-rows: repeat(3, 140px);
            grid-template-rows: repeat(3, 1fr);
            gap: 10px;

            background-color: #0d1b2a;
@@ -218,16 +229,16 @@ O último desafio é o mais importante. O meio da mesa precisa ser uma matriz pe
        }
```

Atualize o navegador. **A TRÍADE ESTÁ COMPLETA!** Você criou um tabuleiro complexo passando por todas as fases sem copiar código cego.

💾 **O SAVE GAME OBRIGATÓRIO FINAL:**
```bash
git add .
git commit -m "Passo 4: Matriz 3x3 gerada no centro da mesa. Layout concluído!"
git push
```
Atualize o navegador. **A TRÍADE ESTÁ COMPLETA!**

*(Agora sim! Envie tudo para o GitHub e comemore).*
💾 **O SALVAMENTO FINAL E ENVIO PARA A NUVEM:**
1. Vá no **Source Control** do VSCode.
2. Digite a mensagem: `Passo 4: Matriz 3x3 gerada no centro da mesa`.
3. Clique em **Commit**.
4. **AGORA A MÁGICA DA NUVEM:** Clique no botão azul **Publish Branch** (ou "Publish to GitHub") que apareceu.
5. Um menu superior vai abrir. Escolha **"Publish to GitHub public repository"**.
6. Se o VSCode abrir uma janela no seu navegador pedindo permissão, clique em **Authorize / Allow** e volte pro VSCode.
7. Quando aparecer a mensagem de sucesso, todo o seu código estará blindado e seguro na nuvem da Microsoft!

---
