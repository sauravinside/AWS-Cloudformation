A three-tier architecture:
    1. Web tier: Launch an instance in the public subnet so that the instance should allow HTTP and SSH from the Internet
    2. Application tier: Launch an instance in the private subnet of the web tier, and it should allow only SSH from the public subnet of the web tier 
    3. DB tier: Launch an RDS MySQL instance in the private subnet, and it should allow connection on port 3306 only from the private subnet of the application tier
    4. Set up a Route 53 hosted zone, and direct the traffic to the EC2 instance
