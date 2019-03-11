# Mule 4 ServiceNow Connector Demo
The ServiceNow connector facilitates connections between Mule and ServiceNow apps. You can use the ServiceNow operations with the custom ServiceNow tables, along with any operations available through the installed plugins.

# Prerequisites
- A ServiceNow account (Steps are mentioned below)
- Anypoint Studio, Design Center, or a standalone application developed in XML.



# ServiceNow Instance details 
1.    Click on **developer.servicenow.com** and **Login**
2.    Click on the **Manage tab** and **Instance** under it as shown in the below diagram.

   ![servicenow-dashboard](mule-servicenow-connectorDemo/Images/servicenow-dashboard.png)

3.    Instance tab will open and display the instance details which is created for you. 
    
   ![myinstance](mule-servicenow-connectorDemo/Images/myinstance.png)

4.    **Login to your instance** for further details. 
5.    Click on the **Incidents**.
    
   ![incidentdetails](mule-servicenow-connectorDemo/Images/incidentdetails.png)


# Configuring Anypoint studio    
1.    Add the ServiceNow module in the project.
    
   ![addModuleFromExchange](mule-servicenow-connectorDemo/Images/addModuleFromExchange.png)
    
   ![selectModule](mule-servicenow-connectorDemo/Images/selectModule.png)


2.    OR (Alternative to the above step)  You can add the dependency directly into the pom.xml file.
    '<dependency>
            <groupId>com.mulesoft.connectors</groupId>
            <artifactId>mule-servicenow-connector</artifactId>
            <version>6.2.2</version>
            <classifier>mule-plugin</classifier>
  </dependency>'

3.    Go to the **Global Element Tab** and create a **ServiceNow Config** Connector.
    
   ![Servicenow Configuration Details](mule-servicenow-connectorDemo/Images/servicenow-config1.png)
    
   ![Servicenow Configuration Details](mule-servicenow-connectorDemo/Images/servicenow-config2.png)

4.    For **Insert Operation** where you can create an incident in ServiceNow.
    
   ![Servicenow Configuration Details](mule-servicenow-connectorDemo/Images/Config1.png)

5.    For **GetRecords Operation** to fetch the available records in ServiceNow.
    
   ![Servicenow Configuration Details](mule-servicenow-connectorDemo/Images/Config2.png)

6.    **Detailed implementation** is present in the Github repository

    https://github.com/Anupam2388/mule-servicenow-connectorDemo.git 
    
**Note:** Apart from the above mentioned two operations. Other Operations supported by ServiceNow connector are as below;
- Aggregate
- Delete Multiple
- Delete Record
- Get
- Get Keys
- Insert Multiple
- Update
