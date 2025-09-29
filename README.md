# Create and Configure a vNet in Azure
This is a lab I built and practiced to strengthen my understanding of Azure networking fundamentals. I created a custom Virtual Network (vNet) and segmented it with subnets to simulate real-world infrastructure scenarios. I configured address spaces, applied encryption for secure traffic flow, and used tags to organize resources by environment and department—making the setup easier to manage and audit.

This lab helped me explore how vNets support scalable, secure communication between Azure services. Every step is documented with screenshots and narration, showing exactly how I approached the design, configuration, and governance of cloud networks.

## 🔹 Lab Objectives – Azure Virtual Network (vNet)
In this hands-on lab, I practiced building and securing an Azure Virtual Network from the ground up.

✅ Practiced creating a Virtual Network in Azure using the portal interface

✅ Configured custom address spaces and IP ranges to match realistic deployment scenarios

✅ Set up multiple subnets to logically segment resources within the vNet for better control and isolation

✅ Applied encryption settings to secure internal traffic and reinforce network security

✅ Used resource tags to organize the vNet by environment type—clearly labeling production vs. development

✅ Reviewed and validated all vNet and subnet configurations before deployment to ensure accuracy and alignment with best practices

## 📸 Screenshots
### Step 1: "Select Virtual Network and Subnet"
_<span title="Choose the appropriate virtual network and subnet for your resource">Screenshot shows the dropdown menus for selecting a vNet and its associated subnet during resource configuration.</span>_

![Select Virtual Network](Screenshots/Click%20Virtual%20Network.png)

### Step 2: Click + Create  
_Selected the “+ Create” button in the Virtual networks section to begin provisioning a new vNet. This step initiates the setup of custom address spaces, subnets, and region-specific connectivity for secure Azure infrastructure._

![ Click + Create ](Screenshots/Click%20Create%20vNet.png)

### Step 3: Click Resource group dropdown  
_Selected the Resource group dropdown to associate the virtual network with a logical container for related resources. This step simplifies Azure resource organization, access control, and cost tracking._

![Click Resource group dropdown](Screenshots/Click%20Resource%20Group%20dropdown.png)

### Step 4: Select ProdRG resource group  
_Assigned the virtual network to the **ProdRG** resource group to group the vNet with relevant production assets. This enhances resource management, access control, and billing._

![Select ProdRG resource group](Screenshots/Select%20ProdRG.png)

### Step 5: Click Virtual network name field  
_Selected the Virtual network name field to define a clear and descriptive label for the vNet. Naming the network helps with resource identification, automation scripts, and long-term infrastructure clarity._

![Click Virtual network name field](Screenshots/Click%20Virtual%20Network%20Name%20Field.png)

### Step 6: Type vNet-App and press Enter  
_Entered “vNet-App” as the virtual network name to clearly define and segment the network in Azure. Naming conventions aid in resource identification, automation, and governance._

![Type vNet-App and press Enter](Screenshots/Type%20vNet-App%20.png)

### Step 7: Click Next: Security  
_Advanced to the **Security** tab during virtual network creation to configure protection settings such as **encryption**. This step ensures secure access and traffic control for your vNet._

![Click Next: Security](Screenshots/Click%20Next.png)

### Step 8: Click Virtual network encryption checkbox  
_Checked the Virtual network encryption box to enable encryption for traffic within the vNet. This enhances data confidentiality and aligns with compliance requirements for secure cloud environments._

![Click Virtual network encryption checkbox ](Screenshots/CLick%20Virtual%20Network%20Encryption%20checkbox.png)

### Step 9: Click Next  
_to proceed with configuring your IP address range and defining subnets for logical resource segmentation within the virtual network._

![Click Next](Screenshots/Click%20Next%202.png)

### Step 10: Double-click 10.0.0.0  
_Double-clicked the default IPv4 address space **10.0.0.0/16** to edit or confirm the virtual network’s address range. This CIDR block defines the scope of IP allocation for subnets and connected resources._

![Double-click 10.0.0.0 ](Screenshots/Double-Click%20IP%20address%20range.png)

### Step 11: Type 192.168.0.0 and press Enter  
_Entered the custom IPv4 address space **192.168.0.0/16** to define the private IP range for the virtual network. This CIDR block sets the foundation for subnetting and internal resource communication._

![Type 192.168.0.0](Screenshots/Type%20192.168.0.0%20and%20press%20enter.png)

### Step 12: Click + Add a subnet  
_Selected the “+ Add a subnet” button to define a custom subnet within the virtual network. This step enables segmentation of the address space, allowing isolated resource groups and service-specific routing._

![Click + Add a subnet](Screenshots/Add%20a%20Subnet.png)

### Step 13: Click Subnet purpose dropdown  
_Selected the Subnet purpose dropdown to define the role of the subnet within the virtual network. This setting helps Azure optimize routing, security, and service behavior based on workload type._

![Click Subnet purpose dropdown](Screenshots/Click%20Subnet%20Purpose%20dropdown.png)

### Step 14: Select Default subnet name  
_Selected “Default” as the subnet name to designate the primary segment within the virtual network. This naming convention simplifies routing, policy assignment, and resource grouping._

![Select Default subnet name](Screenshots/Select%20Default%20from%20Dropdown.png)

### Step 15: Double-click defaultv2  
_Double-clicked the subnet name “defaultv2” to edit its properties, including address range, security group, and delegation settings. This step ensures the subnet is correctly configured before deployment._

![Double-click defaultv2 ](Screenshots/Double-Click%20Default%202.png)

### Step 16: Type apps and press Enter  
_Entered “apps” as the subnet name to designate a dedicated segment for application workloads. Clear naming conventions help organize resources, apply targeted policies, and simplify future scaling._

![Type apps and press Enter ](Screenshots/Type%20apps%20for%20Subnet.png)

### Step 17: Click here to scroll down  
_Scrolled down the subnet configuration panel to access advanced options like NAT gateway, route table, service endpoints, and delegation. This step ensures full visibility before finalizing subnet setup._

![Click here to scroll down](Screenshots/Scroll-down%20to%20see%20other%20settings.png)

### Step 18: Click Add  
_Selected the “Add” button to finalize subnet configuration and attach it to the virtual network. This step commits the subnet’s address range, security settings, and routing policies for deployment._

![Click Add ](Screenshots/Click%20Add%20for%20the%20Subnet.png)

### Step 19: Click Next  
_Advanced to the next configuration blade after defining IP address space and adding subnets like **default** and **apps**. This step transitions from network layout to tagging._

![Click Next](Screenshots/Click%20Next%20to%20assign%20Tags.png)

### Step 20: Click Name dropdown  
_Selected the tag **Name** dropdown to choose a predefined label for the virtual network. Tags help organize resources by environment, department, or cost center — making management and billing more efficient._

![Click Name dropdown](Screenshots/Click%20Name%20Dropdown.png)

### Step 21: Select Environment  
_Selected “Environment” from the tag name dropdown to classify the virtual network by its deployment context — such as Development, Testing, or Production. Tagging improves cost tracking, automation, and resource visibility._

![Select Environment](Screenshots/Select%20Environment%20.png)

### Step 22: Click Value dropdown  
_Selected the tag **Value** dropdown to assign a specific environment label — such as Development, Staging, or Production — to the virtual network. This enhances resource tracking, automation, and cost attribution._

![Click Value dropdown](Screenshots/Click%20Value%20dropdown.png)

### Step 23: Select Production  
_Chose “Production” from the tag Value dropdown to indicate the virtual network’s operational environment. This tag helps distinguish mission-critical workloads from development or staging, improving governance and cost tracking._

![Select Production](Screenshots/Select%20Production.png)

### Step 24: Click Next  
Click to review the configured settings—this step confirms your vNet name, resource group, and prepares for IP range and subnet definition._

![Click Next](Screenshots/Click%20Next%20to%20Review.png)

### Step 25: Click Create  
_Selected the "Create" button to deploy the virtual network **AzureVNet** with its configured subnets, IP ranges, security settings, and tags. This action provisions the network infrastructure, enabling connectivity for dependent Azure services._

![Click Create](Screenshots/Click%20Create%20to%20Begin%20Deployment.png)

### Step 26: Deployment in progress  
_Triggered deployment for **Web-App-17268972413**, initiating resource provisioning and configuration. This step monitors the deployment lifecycle and ensures successful setup of the web application environment._

![Deployment in progress](Screenshots/Veiw%20the%20deployment%20.png)

### Step 27: Click Go to resource  
_Selected the “Go to resource” button after successful deployment of **vNet-App-17268972413**. This step opens the resource overview for post-deployment validation, configuration, and integration with other Azure services._

![Click Go to resource](Screenshots/Go%20to%20Resource%20after%20Deployemt%20finish.png)

### Step 28: Expand Settings  
_Clicked the “Settings” section in the left sidebar to access advanced configuration options for the virtual network **vNet-App**. This includes diagnostics, access control, tagging, and integration with security services._

![Step: Expand Settings](Screenshots/Expand%20Settings.png)

### Step 29: Click Address space  
_Selected the “Address space” field to review or modify the IP range assigned to **VNetApp**. This CIDR block defines the scope for subnetting and internal resource communication across the virtual network._

![Click Address space](Screenshots/Click%20Address%20Space.png)

### Final Step 30: Click Subnets  
_Opened the **Subnets** blade to view and manage subnet configurations within the virtual network **vNet-App**. This includes subnet names, address ranges, service endpoints, NAT gateways, and security group assignments._

🔚 _This marks the end of the virtual network setup steps. From here, you’ll see a detailed table of existing subnets and can begin provisioning workloads, applying policies, or integrating services like Azure Firewall or Bastion._

![Click Subnets ](Screenshots/Click%20Subents.png)