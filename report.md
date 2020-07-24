# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

24.07.2020 было проведено тестирование приложения Credit Card Number Validator.

На тестирование затрачено: 0,5 часа

В результате тестирования выявлены следующие дефекты:
* Номер кредитной карты 343199629337102 (AMEX) - fail - невалиден (должен быть валидным)
* Номер кредитной карты 36436945468415 Diners Club - International - fail - невалиден (должен быть валидным)

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* [Руководство по установке IntelliJ IDEA](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/idea.md)

В качестве тестовых данных использовались данные [Credit Card Number Generator & Validator](https://www.freeformatter.com/credit-card-number-generator-validator.html#validate):

### Валидные номера кредитных карт:

* 343199629337102 AMEX
* 5122530189076753 MasterCard
* 4024007116985457 VISA
* 3529993378517280 JCB
* 4508264873759287 Visa Electron
* 6762739346466004 Maestro
* 36436945468415 Diners Club - International
* 6370859150836615 InstaPayment

### Невалидные номера кредитных карт:

* 4024007116985450
* 6011509070137729
* 343199629337103
* 6392782076756968
* 222222222222222

### Тестирование производилось в следующем окружении:
* Windows 8.1 Professional x64
* Openjdk version "11.0.8" 2020-07-14
* OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.8+10)
* OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.8+10, mixed mode)