## AWS Cloud Practitioner:Module 3 - Global Infrastructure and Reliability

Module 3 explained the AWS Global Infrastructure with geographical regions which include multiple avilability zones that can provide network redundancy and service reliability. Each Region meets national data governance requirements/legislation.

<p align="center">
  <img src="availability-zones.png">
</p>

Edge locations can be set up in any region to cache an instance closer to customers, thus providing lower latency and better quality of service.  Useful for services with multi-national customers. For example, a company in Brazil with a large customer base in China could spin up an Edge location in China - see image below:

<p align="center">
  <image src="edge-locations.png">
</P>

## ☁️ How to Provision Resource

AWS Infrastructure can be provisioned via multiple tools:

1. AWS Console - Set up infrastructure using the GUI
2. AWS CLI - better for managing multiple instances, via Command Line using yaml or json
3. Software Development Kits - for developers

Managing Infrastructure via code aka 'infrastructure as code' provides much higher efficiency to infrastructure management via command line scripts and configuration settings for auto scaling, load balancing and health monitoring. AWS have a couple of tools for that:

4. AWS Elastic Beanstalk 
5. AWS Cloud Formation 

## End of module 3.
