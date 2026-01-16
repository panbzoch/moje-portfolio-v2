---
title: "Portfolio Projektů"
description: "Moderní statický web pro prezentaci projektů s CI/CD pipeline."
tech: "Astro, Markdown, GitHub Actions, StackBlitz"
order: 4
---
Tento web sám o sobě je technickým projektem. Cílem bylo vytvořit bleskurychlé, bezúdržbové řešení, kde je obsah striktně oddělen od kódu.

**Jak to funguje:**
* **Jádro:** Web běží na frameworku **Astro**, který generuje čisté statické HTML (žádný zbytečný JavaScript v prohlížeči).
* **Obsah:** Projekty se píší jako jednoduché **Markdown** soubory. Přidání nového projektu nevyžaduje zásah do HTML kódu.
* **Vývoj:** Celý proces tvorby probíhá v cloudu přes **StackBlitz**, což eliminuje nutnost lokálního vývojového prostředí.
* **Automatizace:** Po uložení změny (commit) se spustí skript v **GitHub Actions**, který web automaticky sestaví a publikuje na GitHub Pages.