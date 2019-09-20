Java Practice
====================

#### Intialize Maven App

- Check `mvn` version

`mvn --version`

- Initialze using archtype

`mvn archetype:generate -DgroupId=com.example.app -DartifactId=webscraping-jenkins-plugin -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false`
`mv webscraping-jenkins-plugin/src src && rm -rf webscraping-jenkins-plugin`

- Add pom.xml

- Run Hello World App !

`java -cp target/webscraper-jenkins-plugin-1.0-SNAPSHOT.jar com.example.app.App`

Todo:
- ~~Initialize Maven App~~
- Create Java Maven Application which scrapes a website
- Serialize Scraped Data.
- The scraped content is served on a Webpage through a Servlet.
- Use Concurrency to enhance performance.
- Convert Application to a Jenkins Plugin extending a BuildStep.



[Serializaton Crash Course](https://www.youtube.com/watch?v=uS37TujnLRw)
[Concurency & Multithreading tut](http://tutorials.jenkov.com/java-concurrency/index.html)
[Jenkins Plugin Dev](https://jenkins.io/doc/developer/plugin-development/)