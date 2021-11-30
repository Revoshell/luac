# luac
This repository contains compiled versions of scripts for the RDS server

RUS:

RDS UCAR (Актуальная версия 1.6)
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
- Параметр "render" отвечает за работу рендера по умолчанию. Функция отображает задержку скрипта в реальном времени.
Если ввести "render=false" или "render=0", то рендер не будет отображаться надпись на экране. Если же ввести "render=true" или "render=1", то рендер будет отображаться на экране.

ОБРАТИТЕ ВНИМАНИЕ! ВАЖНО!
- Для работы скрипта необходима библиотека SAMP.Lua (модуль SAMP.Events). Скачать можно либо по ссылке: blast.hk/threads/14624, либо из репозитория разработчика: github.com/THE-FYP/SAMP.Lua
- Если скрипт перестал работать, вы можете перезагрузить все ваши скрипты скриптом, который идёт в комплекте с moonloader (нажав клавиши ctrl+r).


ENG:

RDS UCAR (Current version 1.6)
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
- The "render" parameter is responsible for the default rendering. The function displays the script delay in real time.
If you enter "render=false" or "render=0", then the render will be displayed on the screen. If you enter "render=true" or "render=1", then the render will be displayed on the screen.

NOTE! IMPORTANT!
- For the script to work, the SAMP.Lua library (SAMP.Events module) is required. You can download it either from the link: blast.hk/threads/14624, or from the developer's repository: github.com/THE-FYP/SAMP.Lua
- If the script stops working, you can reload all your scripts with the script that comes with moonloader (by pressing ctrl+r).

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

RUS:

RDS XCAR (Актуальная версия 2.8)
Сервер СА-МП: РДС (176.32.36.131:7777)
1. Скрипт предназначен для восстановления ранней позиции автомобиля.
- При нажатии на клавишу активации: X (по умолчанию) происходит телепортация на позицию, которая была ранее, но без перебора во временных рамках.
Этого достаточно, чтобы объехать препятствие. Для целесообразности и защиты от использования во вред установлено ограничение на использование размером в 7 секунд.
- У скрипта присутствует рендер текущего состояния скрипта. По команде /xc или /xcount он активируется. По этой же команде происходит деактивация.
- Выставлена проверка на локацию. Помимо обычного мира - нигде нельзя использовать этот скрипт.
- Скрипт создаёт и использует файл конфигурации по пути: Корневая папка игры\moonloader\config\XCAR.ini
Параметры:
- "key" отвечает за установку клавиши по умолчанию. Можно использовать одну из клавиш, которые указаны ниже.
(x, r, q, e, g, z, b, n, ctrl(control), shift, space, default(Клавиша по умолчиню, т.е. "x")
- "messages" отвечает за отображение сообщений скрипта. Если в параметр введено "1" или "true", то сообщения будут отображаться. Если ввести "0" или "false", то сообщения отображаться не будут.
- "count" отвечает за активацию рендера по умолчанию. При входе в игру вам не нужно будет вписывать каждый раз /xc или /xcount, чтобы рендер появился.
Если ввести "1" или "true", то по умолчанию рендер будет отображаться. Если ввести "0" или "false", то по умолчанию рендер не будет отображаться.

Для того, чтобы не ходить сюда за информацией, в скрипте предусмотрено диалоговое окно с информацией. Активация по команде /xcar.

ОБРАТИТЕ ВНИМАНИЕ! ВАЖНО!
- Для работы скрипта необходима библиотека SAMP.Lua (модуль SAMP.Events). Скачать можно либо по ссылке: blast.hk/threads/14624, либо из репозитория разработчика: github.com/THE-FYP/SAMP.Lua
- Если скрипт перестал работать, вы можете перезагрузить все ваши скрипты скриптом, который идёт в комплекте с moonloader (нажав клавиши ctrl+r).

ENG:

RDS XCAR (Current version 2.8)
SA-MP server: RDS (176.32.36.131:7777)
1. The script is designed to restore the early position of the car.
- When you press the activation key: X (by default), teleportation occurs to the position that was previously, but without busting in the time frame.
This is enough to get around the obstacle. For expediency and protection against harmful use, a limit of 7 seconds is set.
- The script has a render of the current state of the script. By command /xc or /xcount it is activated. Deactivation occurs on the same command.
- Checked on the location. Apart from the usual world, this script cannot be used anywhere.
- The script creates and uses a configuration file along the path: Root folder of the game\moonloader\config\XCAR.ini
Options:
- "key" is responsible for setting the default key. You can use one of the keys below.
(x, r, q, e, g, z, b, n, ctrl(control), shift, space, default(Default key, ie "x")
- "messages" is responsible for displaying script messages. If "1" or "true" is entered in the parameter, the messages will be displayed. If you enter "0" or "false", no messages will be displayed.
- "count" is responsible for activating the default render. When entering the game, you will not need to enter /xc or /xcount every time for the render to appear.
If you enter "1" or "true", then by default the render will be displayed. If you enter "0" or "false", then by default the render will not be displayed.

In order not to go here for information, the script provides a dialog box with information. Activation by command /xcar.

NOTE! IMPORTANT!
- For the script to work, the SAMP.Lua library (SAMP.Events module) is required. You can download it either from the link: blast.hk/threads/14624, or from the developer's repository: github.com/THE-FYP/SAMP.Lua
- If the script stops working, you can reload all your scripts with the script that comes with moonloader (by pressing ctrl+r).

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
