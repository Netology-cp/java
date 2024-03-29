# Структура программы

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
  <summary>Задание сдаём в реплите </summary>
  
  Это задание сдаётся через [реплит](https://replit.com/). Если вы ещё не зарегистрированы на этом сайте - зарегистрируйтесь.
  После чего создайте новый проект, выполните в нём задание и отправьте ссылку на редактируемый вами реплит на проверку.
  Каждую задачу следует делать в своём реплите если об этом не оговорено в условии самой задачи.
</details>

## Задача 1 (обязательная)
Напишите программу для рассчёта ежемесячного платежа по беспроцентной рассрочке. 

Для этого создайте статический метод, который принимал бы три параметра:
* первоначальный взнос `start`;
* общую сумму покупки `amount` (в неё входит и первоначальный взнос);
* количество лет, на которое дана рассрочка `years`.

Метод должен рассчитывать ежемесячный платёж и отдавать его в качестве возвращаемого значения; сам выводить на экран этот вспомогательный метод расчёта ничего не должен, выводом должен заниматься метод `main`.

Продемонстрируйте работу этого метода в `main`. Например, для суммы `2600000` со взносом `200000` и сроком `2` года ежемесячный платёж будет `100000` рублей.

### Подказки
  * Для получения количества месяцев умножьте переданное количество лет на 12.
  * Для получения ежемесячного платежа вычтите из суммы покупки первоначальный взнос и разделите на количество месяцев.
  * Для создания статичекого метода напишите в классе `Main` (но не внутри метода `main`) конструкцию: `public static int calcPayment(???) {...`.
  * Для вызова созданного метода напишите в `main`: `int payment = calcPayment(2600000, 200000, 2);`.

## Задача 2 (необязательная)
:warning: **ВНИМАНИЕ** эта задача делается на основе предыдущей и в том же реплите, т.е. в итоге вы присылаете только одну ссылку на две задачи. Зачёт по этой будет означать автоматический зачёт по предыдущей.

Вынесите статический метод рассчёта платежа рассрочки в отдельный класс `Finances` пакета `ru.netology.finances`. Помните, что сам `Main` в реплите всегда должен быть без пакета.
