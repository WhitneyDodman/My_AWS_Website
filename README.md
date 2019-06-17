# My_AWS_Website
Infrastructure as Code with sample index.php


This has a New VPC with Two Availability Zones in Canada-Central-1

There are two Private subnets and two Public subnets.  Although there is nothing in the Private Subnets, they are set up to be used for whatever you desire.  Just add the ports to the ACL and RouteTable.

There is a Launchconfig and and Autoscaling Group.

The PHP displays Hello World and the hostname.

The Instances are replaced if they do not respond.  They are upscaled if they get a heavy CPU load > 60% (Easier testing) and downscaled once it reaches <25%.

This can be done better with Ansible and Python.  There are repeats in the .json that can be accomplished with a language that has loops.  It is also tedious to maintain a list of AMIs for each region.  Ansible can go fetch the latest release by owner.
https://nathanwebster.me/2017/find-latest-aws-ami-ansible/

I'll be working on this for the next little while so I have a tool at my disposal.  I just have to finish the deck and paint the garage floor first :)

Happy days!
