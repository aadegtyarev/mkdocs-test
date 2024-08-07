# ПО Wiren Board

## Как устроено
Wiren Board работает под управлением Debian Linux. Для архитектуры используемого процессора есть официальный порт, поэтому любое стандартное Linux-приложение можно установить из репозитория одной командой apt install имя_пакета.

Все сервисы контроллера общаются между собой по общей «шине», в роли которой выступает очередь сообщений MQTT.

По умолчанию установлены веб-интерфейс Wiren Board, движок правил wb-rules, а также драйвера и вспомогательные утилиты.

Опционально можно установить шлюзы для интеграции со SCADA-системами и сторонний софт.

## Установка

ПО устанавливается на заводе на автоматизированном стенде во время производства партии контроллеров.

Конечному пользователю не требуется предпринимать никаких действий для установки ПО, все взаимодействие происходит через пользовательский интерфейс.

## Стоимость

Программное обеспечение поставляется бесплатно вместе с контроллерами Wiren Board.

## Основные компоненты ПО

- [wb-mqtt-serial](wb-mqtt-serial/index.md) — драйвер опроса устройств, подключённых к последовательным портам контроллера.
- [wb-mqtt-homeui](wb-mqtt-homeui/index.md) — веб-интерфейс контролллера.
- [wb-rules](wb-rules/index.md) — движок правил для автоматизации.
