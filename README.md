# Build a Virtual Private Cloud (AWS VPC)

**Project Link:** https://learn.nextwork.org/projects/aws-networks-vpc  
**Author:** Shane Brown  

---

## Overview

This project focuses on building a Virtual Private Cloud (VPC) in Amazon Web Services to understand how cloud networking is structured and secured. The goal is to learn how AWS isolates resources, controls network traffic, and connects cloud environments to the internet.

By completing this project, I gained hands-on experience with core networking components that form the foundation of most AWS architectures.

---

## What I built

I built a custom Amazon VPC and configured the key components required to make it functional, including:

- A Virtual Private Cloud with a defined IPv4 CIDR block  
- Public and private subnets across Availability Zones  
- An Internet Gateway to allow external connectivity  
- Routing and subnet settings to control traffic flow  

This setup demonstrates how cloud resources are isolated by default and only exposed when explicitly configured.

---

## Key concepts learned

- What a Virtual Private Cloud (VPC) is and why it’s used  
- How CIDR blocks define IP address ranges  
- The difference between public and private subnets  
- How Internet Gateways enable outbound and inbound traffic  
- Why AWS provides a default VPC and when to create a custom one  

---

## AWS Console vs AWS CLI

I explored creating VPC resources using both the AWS Management Console and the AWS CLI through CloudShell.

- The **Console** is useful for learning, visualization, and quick troubleshooting  
- The **CLI** is faster for repeatable tasks, automation, and scripting infrastructure  

Using both approaches helped reinforce how cloud infrastructure can be managed visually or programmatically.

---

## Documentation

📄 **Full project documentation:**  
[documentation.md](./documentation.md)

This file contains step-by-step notes, explanations, reflections, and command examples from completing the project.

---

## Credits

Built as part of the **NextWork** AWS learning series.
