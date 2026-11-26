ï»¿# provedores-semcensura

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


[![IA sem censura: onde usar, quanto custa e o que conferir](guia/assets/banner.jpg)](https://linnoff88-dev.github.io/arckhe-/guia/)

**ê°Å¸â¡Â§ê°Å¸â¡Â· [PortuguêÂªs](README.md) êÂ· ê°Å¸â¡Âºê°Å¸â¡Â¸ [English](README.en.md) êÂ· ê°Å¸â¡Âªê°Å¸â¡Â¸ [EspaêÂ±ol](README.es.md)**

## O que êÂ©

Este guia mostra onde encontrar modelos de IA ê¢â¬Åsem censuraê¢â¬Â, ou seja, versêÂµes que nêÂ£o recusam pedidos. Serve para quem testa a seguranêÂ§a do prêÂ³prio sistema, pesquisa ou sêÂ³ quer um assistente que nêÂ£o trave em assunto delicado. VocêÂª vêÂª numa tabela os provedores por API, por chat, por GPU alugada e no seu prêÂ³prio computador, com preêÂ§o, privacidade declarada e se pedem identidade. Para usar, basta ler; os exemplos pedem uma conta no provedor escolhido ou o Ollama instalado.

## ê°Å¸ââ Guia de uso

Guia completo (landing + passo a passo): **https://linnoff88-dev.github.io/arckhe-/guia/**

## O que tem no guia

- DiferenêÂ§a entre **uncensored** (fine-tune, tipo Dolphin), **abliterated** (remove a ê¢â¬ÅdireêÂ§êÂ£o de recusaê¢â¬Â dos pesos, sem treinar) e **jailbroken** (prompt que engana as regras), e o que se perde sem a trava.
- Como achar esses modelos no Hugging Face.
- Tabela comparativa: Venice, abliteration.ai, orcarouter (Ollama), OpenRouter, Featherless, RunPod e local com Ollama ê¢â¬â tipo, modelos, preêÂ§o (conferido em 09/11/2026), identidade, privacidade declarada, compatibilidade OpenAI.
- ê¢â¬ÅQual escolherê¢â¬Â por situaêÂ§êÂ£o.
- Passo a passo: Venice pela API compatêÂ­vel com OpenAI, modelo local com Ollama, e ligar num harness de agente.
- Para onde vêÂ£o os seus dados e uso responsêÂ¡vel.

Nada aqui foi testado com conta ou chave: os fatos vêÂªm das pêÂ¡ginas pêÂºblicas dos provedores; o que nêÂ£o deu para confirmar aparece como ê¢â¬ÅnêÂ£o confirmadoê¢â¬Â.

## O processo, do inêÂ­cio ao fim

Legenda: ê°Å¸Â§Â  sessêÂ£o com o Nei êÂ· ê¢Å¡â¢ê¯Â¸Â script êÂ· ê°Å¸Â¤â `claude -p` / agente

1. ê°Å¸Â§Â  **Pesquisa** das pêÂ¡ginas pêÂºblicas dos provedores (sêÂ³ leitura, sem conta nem API) ê¢â â `~/projetos/output/provedores-semcensura/PESQUISA.md`, com o que nêÂ£o foi confirmado.
2. ê¢Å¡â¢ê¯Â¸Â **Capa** do catêÂ¡logo + arte crua da hero: `node ~/.claude/skills/capa-ARCKHÉ/assets/gerar-capa.cjs --repo . --title "Provedores de IA sem censura" --cat "IA" --save-raw guia/assets/hero.png --gerador auto` ê¢â â `capa/capa.png`.
3. ê¢Å¡â¢ê¯Â¸Â **Banners** (Codex image_gen pela assinatura), 2 estilos êâ 3 idiomas: `bash ~/.claude/skills/projetos-landing-guia/assets/gerar-banner.sh --repo . --title "IA SEM CENSURA" --destaque "CENSURA" ...` (`--estilo grade --saida banner-grade`, `--lang en|es --saida banner-en|banner-es`...). Conferir o texto desenhado.
4. ê°Å¸Â§Â  **Guia PT** em `guia/index.html` (skill `projetos-landing-guia`), sêÂ³ com fatos da pesquisa.
5. ê°Å¸Â¤â **TraduêÂ§êÂ£o** EN/ES pelo tradutor central: `ARCKHÉ-traduz -o out-en.html < prompt-en.txt` ê¢â â `guia/en/index.html` e `guia/es/index.html`.
6. ê°Å¸Â¤â **RevisêÂ£o independente** por outro agente (persona de quem nunca viu o projeto).
7. ê¢Å¡â¢ê¯Â¸Â **Publicar**: `git push` ê¢â â GitHub Actions (`.github/workflows/pages.yml`) publica no Pages; conferir 200 em `/guia/`, `/guia/en/`, `/guia/es/`.
8. ê°Å¸Â§Â  **Atualizar preêÂ§os**: refazer o passo 1 e trocar a data ê¢â¬Åconferido emê¢â¬Â no guia e nos READMEs.

## Relacionados no ARCKHÉ

- [IA privada em 3 nêÂ­veis](https://linnoff88-dev.github.io/arckhe-/guia/)
- [IA sem censura defensiva](https://linnoff88-dev.github.io/arckhe-/guia/)

---

ConteêÂºdo aberto do [ARCKHÉ AI](https://ARCKHÉ AI). Use com responsabilidade: tirar a trava do modelo nêÂ£o tira a lei.

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>