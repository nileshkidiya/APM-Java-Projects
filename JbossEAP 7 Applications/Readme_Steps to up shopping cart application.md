1. Navigate to path cd 'E:\Download slave\QA_LAB_Applications\jboss-eap-7.0.0.GA-quickstarts\shopping-kart'

2. Run the command at jboss cli for client :
cd 'C:\Users\Nilesh Kidiya\EAP-7.3.0\bin'
\jboss-cli.bat --connect --file='E:\Download slave\QA_LAB_Applications\JbossEAP 7 Applications\jboss-eap-7.0.0.GA-quickstarts\shopping-cart\configure-system-exception.cli'

3. Run command to create build 
mvn clean install wildfly:deploy -e -X 

4. Verify jar file at deployment upload feature of Jboss EAP at Deployments tab. 
Files is placed at client and server directory : 
jboss-shopping-cart-client.jar
jboss-shopping-cart-server.jar

5. Run the command for client : 
mvn exec:java -f client/pom.xml -e -X

6. Run the command at jboss cli for restore :
.\jboss-cli.bat --connect --file 'E:\Download slave\QA_LAB_Applications\JbossEAP 7 Applications\jboss-eap-7.0.0.GA-quickstarts\shopping-cart\restore-system-exception.cli'

7. Undeploy Archive : 
mvn wildfly:undeploy

8. For debug application :
    mvn dependency:sources


