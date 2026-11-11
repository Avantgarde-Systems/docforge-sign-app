# DocForge sign app

A static Telegram Mini App: a drawing pad for the signature in Sign Forge (DocForge Telegram bots).
It has no backend and stores nothing. The strokes are simplified and sent to the bot with
`Telegram.WebApp.sendData` (a JSON of at most 4096 bytes: `{"v":1,"w":600,"h":240,"s":[[x,y,x,y,…],…]}`);
the bot validates and renders them.

Served by GitHub Pages from the `main` branch root.
