# Jogo da Velha

Projeto web de Jogo da Velha com interface em tema escuro neon, desenvolvido com HTML, CSS e JavaScript puro.

## Visao geral

O projeto possui dois modos de jogo:

- `JXJ` (Jogador vs Jogador): dois usuarios jogam no mesmo dispositivo.
- `JXIA` (Jogador vs IA): voce joga contra o bot, que usa minimax para escolher a melhor jogada.

Visual atual:

- Tema escuro com destaque neon.
- `X` em vermelho neon.
- `O` em azul neon.

## Tecnologias

- HTML5
- CSS3
- JavaScript (sem framework)

## Estrutura do projeto

```text
jogoDaVelha/
├─ index.html          # entrada principal (redireciona)
├─ bot.html            # modo Jogador x IA
├─ user.html           # modo Jogador x Jogador
├─ js/
│  ├─ bot.js           # logica da IA (minimax)
│  └─ user.js          # logica do modo PvP
└─ styles/
	└─ style.css        # estilos e tema neon
```

## Como executar localmente

Como e um site estatico, basta abrir um dos arquivos HTML no navegador:

- `index.html` (entrada principal)
- `bot.html` (JXIA)
- `user.html` (JXJ)

Se preferir rodar com servidor local simples:

```bash
npx serve .
```

## Regras do jogo

- O tabuleiro tem 9 casas (3x3).
- Ganha quem completar 3 simbolos iguais na horizontal, vertical ou diagonal.
- Se todas as casas forem preenchidas sem vencedor, termina em empate.

## Deploy no Vercel

O projeto ja esta pronto para deploy estatico.

```bash
npm i -g vercel
vercel login
vercel
vercel --prod
```

