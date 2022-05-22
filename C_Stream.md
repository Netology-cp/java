# Stream API

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
  <summary>Сдаём через гитхаб </summary>
  
  Время пришло познакомиться с профессиональными инструментами для контроля версий вашего кода. Теперь мы не сдаём домашние задания в реплите, а заливаем проект из идеи сразу же в публичный гитхаб-репозиторий. Одна задача - один репозиторий.
  
  Для того чтобы в репозитории не отслеживался всякий мусор, не забывайте добавлять `.gitignore`.
  В нём должны игнорироваться файлы идеи (правила `*.iml` и `.idea`), папки для автогенерируемых результатов сборки (`out`, позже - `target`).
  Этот файл должен находиться в корне вашего репозитория, а сам репозиторий должен быть инициализирован в корне вашего проекта.
  Т.е. открывая репозиторий вы должны сразу видеть папку `src`.
  Если вы забыли проигнорировать какие-либо файлы и они попали в репозиторий, используйте команду `git rm`.

</details>

## Задача 1 (обязательная)

В данной задаче предлагается проанализировать массив данных с информаций о людях с использованием стримов из библиотеки `Stream API`. 

Для работы необходимо подготовить несколько классов, а именно:
1. `Sex`, содержащий типы полов:
```java
public enum Sex {
    MAN,
    WOMAN
}
```
2. `Education`, содержащий типы образования:
```java
public enum Education {
    ELEMENTARY,
    SECONDARY,
    FURTHER,
    HIGHER
}
```
3. `Person`, содержащий информацию об имени, возрасте, поле и образовании человека:
```java
class Person {
    private String name;
    private String family;
    private Integer age;
    private Sex sex;
    private Education education;

    public Person(String name, String family, int age, Sex sex, Education education) {
        this.name = name;
        this.family = family;
        this.age = age;
        this.sex = sex;
        this.education = education;
    }

    public String getName() {
        return name;
    }

    public String getFamily() {
        return family;
    }

    public Integer getAge() {
        return age;
    }

    public Sex getSex() {
        return sex;
    }

    public Education getEducation() {
        return education;
    }

    @Override
    public String toString() {
        return "Person{" +
                "name='" + name + '\'' +
                ", family='" + family + '\'' +
                ", age=" + age +
                ", sex=" + sex +
                ", education=" + education +
                '}';
    }
}
```

Из коллеции объектов `Person` необходимо:
1. Найти количество несовершеннолетних (т.е. людей младше 18 лет).
2. Получить список фамилий призывников (т.е. мужчин от 18 и до 27 лет).
3. Получить отсортированный по фамилии список потенциально работоспособных людей с высшим образованием в выборке (т.е. людей с высшим образованием от 18 до 60 лет для женщин и до 65 лет для мужчин).

В классе `Main` в функции `main()` необходимо создать коллекцию экземпляров класса `Person`. Вам потребуется действительно большое количство данных. Для примера будем считать, что Вы производите перепись населения города Лондон с населением в 10 миллионов человек. Для генерации исходных данных воспользуемся следующим способом:
```java
List<String> names = Arrays.asList("Jack", "Connor", "Harry", "George", "Samuel", "John");
List<String> families = Arrays.asList("Evans", "Young", "Harris", "Wilson", "Davies", "Adamson", "Brown");
Collection<Person> persons = new ArrayList<>();
for (int i = 0; i < 10_000_000; i++) {
    persons.add(new Person(
                names.get(new Random().nextInt(names.size())),
                families.get(new Random().nextInt(families.size())),
                new Random().nextInt(100),
                Sex.values()[new Random().nextInt(Sex.values().length)],
                Education.values()[new Random().nextInt(Education.values().length)])
    );
}
```
### Подсказки
Из созданной коллекции `persons` для каждого задания создавайте новый стрим методом `stream()` и далее применяйте к нему ряд промежуточных операций и одну терминальную:
1. Для поиска несовершеннолетних используйте промежуточный метод `filter()` и терминальный метод `count()`.
2. Для получения списка призывников потребуется применить несколько промежуточных методов `filter()`, а также для преобразования данных из `Person` в `String` (так как нужны только фамилии) используйте метод `map()`. Так как требуется получить список `List<String>` терминальным методом будет `collect(Collectors.toList())`.
3. Для получения отсортированного по фамилии списка потенциально работоспособных людей с высшим образованием необходимо применить ряд промежуточных методов `filter()`, метод `sorted()` в который нужно будет положить компаратор по фамилиям `Comparator.comparing()`. Завершить стрим необходимо методом `collect()`.