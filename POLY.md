# Полиморфизм

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

:warning: Эта задача является продолжением [предыдущей задачи](./INH.md), поэтому для выполнения этой лучше сперва получить зачёт по предыдущей.

Вы продолжаете работать с системой банковских счетов. Теперь вам предстоит разработать класс клиента банка `Client`. Его нужно создать в пакете `clients`.

Клиент должен обладать следующей функциональностью:
1. Иметь имя
1. При создании клиента помимо имени указывается максимальное количество счетов, которое он может завести
1. Метод добавления нового счёта (приходит параметром); если превышено максимальное количество счетов, то должно выводиться сообщение об этом пользователю
1. Метод `boolean pay(int amount)`, который ищет счёт, с которого можно будет заплатить переданную параметром сумму и, если находит, платит с этого счёта и возвращает `true`. Если нет, то возврашает `false`.

Продемонстрируйте работу созданного класса в `main`.

### Подсказки

Хранить все счета клиент может в виде набора в поле, а именно в виде массива `Account[] accounts`.
В конструкторе же мы можем сразу создать массив размером в переданное максимальное количество счетов, тогда нам точно хватит ячеек для добавления счетов вплоть до этого количества.

При добавлении нового счёта, мы можем пробегаться по массиву счетов в поиске первой пустой ячейки (`null`) и класть туда добавляемый счёт:
```java
public void add(Account account) {
    for (int i = 0; i < accounts.length; i++) {
        if (в accounts[i] лежит null) {
            accounts[i] = account;
            return;
        }
    }
    
    // если дошли сюда, значит не нашлось свободной ячейки, иначе бы уже ушли из for
    System.out.println("Мест для добавления нового счёта нет! :(");
}
```

При реализации метода `pay`, просто пробегитесь по массиву и по-порядку у каждого вызывайте метод `pay`.
Если вызов вернул `true`, то операция удалась и можно выходить из метода, вернув `true`.
Если же все счета перебраны и ни один не вернул `true`, возвращайте `false`.
