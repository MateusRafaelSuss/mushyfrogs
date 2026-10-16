MUSHYFROG — PIXEL QUEST
================================

COMO EXECUTAR LOCALMENTE
1. Extraia a pasta do ZIP.
2. Abra index.html no navegador para jogar no computador ou experimentar os controles de toque em um dispositivo compatível.
3. Para testar recursos PWA/offline localmente, use um servidor local (por exemplo: python -m http.server) porque service workers exigem HTTPS ou localhost.

CONTROLES NO COMPUTADOR
- A / D ou setas: mover
- Espaço, W ou seta para cima: pular
- P ou Esc: pausar/retomar
- R: reiniciar a campanha

CONTROLES NO CELULAR
- ◀ / ▶: movimentar (é possível manter pressionado)
- PULAR: saltar; pode ser pressionado ao mesmo tempo que um botão de direção
- Ⅱ: pausar
- ⛶: solicitar tela cheia (a disponibilidade depende do navegador)
- Recomendado jogar com o celular na horizontal.

PWA / CLOUDFLARE PAGES
O projeto inclui manifest.webmanifest, ícones e sw.js para instalação em navegadores compatíveis e cache do jogo para uso offline após o primeiro carregamento bem-sucedido. Publique todos os arquivos mantendo a estrutura das pastas. Cloudflare Pages serve o site em HTTPS, necessário para service workers fora de localhost.

ESTRUTURA
- index.html: jogo e controles
- assets/: sprites do sapinho
- icons/: ícones PWA
- manifest.webmanifest: configurações da instalação
- sw.js: cache e fallback offline

Observação: os navegadores e sistemas operacionais variam quanto à instalação PWA, tela cheia e execução offline. Teste no aparelho-alvo após publicar.
