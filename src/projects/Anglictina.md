---
title: "Angličtina s Kapybarou"
description: "Interaktivní webová aplikace pro výuku anglické slovní zásoby, kde dítě provází kreslená kapybara Kapinka"
tech: "HTML, CSS, JavaScript (vanilla), GitHub API (synchronizace slovíček), Python http.server (lokální vývoj), GitHub Pages / Netlify (hosting)"
order: 1
link: "https://anglictina-alpha.vercel.app/"
---
Aplikace při každém spuštění náhodně vybere 10 slovíček z editovatelného poolu a zadává je v češtině. Uživatel vybírá správný anglický překlad kliknutím na jednu ze čtyř nabízených možností. Po každé odpovědi dostane okamžitou zpětnou vazbu — při chybě se zvýrazní správná odpověď. U každé otázky se zobrazí náhodný obrázek kapybary. Po dokončení kola se zobrazí finální skóre a kapybara vyjádří svůj názor: šťastná při dobrém výsledku, smutná při špatném. Slovíčka spravuje admin přes heslem chráněný panel, kde může přidávat, upravovat a mazat záznamy. Změny se přes GitHub API uloží do sdíleného souboru words.json, takže jsou okamžitě dostupné na všech zařízeních — admin edituje na počítači, dítě procvičuje na tabletu.
