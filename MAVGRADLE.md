# Maven и Gradle

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

Для закрепления лекционного материала попрактикуемся в том, как создавать проекты. 

Стандартный многомодульный проект имеет составляющие по функционалу:
* `db` - модуль работы с базой данных;
* `api` - модуль работы с web;
* `service` - слой сервисов.

Для начала создайте одномодульный проект - как это было показано на занятии.

После необходимо установить packaging в pom

```pom
<packaging>pom</packaging>
``` 

После создаем 3 папки в директории проекта: db, api, service.

В каждой из директории создаем pom.xml c содержимым:

```pom
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <parent>
        <artifactId>App</artifactId>
        <groupId>ru.netology</groupId>
        <version>1.0-SNAPSHOT</version>
    </parent>
    <modelVersion>4.0.0</modelVersion>
    <artifactId>db</artifactId>
    <packaging>jar</packaging>
</project>
``` 

где обязательно указываем parent - в качестве родительского модуля с его данными и 
название artifactId текущего модуля (db, api, service) 

Чтобы подключить новые модули к проекту, добавляем в корне проекта в файл pom.xml новые созданные модули:

```pom
  <modules>
    <module>db</module>
    <module>api</module>
    <module>service</module>
  </modules> 
``` 

После создания многомодульного проекта, подключим связанные модули между собой.
 
Для подключения модуля db в модуль  service добавим зависимость:

```pom
    <dependencies>
        <dependency>
            <groupId>ru.netology</groupId>
            <artifactId>db</artifactId>
            <version>1.0-SNAPSHOT</version>
            <scope>compile</scope>
        </dependency>
    </dependencies>
```  

Для подключения модуля service в модуль api добавим зависимость:

```pom
    <dependencies>
        <dependency>
            <groupId>ru.netology</groupId>
            <artifactId>service</artifactId>
            <version>1.0-SNAPSHOT</version>
            <scope>compile</scope>
        </dependency>
    </dependencies> 
```

Теперь можно собрать проект, выполнив команду: 

```shell script
mvn clean install
``` 

Для демострации работы модульности в проекте db создадим классы:

```java
public class DbSetting {

    private String name;
    private String password;

    public DbSetting(String name, String password) {
        this.name = name;
        this.password = password;
    }

}
```

```java
public class MyEntity {

    private UUID id;
    private String name;

    public MyEntity(String name) {
        this.name = name;
    }

    public UUID getId() {
        return id;
    }

    public void setId(UUID id) {
        this.id = id;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    @Override
    public String toString() {
        return new StringBuilder().append("MyEntity{").append("id=").append(id).append(", name='").append(name).append('\'').append('}').toString();
    }
}
```

```java
public class Db {

    private DbSetting dbSetting;
    private MyEntity myEntity;

    public Db(DbSetting dbSetting) {
        this.dbSetting = dbSetting;
        myEntity = new MyEntity("first");
        myEntity.setId(UUID.randomUUID());
    }

    public DbSetting getDbSetting() {
        return dbSetting;
    }

    public MyEntity getMyEntity() {
        return myEntity;
    }

    public void setMyEntity(MyEntity myEntity) {
        this.myEntity = myEntity;
    }
}
```

В проекте Service создадим класс:

```java
public class MyService {

    private DbSetting dbSetting = new DbSetting("name", "password");
    private String name = "myService";
    private Db db = new Db(dbSetting);

    public String getName() {
        return name;
    }

    public MyEntity setMyEntity(MyEntity myEntity) {
        myEntity.setId(UUID.randomUUID());
        db.setMyEntity(myEntity);
        return myEntity;
    }

    public MyEntity getMyEntity() {
        return db.getMyEntity();
    }
}
```

В проекте api создадим класс:

```java
public class Main {

    public static void main(String[] args) {
        MyService myService = new MyService();
        System.out.println(myService.getMyEntity());
        System.out.println(myService.setMyEntity(new MyEntity("second")));
        System.out.println(myService.getMyEntity());
    }
}
```

После успешной сборки проекта можем выполнить данный код. 

В результате выполнения данного задания мы получили модульный проект с разделением по функциональности

## Задача 2 (обязательная)

Для закрепления лекционного материала попрактикуемся, как создавать проекты. 

Стандартный многомодульный проект имеет составляющие по функционалу:
* `db` - модуль работы с базой данных;
* `api` - модуль работы с web;
* `service` - слой сервисов.

Для начала создайте одномодульный проек - как это делали на занятии.

После создаем 3 папки в директории проекта: `db`, `api`, `service`.

В каждой из директории создаем build.gradle c содержимым:

```groovy
plugins {
    id 'java'
}

group 'ru.netology'
version '1.0-SNAPSHOT'

repositories {
    mavenCentral()
}

dependencies {

}
``` 

Чтобы подключить новые модули к проекту, добавляем в корне проекта в settings.gradle новые созданные модули:

```groovy
include 'db'
include 'service'
include 'api'
``` 

После создания многомодульного проекта подключим связанные модули между собой.
 
Для подключения модуля db в модуль service добавим зависимость:

```groovy
dependencies {
    implementation project(":db")
}
```  

Для подключения модуля service в модуль api добавим зависимость:

```groovy
dependencies {
    implementation project(":db")
    implementation project(":service")
}
```

Теперь можно собрать проект, выполнив команду: 

```shell script
gradle build
``` 

Для демострации работы модульности в проекте db создадим классы.

```java
public class DbSetting {

    private String name;
    private String password;

    public DbSetting(String name, String password) {
        this.name = name;
        this.password = password;
    }

}
```

```java
public class MyEntity {

    private UUID id;
    private String name;

    public MyEntity(String name) {
        this.name = name;
    }

    public UUID getId() {
        return id;
    }

    public void setId(UUID id) {
        this.id = id;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    @Override
    public String toString() {
        return new StringBuilder().append("MyEntity{").append("id=").append(id).append(", name='").append(name).append('\'').append('}').toString();
    }
}
```

```java
public class Db {

    private DbSetting dbSetting;
    private MyEntity myEntity;

    public Db(DbSetting dbSetting) {
        this.dbSetting = dbSetting;
        myEntity = new MyEntity("first");
        myEntity.setId(UUID.randomUUID());
    }

    public DbSetting getDbSetting() {
        return dbSetting;
    }

    public MyEntity getMyEntity() {
        return myEntity;
    }

    public void setMyEntity(MyEntity myEntity) {
        this.myEntity = myEntity;
    }
}
```

В проекте Service создадим класс:

```java
public class MyService {

    private DbSetting dbSetting = new DbSetting("name", "password");
    private String name = "myService";
    private Db db = new Db(dbSetting);

    public String getName() {
        return name;
    }

    public MyEntity setMyEntity(MyEntity myEntity) {
        myEntity.setId(UUID.randomUUID());
        db.setMyEntity(myEntity);
        return myEntity;
    }

    public MyEntity getMyEntity() {
        return db.getMyEntity();
    }
}
```

В проекте api создадим класс:

```java
public class Main {

    public static void main(String[] args) {
        MyService myService = new MyService();
        System.out.println(myService.getMyEntity());
        System.out.println(myService.setMyEntity(new MyEntity("second")));
        System.out.println(myService.getMyEntity());
    }
}
```

После успешной сборки проекта можем выполнить данный код. 

В результате выполнения данного задания мы получили модульный проект с разделением по функциональности
