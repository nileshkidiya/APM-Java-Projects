1. Navigate to path cd 'E:\Download slave\QA_LAB_Applications\jboss-eap-7.0.0.GA-quickstarts\kitchensink'

2. Run command to create build 
mvn clean install wildfly:deploy -e -X 

Pre-requisites : 
If JBOss application is not up then this application won't be up so first we have to up the application and then target

3. WebAppURL : 
http://localhost:8080/jboss-kitchensink/
