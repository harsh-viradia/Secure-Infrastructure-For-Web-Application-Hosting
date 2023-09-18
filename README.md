# Secure Infrastructure

![Secure Infrastructure](https://github.com/harsh-viradia/Secure-Infrastructure-For-Web-Application-Hosting/assets/140060556/7ccd6f1e-b1f2-4f34-8ba5-1fded5be10d2)


- In the above image we can see this is the most secure infrastructure. Let's see how this works.

- Network packet will enter through security VPC, where we used AWS WAF as our first firewall, which forward our request to the application load balancer.
- We have used AWS WAF for protect load balancer.
- Next is Application load balacner which is just carry forward to EC2 instance. In sort we just jump three IP address.
- Now in the other VPC is DMZ VPC where we ahve hosted our web servers. 
- DMZ VPC is just mediater who is reponsible to communicate database and user. 
- In the last VPC we hosted our database. 
- So when user trying to access our application the request will hit six different firewall. 
- So attacker never know our database IP and server IP so as point of security it's most secure infrastructure.
- All six firewall are AWS managed so there is no problem with downtime or any other issue so it's highly available also.   