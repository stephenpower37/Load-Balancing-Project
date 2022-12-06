# Load-Balancing-Project
Developer Operations assignment that automates the management of a web app using load-balancing and auto-scaling through AWS. Auto-scaling was set up based on CloudWatch alarms. If CPU usage or messages in SQS exceeded a certain value, the auto-scaling group would scale out. An application load balancer was set up and mapped with a custom VPC so the public subnets could be used in order to deploy the web app.

## Monitoring Script
A monitoring script was written using the shell scripting language in order to monitor custom metrics on the EC2 instances. The script monitored the following 
metrics: percentage of used memory, the number of total and port 80 TCP connections, the percentage of I/O wait time, the number of HTTPD processes running and the total number of processes running. [Monitoring File](https://github.com/stephenpower37/Load-Balancing-Project/blob/main/script.sh)

## Documentation
Report on Load-Balancing and Auto-Scaling Implementation: [Documentation File](https://github.com/stephenpower37/Load-Balancing-Project/blob/main/CA2-StephenPower-Documentation.pdf)
