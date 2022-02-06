# AWS-VPC-production-devlopment-environment
Creating production network and devlopment network by cloudformation automation.


Production Network:
1. Design and build a 4 tier architecture
2. Create 5 subnets out of which 4 should be private with names app1, app2, dbcache and db and one 
should be public named web.
3. Launch instances in all subnets and name them as per the subnet that they have been
launched in.
4. Allow dbcache instance and app1 subnet to send internet requests
5. Manage security groups and NACLs

Development Network:
1. Design and build 2 tier architecture with two subnets named web and db and launch instances in 
both subnets and name them as per the subnet names.
2. Make sure only web subnet can send internet requests
3. Create peering connection between production network and development network
4. Setup connection between db subnets of both production network and development network 
respectively
