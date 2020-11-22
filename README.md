
# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

Начало тестирования 18.11.2020 - 19.11.2020 
Было проведено функциональное тестирование (метод черного ящика) поля ввода номера карты приложения Credit Card Number Validator.

На тестирование затрачено: 3 часа

В результате тестирования выявлены следующие дефекты:

[Баг-репорт №1 (Ввод валидных значений в поле ввода номера карт) приложения Credit Card Number Validator](https://github.com/evgen-911/projekt-1/issues/1)



## Описание процесса тестирования

Тест №1 - Ввод 16-значного номерка карты "0000000000000000"

Ожидаемый результат - "Result is FAIL"

Фактический результат - "Result is FAIL"

Скриншот:

https://skr.sh/s5DKHoICY7w

Тест №2 - Ввод 15-значного номера карты "491644320019496"

Ожидаемый результат - ""Result is FAIL""

Фактический результат - "Result is FAIL"

Скриншот:

https://skr.sh/s5DTQAbAU0g

Тест №3 - Ввод 16-значного валидного номера карты "4916443200194964"

Ожидаемый результат - "Result is OK"

Фактический результат - "Result is OK"

Скриншоты:

https://skr.sh/s5Dn3ZN3FdL

https://skr.sh/s5D7sihwiws

Тест №4 - Ввод 17-значного номера карты "49164432001949655"

Ожидаемый результат - ""Result is FAIL""

Фактический результат - "Result is FAIL"

Скриншот

https://skr.sh/s5DGmdjb4L0

Ссылка на коммит https://github.com/evgen-911/projekt-1/commit/295f7d141bd185a5ece4f9ca6a84ab4e0ba1300b

Тест №5 - Ввод одного значения "1"

Ожидаемый результат - ""Result is FAIL""

Фактический результат - "Result is FAIL"

Скриншот

https://skr.sh/s5DIeCPiJkP

Ссылка на коммит https://github.com/evgen-911/projekt-1/commit/2a9ccf7e74ce22ffd4e16e08b92eba7c1180259b

Тест №6 - Ввод 19-значного валидного номера карты "4539222137126900518"

Ожидаемый результат - "Result is OK"

Фактический результат - "Result is FAIL"

Скриншоты:

https://skr.sh/s5DW4wxqZFp

https://skr.sh/s5DO2Hh930f


Тест №7 - Оставляем поле пустым

Ожидаемый результат - ""Result is FAIL""

Фактический результат - "Result is FAIL"

Скриншот

https://skr.sh/s5DxW2oDORr

Тест №8 - Ввод 16 значений на латинице "QWERTYUIOPASDFGH"

Ожидаемый результат - ""Result is FAIL""

Фактический результат - "Result is FAIL"

Скриншот

https://skr.sh/s5DZIyd647v


В качестве тестовых данных использовались номера карт из веб-сайта https://www.freeformatter.com/credit-card-number-generator-validator.html:

Тестирование производилось в следующем окружении:

Windows 10 Pro x64

java version "11.0.9" 2020-10-20 LTS

Google Crome Версия 86.0.4240.198 (Официальная сборка), (64 бит),

IntelliJ IDEA 2020.2.3 (Community Edition)
