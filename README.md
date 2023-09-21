# Browserstack-Parallel-Testing
This project contains test to run it parallelly over browserstack vm using browserstack sdk and browserstack local for private network. 

Public network:
If target application is accessible over internet directly then this project will execute the test using browserstack sdk. The Java agent mentioned in pom file will 
intercept the test and start its execution over Browserstack cloud irrespective of local configuration.

Private network:
If application is accessible through private network then we have to use browserstack local. Browserstack local need to be true in browserstack.yaml file in order to access 
these type of application.
