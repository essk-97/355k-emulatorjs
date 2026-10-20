# 355k-emulatorjs

O [EmulatorJS](https://github.com/EmulatorJS/EmulatorJS) **4.2.3** como é usado no [355k](https://355k.essk.space): a pasta `data` da versão oficial, em `emulatorjs/`.

Licença: **GPL-3.0** (ver `LICENSE`). Os núcleos têm as licenças próprias (abaixo); o texto de cada uma vai dentro do pacote do núcleo.

## Sem modificações

Todos os arquivos são os da versão 4.2.3, sem alteração: foram conferidos um a um (SHA-1) com `https://cdn.emulatorjs.org/4.2.3/data/`. O código-fonte é o do repositório oficial, na tag [v4.2.3](https://github.com/EmulatorJS/EmulatorJS/tree/v4.2.3).

A única diferença é o que **não** está aqui: o núcleo **snes9x** (Super Nintendo), porque a licença dele proíbe uso comercial. No 355k, o Super Nintendo usa o Mesen-S, do repositório [355k-mesen-s](https://github.com/essk-97/355k-mesen-s).

## Núcleos incluídos

Os que vêm no EmulatorJS 4.2.3, sem modificação, cada um em duas variantes (WebGL2 e `-legacy`, WebGL1):

| Console | Núcleo | Licença | Código |
|---|---|---|---|
| Game Boy Advance | mGBA (`mgba`) | MPL-2.0 | [EmulatorJS/mgba](https://github.com/EmulatorJS/mgba) |
| Nintendo DS | melonDS (`melonds`) | GPL-3.0 | [EmulatorJS/melonDS](https://github.com/EmulatorJS/melonDS) |
| PlayStation | PCSX ReARMed (`pcsx_rearmed`) | GPL-2.0 | [EmulatorJS/pcsx_rearmed](https://github.com/EmulatorJS/pcsx_rearmed) |

Todos levam o RetroArch adaptado do EmulatorJS ([EmulatorJS/RetroArch](https://github.com/EmulatorJS/RetroArch), GPL-3.0).

O EmulatorJS também traz [nipplejs](https://github.com/yoannmoinet/nipplejs) (MIT), um extrator de .7z (p7zip, LGPL-2.1) e o [libunrar-js](https://github.com/tnikolai2/libunrar-js) (licença unRAR).

## Como o 355k usa

Esta pasta fica em `emulatorjs/`, ao lado da [ponte](https://github.com/essk-97/355k-ponte), com o Mesen-S em `emulatorjs/cores/`. O 355k só conversa com a ponte por mensagens.
