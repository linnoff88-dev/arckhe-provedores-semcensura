# provedores-semcensura

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


[![IA sem censura: onde usar, quanto custa e o que conferir](guia/assets/banner.jpg)](https://inematds.github.io/provedores-semcensura/guia/)

**ðŸ‡§ðŸ‡· [PortuguÃªs](README.md) Â· ðŸ‡ºðŸ‡¸ [English](README.en.md) Â· ðŸ‡ªðŸ‡¸ [EspaÃ±ol](README.es.md)**

## O que Ã©

Este guia mostra onde encontrar modelos de IA â€œsem censuraâ€, ou seja, versÃµes que nÃ£o recusam pedidos. Serve para quem testa a seguranÃ§a do prÃ³prio sistema, pesquisa ou sÃ³ quer um assistente que nÃ£o trave em assunto delicado. VocÃª vÃª numa tabela os provedores por API, por chat, por GPU alugada e no seu prÃ³prio computador, com preÃ§o, privacidade declarada e se pedem identidade. Para usar, basta ler; os exemplos pedem uma conta no provedor escolhido ou o Ollama instalado.

## ðŸ“– Guia de uso

Guia completo (landing + passo a passo): **https://inematds.github.io/provedores-semcensura/guia/**

## O que tem no guia

- DiferenÃ§a entre **uncensored** (fine-tune, tipo Dolphin), **abliterated** (remove a â€œdireÃ§Ã£o de recusaâ€ dos pesos, sem treinar) e **jailbroken** (prompt que engana as regras), e o que se perde sem a trava.
- Como achar esses modelos no Hugging Face.
- Tabela comparativa: Venice, abliteration.ai, orcarouter (Ollama), OpenRouter, Featherless, RunPod e local com Ollama â€” tipo, modelos, preÃ§o (conferido em 09/11/2026), identidade, privacidade declarada, compatibilidade OpenAI.
- â€œQual escolherâ€ por situaÃ§Ã£o.
- Passo a passo: Venice pela API compatÃ­vel com OpenAI, modelo local com Ollama, e ligar num harness de agente.
- Para onde vÃ£o os seus dados e uso responsÃ¡vel.

Nada aqui foi testado com conta ou chave: os fatos vÃªm das pÃ¡ginas pÃºblicas dos provedores; o que nÃ£o deu para confirmar aparece como â€œnÃ£o confirmadoâ€.

## O processo, do inÃ­cio ao fim

Legenda: ðŸ§  sessÃ£o com o Nei Â· âš™ï¸ script Â· ðŸ¤– `claude -p` / agente

1. ðŸ§  **Pesquisa** das pÃ¡ginas pÃºblicas dos provedores (sÃ³ leitura, sem conta nem API) â†’ `~/projetos/output/provedores-semcensura/PESQUISA.md`, com o que nÃ£o foi confirmado.
2. âš™ï¸ **Capa** do catÃ¡logo + arte crua da hero: `node ~/.claude/skills/capa-inema/assets/gerar-capa.cjs --repo . --title "Provedores de IA sem censura" --cat "IA" --save-raw guia/assets/hero.png --gerador auto` â†’ `capa/capa.png`.
3. âš™ï¸ **Banners** (Codex image_gen pela assinatura), 2 estilos Ã— 3 idiomas: `bash ~/.claude/skills/projetos-landing-guia/assets/gerar-banner.sh --repo . --title "IA SEM CENSURA" --destaque "CENSURA" ...` (`--estilo grade --saida banner-grade`, `--lang en|es --saida banner-en|banner-es`...). Conferir o texto desenhado.
4. ðŸ§  **Guia PT** em `guia/index.html` (skill `projetos-landing-guia`), sÃ³ com fatos da pesquisa.
5. ðŸ¤– **TraduÃ§Ã£o** EN/ES pelo tradutor central: `inema-traduz -o out-en.html < prompt-en.txt` â†’ `guia/en/index.html` e `guia/es/index.html`.
6. ðŸ¤– **RevisÃ£o independente** por outro agente (persona de quem nunca viu o projeto).
7. âš™ï¸ **Publicar**: `git push` â†’ GitHub Actions (`.github/workflows/pages.yml`) publica no Pages; conferir 200 em `/guia/`, `/guia/en/`, `/guia/es/`.
8. ðŸ§  **Atualizar preÃ§os**: refazer o passo 1 e trocar a data â€œconferido emâ€ no guia e nos READMEs.

## Relacionados no INEMA

- [IA privada em 3 nÃ­veis](https://inematds.github.io/ia-privada-3-niveis/guia/)
- [IA sem censura defensiva](https://inematds.github.io/ia-sem-censura-defensiva/guia/)

---

ConteÃºdo aberto do [INEMA.CLUB](https://inema.club). Use com responsabilidade: tirar a trava do modelo nÃ£o tira a lei.

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>