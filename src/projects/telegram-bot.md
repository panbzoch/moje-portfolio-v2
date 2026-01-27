---
title: "Pork Hunter Agent"
description: "Automatizovaný cloudový hlídač slev masa na Kupi.cz"
tech: "Python, GitHub Actions (CRON), Telegram API, JSON parsing"
order: 2
image: "/moje-portfolio-v2/images/PorkHunter.jpg"
---
Agent se spouští automaticky každý den ráno v cloudu (GitHub Actions). Místo nespolehlivého čtení HTML kódu extrahuje přímo skrytá strukturovaná data (JSON-LD) ze stránek Kupi.cz. Porovnává ceny specifického produktu (vepřová pečeně) s nastaveným limitem (130 Kč), inteligentně filtruje duplicity z různých regionů a v případě shody odesílá formátovanou notifikaci s obchodem, cenou a datem konce akce na Telegram.
