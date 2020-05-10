# AirportLearnLib
Library for Skillbox courses

Это библиотека для домашнего задания 7.1
Чтобы подключить её, необходимо добавить в файл pom.xml своего maven-проекта
репозиторий на гитхабе, с которого будет скачиваться библиотека:

    <repositories>
        <repository>
            <id>AirportLearnLib-mvn-repo</id>
            <url>https://raw.github.com/Folko85/AirportLearnLib/mvn-repo/</url>
            <snapshots>
                <enabled>true</enabled>
                <updatePolicy>always</updatePolicy>
            </snapshots>
        </repository>
    </repositories>
    
    а также добавить в зависимости саму библиотеку:
    
    <dependencies>
        <dependency>
            <groupId>com.skillbox</groupId>
            <artifactId>AirportLearnLib</artifactId>
            <version>1.0.1</version>
        </dependency>
    </dependencies>
    
    После этого следует в IDEA, в контекстном меню файла pom.xml выбрать Maven -> reimport
    
    P.S. Зависимость может подсвечиваться красным, пока не выполнен импорт библиотеки.
    Но если она остаётся красным и после импорта - проверьте правильность ввода данных.
