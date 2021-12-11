# luac
This repository contains compiled versions of scripts for the RDS server

RDS UCAR (Актуальная версия 1.8)
Сервер СА-МП: РДС (176.32.36.131:7777)
1. Скрипт предназначен для минимизирования помех.
- По нажатию на клавишу активации: B (по умолчанию) включается часть кода скрипта, которая отправляет ложную синхронизацию по координате Z (data.position.z = -70).
В следствие чего для остальных игроков вы находитесь под землёй, но локально у вас ничего не меняется. В момент отправки и до момента автоматической деактивации
у вас отключается коллизия на все авто, поэтому вы можете ехать и не волноваться, что вас толкнут. А поскольку отправляется ложная синхронизация, вы сами никого не толкаете,
ведь для других игроков вы просто парите глубоко под текстурами.
- Выставлена проверка на локацию. Помимо обычного мира - нигде нельзя использовать этот скрипт.
- При активации присутствует ограничение в использовании и активность длится 5 секунд.
2. У скрипта есть файл конфигурации .ini по пути: Корневая папка игры\moonloader\config\UCAR.ini
- В файле конфигурации есть параметры.
- Параметр "key" отвечает за установку клавиши активации по умолчанию.
Доступные клавиши для использования: shift, space, default, x, r, q, e, g, z, b, n, ctrl(control).
- Параметр "messages" отвечает за отображение сообщений скрипта по умолчанию.
Если ввести "messages=false" или "messages=0", то сообщения скрипта отправляться не будут. Если же ввести "messages=true" или "messages=1", то сообщения будут отправляться.
- Параметр "render" отвечает за работу рендера по умолчанию. Функция отображает задержку скрипта в реальном времени.
Если ввести "render=false" или "render=0", то рендер не будет отображать надпись на экране. Если же ввести "render=true" или "render=1", то рендер будет отображаться на экране.
- Параметр "flicker" отвечает за мерцание авто при использовании основной функции скрипта. (Можно использовать как замену "render" и "messages", либо использовать всё вместе, как вам угодно!)
Если ввести "flicker=false" или "flicker=0", то при использовании скрипта машина мерцать не будет. Если же ввести "flicker=true" или "flicker=1", то при использовании скрипта ваша машина будет мерцать, таким образом давая вам понять, что скрипт работает и активен. (Ну и для красоты:))
- Параметр "flickerMode" неразрывно связан с параметром выше. Данный параметр предоставляет возможность пользователю выбрать определённый пресет мерцания авто.
Если ввести "0", то ваше авто авто будет резко становиться прозрачным на время активации скрипта.
Если ввести "1" (по умолчанию 1), ваше авто будет мерцать мягко и плавно, не исчезая до конца. Второй параметр "2" это тот, который был в более ранней версии, но стал совсем чуточку быстрее. Третий параметр "3" это тот же самый параметр "2", но в нём используются другие интервалы. Т.е. при активации ваша машина резко моргает, после чего на протяжение секунды не моргает, и снова по тому же сценарию.
- Параметр "detector" отвечает за работу отслеживания других игроков, кто использует UCAR. Если скрипт находит в зоне стрима того, кто использует UCAR в чат будет отправлено сообщение о том, что определённый игрок использует данный скрипт.
Если ввести "detector=false" или "detector=0", то скрипт не будет отслеживать других игроков и предупреждать вас в чате о том, что кто-то использует схожий скрипт. Если же ввести "detector=true" или "detector=1", то другие игроки будут отслеживаться на предмет использования схожего скрипта.
- Во избежание проблем с зоной стрима и объектами поставленными сервером: была добавлена проверка на то, что игрок не находится в воздухе. Поскольку отправляется ложная синхронизация вниз под карту, сервер думает, как и остальные игроки, что вы находитесь под землёй, соответственно объекты из зоны стрима могут пропасть, если вы находитесь слишком далеко от них (например высоко).
- Добавлена проверка на файл конфигурации. Если найден старый файл, то скрипт заново создаст файл конфигурации но теперь уже с актуальными параметрами, после чего автоматически перезагрузит все скрипты.

ОБРАТИТЕ ВНИМАНИЕ! ВАЖНО!
Установка:
- Скачать архив UCAR.7z из этого репозитория и извлечь папку из него в корень игры. Если появляется уведомление о замене файлов: смело соглашаемся на замену. Это нужно для того, чтобы вы сами не искали пути для файлов библиотек и не тратили своё драгоценное время.
- Так же вместе с архивом идёт текстовый файл с информацией, которая предоставлена здесь, чтобы вы могли найти её у себя локально.
- Если скрипт перестал работать, вы можете перезагрузить все ваши скрипты скриптом, который идёт в комплекте с moonloader (так же имеется в UCAR.7z) (нажав клавиши ctrl+r).

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

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

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
