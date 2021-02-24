# utility-jar-test

## Steps To Run 

- Replace the following values in settings.xml
    - NEXUS_USER : Replace this with username of nexus repository
    - NEXUS_PASSWORD: Replace this with password of nexus repository
    - NEXUS_URL: Replace this with maven public url of nexus

- Run the following command on root of repository


  ```  
  mvn -B deploy:deploy-file -s settings.xml -Durl=<nexus-snapshot-url>   -DpomFile=pom.xml -Dfile=target/utility-jar-test-1.0-SNAPSHOT.jar  -DrepositoryId=nexus 
  ```
 
Replace   `nexus-snaphot-url` with appropirate value