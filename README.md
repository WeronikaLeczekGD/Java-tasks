## Java-tasks

1. [Download/install Tomcat server]

2. [Verify that it works by visiting the root page](#ad-2)
* What ports are used by the java process?

-By default, Apache Tomcat runs on port 8080

3. [Remove all default applications (including manager), restart Tomcat]

4. [Download Jenkins WAR and deploy into Tomcat](#ad-4)

5. [Verify that application works (visit application URL)](#ad-5)

6. [Enable JMX in Tomcat](#ad-6)
* What ports are used by the java process?

-Now it is set to 9000

* Change CATALINA_OPTS to use same for RMI as for JMX

* What ports are used by the java process?

-It is 9000

7. [Rerun tomcat with min heap size 10M and max heap size 20M](#ad-7)
* What type of error will you get?
* Increase min heap size to 1G and max heap size to 3G, enable parallel garbage collector.

8. [Connect by JConsole to Tomcat and look around](#ad-8)

9. [Stop Tomcat](#ad-9)

10. [Launch Jenkins WAR as standalone application, verify that it works](#ad-10)




## Ad 2
<img width="1273" alt="Screenshot 2022-11-17 at 12 30 31" src="https://user-images.githubusercontent.com/114099418/202735401-6b11010d-b4ef-4b50-90e1-9e3a907156f2.png">

*There is no root page because I have removed all default applications

## Ad 5
![Screenshot 2022-11-18 at 15 42 26](https://user-images.githubusercontent.com/114099418/202735434-45c163ec-aeda-40d7-814c-fb9a29d9b603.png)

## Ad 7
![Screenshot 2022-11-18 at 15 47 30](https://user-images.githubusercontent.com/114099418/202735496-e52f1886-429d-4ed0-bb4b-bc4fc111cb05.png)
![Screenshot 2022-11-18 at 16 11 09](https://user-images.githubusercontent.com/114099418/202737536-a96b7476-37a7-4e63-8477-3682d906ee5b.png)

## Ad 8
![Screenshot 2022-11-18 at 15 51 23](https://user-images.githubusercontent.com/114099418/202735552-8dc1a268-b9f6-451e-9b96-569b343fadad.png)

## Ad 10
![Screenshot 2022-11-18 at 16 13 01](https://user-images.githubusercontent.com/114099418/202737506-0d141ca7-7103-429f-84eb-1b634b66fd25.png)
