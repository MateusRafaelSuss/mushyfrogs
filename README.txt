SALTO DO SAPINHO — PIXEL QUEST

Como jogar
1. Abra o arquivo index.html em um navegador moderno (Chrome, Edge ou Firefox).
2. Clique em JOGAR CAMPANHA ou use Enter.
3. Mova com A/D ou as setas esquerda/direita.
4. Pule com Espaço, W ou seta para cima.
5. P ou Esc pausa/retoma. R reinicia a campanha.
6. Colete moedas, toque nos checkpoints e alcance a bandeira verde para concluir cada fase.

O jogo é feito em HTML, CSS e JavaScript puro usando Canvas. Não exige instalação, servidor ou bibliotecas externas.

Fases
- Bosque Saltitante: introdução aos saltos, espinhos e slimes.
- Caverna Cristalina: mais perigos e plataformas móveis.
- Arquipélago das Nuvens: saltos mais longos, plataformas móveis e maior dificuldade.

Regras
- Cada moeda vale 10 pontos.
- Você começa com três vidas.
- Ao tocar em espinhos, slimes ou cair, perde uma vida e retorna ao último checkpoint.
- Ao terminar as três fases, o jogo exibe sua pontuação final.

Sprites
- O sapo usa assets/frog-sprites.png, uma spritesheet PNG transparente com 4 quadros de 32x32 (parado, corrida A, corrida B e pulo).
- Para trocar a aparência, mantenha os quadros lado a lado nesta ordem e atualize o arquivo PNG.

Checkpoints
- As bandeiras foram reposicionadas em plataformas sólidas e o código só ativa um checkpoint quando detecta uma plataforma de apoio na altura da bandeira. O renascimento fica centralizado acima dessa plataforma.
