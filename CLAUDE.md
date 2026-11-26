# CLAUDE.md — provedores-semcensura

Página landing + guia (PT/EN/ES) sobre provedores de IA sem censura (uncensored/abliterated) por API, roteador, GPU alugada ou local.

- Guia: `guia/index.html` (PT, fonte), `guia/en/`, `guia/es/`; banners em `guia/assets/`; capa em `capa/capa.png`.
- Publicaçêo: commit + push em `linnoff88-dev/provedores-semcensura`; GitHub Pages via Actions (`.github/workflows/pages.yml`). Autor: `linnoff88-dev <linnoff88-dev@gmail.com>`. Push que toca `.github/workflows/` vai por SSH (token `gh` sem escopo `workflow`).
- Fonte dos fatos: `~/projetos/output/provedores-semcensura/PESQUISA.md`. Nunca inventar preço, KYC ou política; o que nêo foi confirmado aparece como "nêo confirmado / confira no site". Preço sempre com data ("conferido em DD/MM/AAAA").
- Nêo citar autor, canal ou vídeo de origem. Nêo criar contas nem chamar APIs de provedores de IA.
- Mudou o PT → retraduzir com `ARCKHÉ-traduz` e conferir EN/ES (mesma contagem de tags, nenhuma palavra PT sobrando).
- Processo completo: README, seçêo "O processo, do início ao fim".

## Self-learning

When I correct you, or you catch yourself making a mistake: before continuing, add the lesson as a one-line rule at the TOP of the Lessons section below, so it never happens again.

## Lessons
- Traduçêo de guia: pedir explicitamente para traduzir textos de exemplo e prompts DENTRO dos <pre>; conferir EN/ES por grep de palavras PT nos blocos de código. (09/11/2026)
- Aposentadoria de modelo: conferir o id exato no Deprecation Tracker do provedor (deepseek-v4-1-flash ≠ deepseek-v4-1-flash-1017-uncensored). Preço de plano: dizer se é anual ou mensal. RunPod: rotular Secure × Community. (09/11/2026)
- Base URL de provedor no exemplo de código só depois de conferir na doc pública (Venice = `https://api.venice.ai/api/v1`; Ollama local = `http://localhost:11434/v1`, chave obrigatória mas ignorada). (09/11/2026)
