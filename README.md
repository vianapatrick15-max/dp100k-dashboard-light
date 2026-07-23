# DP100K — Dashboard (tema claro)

Versão de tema claro, com visual premium e gráficos com gradiente, do dashboard geral
do DP100K. Mesmas views, métricas e dados do dashboard principal — apenas o design muda.

**Live:** https://vianapatrick15-max.github.io/dp100k-dashboard-light/

## Dados
Puxa o mesmo `data.json` do dashboard principal em tempo real (mesma origem GitHub Pages):
`https://vianapatrick15-max.github.io/dp100k-fp02-dashboard/data.json`.
Se a fonte estiver indisponível, cai no `data.json` local (espelhado de hora em hora
pelo workflow `mirror.yml`). Toda a lógica de negócio (funil, CPA, atribuição por UTM,
turmas) vive no repo principal `dp100k-fp02-dashboard`.

## Design
Tema claro profissional (padrão BI/apresentação de diretoria): tipografia **IBM Plex Sans**
com numerais tabulares, canvas com gradientes suaves, cards brancos com sombra, e gráfico
de área com preenchimento em gradiente + glow.

Preview dos ads = **embed do link do Instagram** (`instagram.com/p/<code>/embed` em iframe
lazy). Funciona porque o browser envia `Sec-Fetch-Dest: iframe` — sem esse header o IG
responde `X-Frame-Options: DENY`. Usar `/embed` (não `/embed/captioned`, que bloqueia).
Grade limitada ao top 60 por ordenação (embeds são pesados); fallback: thumb Meta ou link.
