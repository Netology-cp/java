# Модификаторы доступа, наследование

## Памятка к домашнему заданию
Перед тем, как отправить своё решение на проверку преподавателю, сверьтесь с чеклистом

<details>
  <summary> Что делать, если возникли сложности? </summary>
  
  И это здорово! Если их преодолевать правильно, то можно получить большую образовательную пользу для себя. Периодическое возникновение вопросов, недопонимание пройденного материала - нормальная и неотъемлемая часть обучения. А мы здесь, чтобы помочь вам пройти этот путь.
  
  ### Что делать, если непонятна теория?
  1. Если подобный вопрос разбирался на лекции, посмотрите еще раз раздел с этой темой в видеозаписи.
  1. Если вопрос не решился, попробуйте поискать ответ самостоятельно в интернете, этот навык пригодится вам в работе.
  1. Если самостоятельно разобраться не удалось, задайте вопрос в общем чате, мы обязательно поможем.

  ### Что делать, если непонятно условие задания?
  1. Прежде чем задать вопрос по условию задачи, перечитайте его ещё раз и убедитесь, что в тексте условия нет прямого ответа на этот вопрос. Умение работать с текстом - важный навык работы с информацией.
  1. Если ответа на свой вопрос в тексте условия не увидели, задайте его в общем чате, мы раскроем детали условия подробнее. Не забудьте при этом скинуть и ссылку на условие задания, про которую у вас вопрос.

  ### Что делать,если не получается задача?
Если ваша проблема это **ошибка компиляции** (подчёркивает красным, не даёт запустить программу), сборки проекта, CI и прочие подобные ошибки, то:
  1. Найдите и прочитайте текст ошибки, который вам подсвечивает реплит, идея (или логи); "подчёркивает красным" - это не описание ошибки.
  1. Попробуйте понять текст ошибки, при необходимости воспользуйтесь переводчиком. Нестрашно, если вы переведёте неточно, тут главное сам процесс: со временем и с нашей помощью вы будете это делать лучше и лучше, но, пропуская этот этап, вы не сможете научиться это делать.
  1. Если не получилось понять ошибку по её тексту, попробуйте её загуглить и изучить подобную ошибку у других людей. Попробуйте примерить решения их проблем на свой код. Соотнесите найденные описания ошибки с пройденной теорией.
  1. Если все равно вашу трудности не разрешились, напишите в общий чат, обязательно указав:
      1. Название задачи и ссылку на условие
      1. Ссылку на вашу работу
      1. Текст и скриншот (не фотография) ошибки.
      1. Ваши размышления и описание шагов, которые вы совершили для решения.

Если ваша проблема это **ошибка исполнения** (программа умирает уже после запуска) или она **отрабатывает неправильно**, то:
  1. Воспользуйтесь отладчиком для пошагового анализа работы вашей программы. Так вы либо убедитесь в неправильности придуманного вами алгоритма или найдёте конкретное место, где ожидаемое поведение программы разошлось с фактическим.
  1. Если проблему найти не получилось, напишите в общий чат, обязательно указав:
      1. Название задачи и ссылку на условие
      1. Ссылку на вашу работу
      1. Конкретное и подробное описание проблемы или затруднения при решении задачи ("Помогите что не так" - это не описание)
      1. Подробное описание вашего анализа программы с помощью отладчика вместе со скринами
      1. Ваши размышления и описание шагов, которые вы совершили для решения.
  ---
  
</details>

<details>
  <summary> В решении выполнены все требования задания </summary>
  
  Убедитесь, что все требования задания выполнены. Для этого перед отправкой внимательно прочтите весь текст условия задания и соотнесите сказанное в нём с вашим решением. Навык самопроверки работы перед ревью пригодится вам как при обучении, так и на работе.

  ---
  
</details>

<details>
  <summary>Пишем в идее, сдаём в реплите</summary>
  
  Теперь вы знакомы с профессиональным редактором кода - [Intellij IDEA Community Version](https://www.jetbrains.com/idea/download/). Все задачи теперь должны выполняться в нём.
  
  Как минимум перед каждой отправкой работы на проверку (а лучше - вегда) форматируйте код. Ячейки, а именно локальные переменные, параметры, поля и тп должны быть названы камелкейсом с маленькой буквы, а классы и интерфейсы камелкейсом с большой буквы. Правила, связанные с отступами можно доверить самой идее - выберите в меню Code -> Reformat code чтобы отформатировать код в текущем файле.

  При этом задание сдаётся через [реплит](https://replit.com/). Обратите внимание на то, что на реплит ваш код следует добавлять через загрузку файлов, а не через копирование текста; при копировании и вставке кода в окно реплита форматирование может поехать. Тут алгоритм один и тот же: в пустом проекте удаляете `Main.java` (`Delete` в меню действий над файлом) и выбираете в меню что повыше пункт `Upload file` (англ. Загрузить файл) и загружаете `Main.java` с вашего компьютера из папки вашего проекта, после чего нажимаете в том же меню `Upload folder` (англ. Загрузить папку) и загружаете папки-пакеты с .java-файлами если они вам нужны. 
  
![](https://u.netology.ngcdn.ru/backend/uploads/markdown_images/image/30569/image.png)

При любой же проблеме с поведением кода теперь необходимо рассказывать про ваш анализ отладчиком вашей программы.

</details>

## Задача 1 (обязательная)

Вы пишете систему из классов, описывающую банковские счета. Все классы кроме `Main` должны быть в пакете `accounts`.

У каждого счёта есть баланс (`long`) и имя владельца (`String`). У каждого счёта есть две операции: оплатить (`pay(long amount)`) и пополнить (`add(long amount)`); в параметрах передаётся сумму покупки или пополнения соответственно. Каждая операция должна возвращать `boolean` о том, успешно ли она прошла. Никакого вывода на экран нкиакая операция не должна производить.

Также есть три вида счёта: накопительный (`SavingsAccount`), расчётный (`CheckingAccount`) и кредитный (`CreditAccount`).

| Syntax | SavingsAccount | CheckingAccount | CreditAccount |
| --- | ----------- | --- | --- |
| Есть имя | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| Есть баланс | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| Имеет минимальный баланс (нельзя платить, если он станет ниже) | выставляется конструктором | 0 | :x: (баланс может быть отрицательным) |
| Может быть положительным | :white_check_mark: | :white_check_mark: | :x: |

У вас должен быть класс `Account`, который является родителем для всех трёх классов-видов аккаунтов. В нём должно быть два метода (`pay` и `add`). И три класса-наследника, по одному для каждого типа счёта. Подумайте, какие поля они должны будут иметь.

В `Main` продемонстрируйте работу ваших классов (с пользователем общаться необязательно).

### Подсказки

Создайте класс `Account` с двумя методами, общими для всех счетов данными в виде полей и конструктором для заполнения этих полей.

Создайте трёх наследников. У `SavingsAccount` появится ещё один параметр конструктора, которым будет будет задаваться минимальный баланс.
Переопределите в наследниках методы операций над счётом, чья логика отличается между типами счёта.

Не забудьте про инкапсуляцию!


