Deployment of the azure blockchain to a local azure enviorment. 
Note this was not tested on AD's outside of Wood-Azure AD and so failures are expected (please raise an issue in github if your having issues and ill debug)

Overall cost of deployment - 412 euros a month for one node (up to three is optimal but costs increase around 100 euro per node)

resources include:
-Storage account
-IoT Central Application
-SQL server
-SQL database
-Key vault
-Public IP address
-Log Analytics workspace
-Storage account
-Load balancer
-Network security group
-Virtual network
-Availability set
-Virtual machine
-Disk
-Virtual machine
-Disk
-Network interface
-Availability test
-Application Insights
-Key vault
-App Service
-Event Grid Topic
-Load balancer
-Public IP address
-App Service plan
-Service Bus Namespace
-Network security group
-Virtual network
-Virtual machine scale set

To deploy from the template included above please refer to the azure documentation https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-manager-quickstart-create-templates-use-the-portal#edit-and-deploy-the-template
Most rules for LB and NSG would need to be changed from wood defaults to your local resource defaults.

References:
https://channel9.msdn.com/Shows/Blocktalk/Building-your-first-Azure-Blockchain-Workbench-application
https://channel9.msdn.com/Shows/Blocktalk/Introduction-to-Azure-Blockchain-Workbench
