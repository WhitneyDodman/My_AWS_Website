# My_AWS_Website
Infrastructure as Code with sample index.php


This has a New VPC with Two Availability Zones in Canada-Central-1

There are two Private subnets and two Public subnets.  Although there is nothing in the Private Subnets, they are set up to be used for whatever you desire.  Just dd the ports to the ACL and RouteTable.

There is a Launchconfig and and Autoscaling Group.

The PHP displays Hello World and the hostname.

The Instances are replaced if they do not repond.  They are added to if they get a heavy CPU load > 60% (Easier testing) and downscaled once it reaches <25%.
