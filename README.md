# luac
This repository contains compiled versions of scripts for the RDS server

RDS UCAR
Сервер СА-МП: РДС (176.32.36.131:7777)
1. Скрипт предназначен для минимизирования помех.
- По нажатию на клавишу активации: B (по умолчанию) включается часть кода скрипта, которая отправляет ложную синхронизацию по координате Z (data.position.z = -90).
В следствие чего для остальных игроков вы находитесь под землёй, но локально у вас ничего не меняется. В момент отправки и до момента автоматической деактивации
у вас отключается коллизия на все авто, поэтому вы можете ехать и не волноваться, что вас толкнут. А поскольку отправляется ложная синхронизация, вы сами никого не толкаете,
ведь для других игроков вы просто парите глубоко под текстурами.
- Выставлена проверка на локацию. Помимо обычного мира - нигде нельзя использовать этот скрипт.
- При активации присутствует ограничение в использовании и активация длится 3 секунды.
2. У скрипта есть файл конфигурации .ini по пути: Корневая папка игры\moonloader\config\UCAR.ini
- В файле конфигурации есть параметры.
- Параметр "key" отвечает за установку клавиши активации по умолчанию.
Доступные клавиши для использования: shift, space, default, x, r, q, e, g, z, b, n, ctrl(control).
- Параметр "messages" отвечает за отображение сообщений скрипта по умолчанию.
Если ввести "messages=false" или "messages=0", то сообщения скрипта отправляться не будут. Если же ввести "messages=true" или "messages=1", то сообщения будут отправляться.

ОБРАТИТЕ ВНИМАНИЕ! ВАЖНО!
- Для работы скрипта необходима библиотека SAMP.Lua (модуль SAMP.Events). Скачать можно либо по ссылке: blast.hk/threads/14624, либо из репозитория разработчика: github.com/THE-FYP/SAMP.Lua
- Если скрипт перестал работать, вы можете перезагрузить все ваши скрипты скриптом, который идёт в комплекте с moonloader (нажав клавиши ctrl+r).

RDS UCAR
Server SA-MP: RDS (176.32.36.131:7777)
1. The script is designed to minimize interference.
- By pressing the activation key: B (by default), a part of the script code is included that sends a false synchronization at the Z coordinate (data.position.z = -90).
As a result, for the rest of the players you are underground, but locally nothing changes for you. At the time of sending and until the moment of automatic deactivation
collision is disabled for all cars, so you can drive and not worry that you will be pushed. And since a false sync is being sent, you yourself are not pushing anyone,
because for other players you just hover deep under the textures.
- Checked on the location. Apart from the usual world, this script cannot be used anywhere.
- When activated, there is a limitation in use and activation lasts 3 seconds.
2. The script has a configuration file .ini along the path: Root folder of the game\moonloader\config\UCAR.ini
- There are parameters in the config file.
- The "key" parameter is responsible for setting the default activation key.
Available keys for use: shift, space, default, x, r, q, e, g, z, b, n, ctrl(control).
- The "messages" parameter is responsible for displaying the messages of the script by default.
If you enter "messages=false" or "messages=0", the script messages will not be sent. If you enter "messages=true" or "messages=1", then messages will be sent.

NOTE! IMPORTANT!
- For the script to work, the SAMP.Lua library (SAMP.Events module) is required. You can download it either from the link: blast.hk/threads/14624, or from the developer's repository: github.com/THE-FYP/SAMP.Lua
- If the script stops working, you can reload all your scripts with the script that comes with moonloader (by pressing ctrl + r).
