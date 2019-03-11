# Servicenow Instance details 
1.	Click on “developer.servicenow.com” and login.
2.	Click on the Manage tab and Instance under it as show in the below diagram.

![servicenow-dashboard](mule-servicenow-connectorDemo/Images/servicenow-dashboard.png)

3.	Instance tab will open and display the instance details which is created for you. 

![myinstance](mule-servicenow-connectorDemo/Images/myinstance.png)

4.	Login into your instance for further details. 
5.	Click on the incident which is our interest as of now.

![incidentdetails](mule-servicenow-connectorDemo/Images/incidentdetails.png)


# Configuring/developing Anypoint studio	
1.	Add the service now module in the workspace.

![addModuleFromExchange](mule-servicenow-connectorDemo/Images/addModuleFromExchange.png)


![selectModule](mule-servicenow-connectorDemo/Images/selectModule.png)


2.	OR (Alternative to the above step)  You can add the dependency directly into the pom.xml file.
    <dependency>
            <groupId>com.mulesoft.connectors</groupId>
            <artifactId>mule-servicenow-connector</artifactId>
            <version>6.2.2</version>
            <classifier>mule-plugin</classifier>
  </dependency>

3.	Go to the “Global Element Tab” and create a “Servicenow Config” Connector.

![Servicenow Configuration Details](mule-servicenow-connectorDemo/Images/servicenow-config1.png)


![Servicenow Configuration Details](mule-servicenow-connectorDemo/Images/servicenow-config2.png)

4.	For Insert Operation where you can create an incident in servicenow.

![Servicenow Configuration Details](mule-servicenow-connectorDemo/Images/Config1.png)

5.	For GetRecords Operation to fetch the available records in servicenow.

 ![Servicenow Configuration Details](mule-servicenow-connectorDemo/Images/Config2.png)

6.	Detailed implementation is present in the github repository

https://github.com/Anupam2388/mule-servicenow-connectorDemo.git 

