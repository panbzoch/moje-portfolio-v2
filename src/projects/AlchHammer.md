---
title: "AI Osobní Skladník: Hlasový Asistent"
description: "Inteligentní Telegram bot, který funguje jako externí paměť pro domácí inventář a umožňuje ukládat i vyhledávat předměty pomocí hlasu a přirozeného jazyka."
tech: "Python, Groq API (LLM Llama 3.3-70b & Audio model Whisper Large v3), Telegram Bot API, JSON databáze, GitHub Codespaces."
Order: 5
images: 
  - "/moje-portfolio-v2/images/AlchHammerTXT.png"
  - "/moje-portfolio-v2/images/AlchHammerVOICE.png"
---
**Jak to funguje:**

Aplikace přijímá vstupy přes Telegram ve formě textu nebo hlasových zpráv. Audio je nejprve přepsáno do textu pomocí modelu Whisper s podporou češtiny. Následně vstup zpracovává LLM (Llama 3 přes Groq API), které autonomně detekuje záměr uživatele (Uložení vs. Hledání). Model sám spravuje a strukturuje data v JSON souboru bez nutnosti pevného databázového schématu, řeší synonyma a vrací uživateli kontextuální odpověď v reálném čase.