### Name: Makayla Carr

## Part One:
### Step 1: VPC Creation.
* An Amazon VPC is a virtural private cloud 
![Step1](screenshotCompilation/Step1.PNG?raw=true "Step 1")

### Step 2: My subnet, CARR-Subnet
* Subnets are used to define machines that are connected on a network. 
![Step2](screenshotCompilation/Step2.PNG?raw=true "Step 2")

### Step 3: Internet Gateway creation
* An internet gateway converts data and communications between other gateways.
![Step3](screenshotCompilation/Step3.PNG?raw=true "Step 3")

### Step 4: Route Table creation
* A route table is a set of rules that determine how internet traffic is directed.
![Step4](screenshotCompilation/Step4.PNG?raw=true "Step 4")
* Adding a rule to my route table that adds my internet gateway: 
![RTRule](screenshotCompilation/InternetGatewayRule.PNG?raw=true "Rule")
### Step 5: Security Group creation
* A security group is like a virtual firewall.
![Step5](screenshotCompilation/Step5.PNG?raw=true "Step 5")

## Part Two:

### Step 1:
* I selected the Amazon Linux 2 AMI and t2 micro instance. Screenshots are added.
![InstanceSelected](screenshotCompilation/instanceselected.PNG?raw=true "Instance Selected")
![AMIselected](screenshotCompilation/AMISELECTED.PNG?raw=true "AMI Selected")

### Step 2: 
* I attatched the instance to my VPC during the creation of the instance. 
![Part2Step2](screenshotCompilation/Part2Step2.PNG?raw=true "Part 2 Step 2")

### Step 3: 
* I chose to auto-assign an ip address to the instance. I honestly thought it just might be easier and would make communication easier.
![Part2Step3](screenshotCompilation/Part2Step3.PNG?raw=true "Part 2 Step 3")

### Step 4: 
* I added a volume during the creation of the instance, on the Add Storage step.
![Part2Step4](screenshotCompilation/Part2Step4.PNG?raw=true "Part 2 Step 4")

### Step 5:
* I added a tag during the creation of the instance, on the Add Tags step.
![Part2Step5](screenshotCompilation/Part2Step5.PNG?raw=true "Part 2 Step 5")

### Step 6:
* I added a security group during the creation of the instance, on the Congifure Security Group step. I chose to select an existing security group and added mine, CARR-sg.
![Part2Step6](screenshotCompilation/Part2Step6.PNG?raw=true "Part 2 Step 6")

### SSH:
* I changed the hostname using a command I found in a google search. 
  * The command: sudo hostnamectl set-hostname --static amazon-linux-2
  * The website: https://bangmetric.com/changing-hostname-of-an-aws-ec2-instance-linux/
![SSH](screenshotCompilation/SSH.PNG?raw=true "SSH") 
