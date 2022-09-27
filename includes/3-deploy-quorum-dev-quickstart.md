# Exercise - Deploy a Quorum Dev Quickstart

To obtain the RPC endpoint which is later required for deploying a workbench, you will need to follow some steps to deploy a Quorum Dev Quickstart for a start in this unit.  

The steps for deploying the are as follows: **Deployment of GoQuorum QuickStart**

Select the link given to reach the Microsoft portal <https://portal.azure.com/#home>

 1. Login to azure
    >[!Note]
    >
    >You must have an active student subscription]
      
      ![Screenshot of the designer view of a bot that collects basic information.](/media/3.1-Quorum-Dev-Quickstart.png)

<br>

 2. In the search bar, search for ‘Quorum’ and under Marketplace, select the option ‘Quorum Dev Quickstart’

      ![Screenshot of the designer view of a bot that collects basic information.](/media/3.2-Create-page-with-RPC-endpoint.png)

    >[!NOTE]  
    >
    > You will land on the page shown above once you select ‘Quorum Dev Quickstart’. On the bottom of the page, you can see a http link mentioned after Ethereum endpoint RPC. The format of the RPC endpoint is same as the http link format.

 3. On landing on the above shown webpage, select ‘Create’

      ![Screenshot of the designer view of a bot that collects basic information.](/media/3.3-Quorum-filled-form.png)

    > [!NOTE]  
    >
    > By clicking on create, you will be able to now see a form with field to fill.

      <br>

      ## Fill in the Azure resource fields

    You are presented with a number of fields that you need to fill in to be able to provision your cloud resource

    | Subscription      | Select the option 'Visual Studio Enterprise |
    | :---:       |    :----:   |
    | Resource Group    | Click on ‘Create New’ option below the field, and give a unique name for your’ resource group. ‘Quorum-dev’ is used as the same name for the Resource group.       |
    | Region   | Any region can be selected, while ‘West Europe’ is preferred for this application.         |
    | VM Name Prefix | Give a name for the VM prefix, since it will later be used as a credential while logging in. ‘quorum’ is taken as the sample VM Prefix name here. |
    | Admin Username | Just like the VM Name Prefix, even Admin Username will be stored as a credential in later steps. Hence give it a unique name. Here, ‘quorumdev’ is taken the sample username. |
    | Authentication type | Select ‘Password’ from the two given choices. |
    | Password | Making sure that the password matches all the above-mentioned criteria, give a password. This password will later be used during login procedure. |
    | Confirm Password | Re-enter the same password carefully to confirm the password. |
    | VM Disk Type | Select Premium SSD from the dropdown |

 4. Once you will the form completely, click on ‘Next: Size>’ option.

 5. Once you reach this page, click on ‘Change Size’ hyperlink

 6. From the pop-up menu, select the option ‘B4ms’ under VM size which has 4 vCPUs

 7. Click on Select on the pop-up menu and close it.

 8. Upon selecting size of the virtual machine, you are ready to deploy Quorum Quickstart. Click on ‘Review + Create’

      ![Screenshot of the designer view of a bot that collects basic information.](/media/3.4-review+create.png)

 9. Once you review all the details you entered, click on ‘Create’. It will take a while to get deployed.

      ![Screenshot of the designer view of a bot that collects basic information.](/media/3.5-azure-portal.png)

 10. Once deployed, to find the resource we deployed, come back to the Azure main portal <https://portal.azure.com/#home> And under the Navigate section, click on ‘Resource groups’

      ![Screenshot of the designer view of a bot that collects basic information.](/media/3.6-resource-groups.png)

You will be able to visualize the resource group you deployed with the Resource group name that you mentioned in the form before deploying it. Here, since the sample Resource group name was ‘Quorum-dev’, you can see a resource deployed on the name of Quorum-dev.

You can click on the name to see the working of Quorum Quickstart.
