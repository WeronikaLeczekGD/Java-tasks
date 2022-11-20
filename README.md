## Java-tasks

1. Download/install Tomcat server

2. [Verify that it works by visiting the root page](#ad-2)
* What ports are used by the java process?

3. Remove all default applications (including manager), restart Tomcat

4. Download Jenkins WAR and deploy into Tomcat

5. [Verify that application works (visit application URL)](#ad-5)

6. [Enable JMX in Tomcat](#ad-6)

* What ports are used by the java process?
* Change CATALINA_OPTS to use same for RMI as for JMX
(screen is in Ad 7)
* What ports are used by the java process?

7. [Rerun tomcat with min heap size 10M and max heap size 20M](#ad-7)
* What type of error will you get?
* Increase min heap size to 1G and max heap size to 3G, enable parallel garbage collector.

8. [Connect by JConsole to Tomcat and look around](#ad-8)

9. [Stop Tomcat](#ad-9)

10. [Launch Jenkins WAR as standalone application, verify that it works](#ad-10)


## Ad 2

1. Root page:

![Screenshot 2022-11-20 at 17 34 48](https://user-images.githubusercontent.com/114099418/202914164-ddf1ae9d-18e2-4769-8368-bd20ce177d97.png)


* What ports are used by the java process?

-By default, Apache Tomcat runs on port 8080

*There is no root page because I have removed all default applications

## Ad 5

1. Visiting aplication url:

![Screenshot 2022-11-18 at 15 42 26](https://user-images.githubusercontent.com/114099418/202735434-45c163ec-aeda-40d7-814c-fb9a29d9b603.png)


## Ad 6

* What ports are used by the java process?

-Now it is set to 9000

* What ports are used by the java process?

-It is 9000

## Ad 7

1. Reruning tomcat with min heap size 10M and max heap size 20M caused this error:

![Screenshot 2022-11-18 at 16 11 09](https://user-images.githubusercontent.com/114099418/202737536-a96b7476-37a7-4e63-8477-3682d906ee5b.png)

2. So I changed min heap size to 1G and max heap size to 3G:

![Screenshot 2022-11-20 at 17 46 30](https://user-images.githubusercontent.com/114099418/202914721-b73b75b7-b77b-46a3-b9ba-8894a32f88ef.png)



## Ad 8

1. To connect by Jconsole to Tomcat I just typed 'jconsole' from a command line

2. After Connecting by JConsole to Tomcat:

![Screenshot 2022-11-18 at 15 51 23](https://user-images.githubusercontent.com/114099418/202735552-8dc1a268-b9f6-451e-9b96-569b343fadad.png)

## Ad 10

1. To Launch Jenkins WAR as standalone application I used this command 'java -jar jenkins.war --httpPort=8888'

2. I verified that it works:

![Screenshot 2022-11-18 at 16 13 01](https://user-images.githubusercontent.com/114099418/202737506-0d141ca7-7103-429f-84eb-1b634b66fd25.png)
