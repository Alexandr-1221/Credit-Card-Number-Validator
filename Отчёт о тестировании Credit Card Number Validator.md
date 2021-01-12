# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

12.01.2021 - 12.01.2021 было проведено функциональное тестирование приложения Credit Card Number Validator.

На тестирование затрачено: 1 час

В результате тестирования выявлены следующие дефекты:
 
* https://github.com/Alexandr-1221/Credit-Card-Number-Validator/issues/1
* https://github.com/Alexandr-1221/Credit-Card-Number-Validator/issues/2

# Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:

* [Требования](https://github.com/netology-code/javaqa-homeworks/tree/master/intro#%D0%B7%D0%B0%D0%B4%D0%B0%D1%87%D0%B0-2---credit-card-number-validator)

В качестве тестовых данных использовались [сгенерированные валидные номера карт](https://www.freeformatter.com/credit-card-number-generator-validator.html#validate), а также невалидные номера, составленные самостоятельно:

* **4485954762737918 (VISA)** *- ответ приложения:* `Result is OK`
* **5493931760755867 (MasterCard)** *- ответ приложения:* `Result is OK`
* **5018206849055621 (Maestro)** *- ответ приложения:* `Result is OK`
* **6011629884835729 (Discover)** *- ответ приложения:* `Result is OK`
* **377171954623389 (AMEX)** *- ответ приложения:* `Result is OK`
* **4532353443630807561 (Visa)** *- ответ приложения:* `Result is OK`
* **0000000000000000** *- ответ приложения:* `Result is FAIL`
* **0485954762737918** *- ответ приложения:* `Result is FAIL`
* **4485954762737910** *- ответ приложения:* `Result is FAIL`
* **asdfghjklzxcvbnm** *- ответ приложения:* `Result is FAIL`
* **!@#$%^&*()_+!@#$** *- ответ приложения:* `Result is FAIL`
* ** 4485954762737918** *- ответ приложения:* `Result is FAIL`
 
Тестирование производилось в следующем окружении:

* Windows 10 (64-разрядная)
* Java "11.0.9.1" 2020-11-04
* InteliJ IDEA Community Edition 2020 (64)

