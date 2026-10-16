MUSHYFROG — PIXEL QUEST
================================

CONTROLES NO COMPUTADOR
- A / D ou setas: mover
- Espaço, W ou seta para cima: pular
- Depois de desbloquear a habilidade, pressione pular novamente no ar para o salto duplo
- P ou Esc: pausar/retomar
- R: reiniciar a fase atual

CONTROLES NO CELULAR
- ◀ / ▶: mover (é possível manter pressionado)
- PULAR: saltar; pode ser pressionado ao mesmo tempo que a direção
- Ⅱ: pausar
- ⛶: solicitar tela cheia (dependente do navegador)
- O tamanho dos botões pode ser ajustado em Configurações. Recomendado jogar na horizontal.

SISTEMAS DO JOGO
- 10 fases principais, mapa com fases desbloqueáveis e progresso salvo localmente
- Moedas, vidas, checkpoints, recordes e conclusão de fase
- Salto duplo desbloqueável, plataformas móveis, de impulso e que desmoronam
- Inimigos podem ser derrotados saltando sobre eles; três fases de chefe (fases 3, 6 e 10), cada uma com barra de vida, ataques próprios e projéteis que podem ser evitados com saltos
- Trilhas chiptune diferentes por fase e subfase, efeitos sonoros gerados pelo Web Audio, volume e opções de som
- Subfases secretas acessadas por tubulações usando ↓ ou S quando o sapinho está em cima do cano; a entrada usa uma animação de afundar e o retorno uma animação de emergência, com o sapinho surgindo centralizado sobre o cano e protegido brevemente contra dano imediato. Ranking global: ao terminar a campanha, o jogador pode enviar uma pontuação com apelido; o menu mostra as 10 maiores pontuações

RANKING GLOBAL / SUPABASE
O ranking usa a tabela public.scores no Supabase, com as colunas player_name, score e created_at (além de id). O navegador usa somente a chave publishable, e o acesso depende das políticas RLS configuradas no projeto Supabase. Para leitura pública, permita SELECT para anon; para envio de pontuações, permita INSERT para anon. Não coloque a chave service_role no front-end.

PWA / PUBLICAÇÃO
O projeto inclui manifest.webmanifest, ícones e sw.js para instalação em navegadores compatíveis e cache offline após o primeiro carregamento bem-sucedido. Publique todos os arquivos mantendo a estrutura das pastas. O nome do cache foi incrementado para mushyfrog-v9, forçando a atualização dos arquivos do jogo.

ARQUIVOS
- index.html: jogo, gráficos, áudio, controles e ranking global
- assets/: sprites atualizados do sapinho
- icons/: ícones PWA
- manifest.webmanifest: configurações da instalação
- sw.js: cache e fallback offline

Observação: PWA, tela cheia e modo offline dependem do navegador. O envio/leitura do ranking depende de conexão com a internet e das políticas RLS do Supabase. Não foi realizado teste de ponta a ponta com o Supabase nesta montagem.