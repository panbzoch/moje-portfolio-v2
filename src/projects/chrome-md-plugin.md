---
title: "Chrome Plugin: Markdown Generator"
description: "Chytrý extraktor webového obsahu s automatizovaným ukládáním do Obsidianu."
tech: "JavaScript (Manifest V3), Readability.js, Turndown.js, Chrome Downloads API, Windows Junction (mklink)."
order: 1
images: 
  - "/moje-portfolio-v2/images/MDclosed.png"
  - "/moje-portfolio-v2/images/MDopen.png"
---
**Jak to funguje:**

Chytrá extrakce: Pomocí knihovny Readability.js (engine z Firefoxu) analyzuje DOM stránky, identifikuje hlavní článek a odstraňuje balast jako reklamy, postranní panely a menu.

Markdown transformace: Převádí vyčištěné HTML na Markdown pomocí Turndown.js se selektivním odstraněním obrázků pro čistě textový zážitek.

Obsidian integrace: Automaticky generuje YAML Frontmatter (metadata: název, URL, datum, tagy), což umožňuje okamžitou indexaci v Obsidianu.

Plně automatizované workflow: Skrze Background Service Worker a Downloads API odesílá soubory do specifické podsložky obsidian-clip. Ta je díky systémovému propojení (mklink) tunelem přímo do trezoru Obsidianu, kde následně plugin Auto Note Mover zajistí finální zařazení podle tagů.