---
title: "AI Textová Adventura: Interaktivní RPG Bot"
description: "Inteligentní Telegram bot, který simuluje textovou RPG hru a procedurálně generuje dynamický herní svět s vlastním vizuálem a logickými pravidly."
tech: "Python, Groq API (LLM Llama 3.3-70b & Audio model Whisper), Fireworks API (Image model Flux.1 [schnell]), Telegram Bot API, JSON databáze, Railway cloud, GitHub."
Order: 6
images: 
  - "/moje-portfolio-v2/images/Adventura1.png"
  - "/moje-portfolio-v2/images/Adventura2.png"
---
**Jak to funguje:**

Aplikace přijímá vstupy přes Telegram ve formě textu nebo hlasových zpráv. Audio je nejprve přepsáno do textu pomocí modelu Whisper. Následně vstup zpracovává LLM (Llama 3 přes Groq API), které využívá techniku Chain of Thought pro interní vyhodnocení logiky hráčových akcí před samotným vygenerováním odpovědi. Model autonomně spravuje inventář, sleduje postup k cíli hry, pomocí integrace hodů virtuální kostkou vyhodnocuje souboje a algoritmicky vyvozuje důsledky z hráčových rozhodnutí. Vizuální kontext zajišťuje model Flux (přes Fireworks API), pro který LLM na pozadí automaticky generuje optimalizované anglické prompty a vytváří tak 16-bitové pixel art obrázky aktuálních lokací. Stav rozehrané hry je ukládán do stavové JSON databáze, která je pro zajištění nepřetržitého běhu napojena na perzistentní virtuální disk v cloudovém prostředí.