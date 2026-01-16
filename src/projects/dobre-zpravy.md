---
title: "Dobré Zprávy: AI Agregátor"
description: "Plně automatizovaný webový portál, který pomocí umělé inteligence vyhledává, filtruje a publikuje pouze pozitivní zprávy z českého internetu."
tech: "Python, Groq API (model Llama 3.3-70b), GitHub Actions (CI/CD), GitHub Pages, RSS (feedparser), Jinja2, HTML/CSS/JS."
order: 3
---
Systém běží zcela autonomně na serverech GitHubu (zdarma), kde se spouští v pravidelných intervalech (4x denně). Skript nejprve stáhne RSS feedy z českých médií a provede rychlou filtraci klíčových slov (odstraní politiku, krimi a bulvár). Potenciálně zajímavé články následně analyzuje pomocí LLM (Llama 3 přes Groq API), který rozhodne, zda je zpráva skutečně pozitivní. Pokud ano, AI vygeneruje vlastní titulek, shrnutí a určí kategorii (Věda, Byznys, atd.). Data se ukládají do JSON historie, aby se neopakovala, a následně se vygeneruje statická HTML stránka, která se automaticky nasadí na GitHub Pages.
