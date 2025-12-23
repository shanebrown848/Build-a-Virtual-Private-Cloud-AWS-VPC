<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Build a Virtual Private Cloud

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-vpc)

**Author:** Shane Brown  
**Email:** shanebrown848@gmail.com

---

## Build a Virtual Private Cloud (VPC)

![Image](http://learn.nextwork.org/encouraged_yellow_silly_yeti/uploads/aws-networks-vpc_2facf927)

---

## Introducing Today's Project!

### What is Amazon VPC?

Amazon VPC is useful because you can stage or develop what you need and be able to have it in your own space and it will be protected in a sense.

I set up the VPC today then I was able to set up the connection to the internet there after.

### Personal reflection

It took me about 45 mins.

I have gone to school for networking and found it boring when I was just reading about it in a book, but in this project it was fun having that hands on experience.

---

## Virtual Private Clouds (VPCs)

### What I did in this step

### How VPCs work

VPCs are Virtual private cloud, basically vpc's are the reason why resources can be made private to you. If you didn't have vpc then anybody could have access to your information.

### Why there is a default VPC in AWS accounts

There was already a default VPC in my account ever since my AWS account was created. This is because this default VPC is a handy starting point, especially for beginners. Otherwise we may have to build everything from scratch. 

![Image](http://learn.nextwork.org/encouraged_yellow_silly_yeti/uploads/aws-networks-vpc_2facf927)

### Defining IPv4 CIDR blocks

To set up my VPC, I had to define an IPv4 CIDR block, which is Classless Inter-Domain Routing is a way to assign a whole block of IP addresses, kind of like creating a zone/area in a city.

---

## Subnets

### What I did in this step

### Creating and configuring subnets

Subnets are like different neighborhoods inside your city. There are already subnets existing in my account, one for every Availability Zone of a Region, which means you'll see 3 subnets on your page if your Region has 3 Availability Zones

### Public vs private subnets

The difference between public and private subnets are public subnet can communicate with external networks. Private subnets are for internal resources. For a subnet to be considered public, it has to be connected to an internet gateway.

![Image](http://learn.nextwork.org/encouraged_yellow_silly_yeti/uploads/aws-networks-vpc_157c4219)

### Auto-assigning public IPv4 addresses

Once I created my subnet, I enabled auto-assign public IPv4 address. This setting makes sure any EC2 instance launched in that subnet will instantly get a public IP address so you won't have to create one manually.

---

## Internet gateways

### What I did in this step

### Setting up internet gateways

Internet gateways are key to making applications available on the internet. An internet gateway connects your VPC and the internet.

Attaching an internet gateway to a VPC means resources in your VPC can now access the internet. If I missed this step then there would be no way to access the resources outside of the VPC.

![Image](http://learn.nextwork.org/encouraged_yellow_silly_yeti/uploads/aws-networks-vpc_4ae90410)

---

## Using the AWS CLI

### What I'm doing in this extension

In this secret mission, I will be creating a VPC and launching it using the Command Line to see which way is faster, because it would not hurt to have experience in launching a project throught the command line. For me personally I enjoy my times on the command line.

### Exploring CloudShell and CLI

VPC resources could also be created with CloudShell, which is a browser-based command-line environment provided by cloud providers like AWS. It gives users instant access to a pre-configured shell with the necessary tools and credentials to manage cloud resources securely — without needing to install anything locally.

CLI is short for Command Line Interface, a tool that allows users to interact with cloud services by typing text-based commands. With the AWS CLI (for example), users can create, configure, and manage resources like VPCs, instances, databases directly from their terminal or command prompt. It's very powerful for automation and scripting tasks.

### Debugging my setup

To set up a VPC or a subnet, you can use the command aws ec2 create-subnet --vpc-id [VPC-ID]
Make sure to avoid errors by including the Cidr block so the correct command should look like this. aws ec2 create-subnet --vpc-id [VPC-ID] --cidr-block [ADD-CIDR-BLOCK-HERE]


![Image](http://learn.nextwork.org/encouraged_yellow_silly_yeti/uploads/aws-networks-vpc_9b2465411)

### Comparing CloudShell vs AWS Console

Compared to using the AWS Console, an advantage of using commands is that you can automate tasks, repeat setups quickly, and handle complex configurations more efficiently. With tools like CloudShell or the AWS CLI, you can script entire environments, avoid manual clicks, and reduce the chance of human error when repeating tasks.

An advantage of using the Console is that it provides a visual interface that’s easier for beginners or for one-time setups. You can see diagrams, relationships between resources, and easily navigate different services without needing to remember command syntax.

Overall, I preferred using CloudShell and CLI commands for tasks like setting up VPC resources because they give me more control, speed, and repeatability, especially as I get more comfortable with AWS. But for initial learning or troubleshooting, the Console is very helpful.

---

---
