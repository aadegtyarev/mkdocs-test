Устройства Wiren Board подключаются через интерфейс RS-485 и управляются по протоколу Modbus RTU. Поддерживаются все основные команды чтения и записи одного или нескольких регистров.

При использовании контроллера Wiren Board, модули настраиваются мышкой через его веб-интерфейс. В остальных случаях вам нужно использовать сторонние программы, например, modbus_client или Rilheva Modbus Poll.

?? note "Параметры порта по умолчанию"

    {%
    include-markdown "default-settings.md"
    %}

В актуальной версии прошивки устанавливать параметр Stop bits необязательно — устройство будет работать без ошибок и в случае, когда количество стоповых битов не совпадает с настройками Modbus-мастер.

Для ускорения отклика устройств рекомендуем поднять скорость обмена до 115 200 бит/с, см. Настройка параметров обмена данными