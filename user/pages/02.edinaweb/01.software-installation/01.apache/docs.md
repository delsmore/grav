---
title: Apache
published: true
taxonomy:
    category:
        - docs
---

####Install Apache


	yum install httpd


####Open Port 80

	firewall-cmd --zone=public --add-port=80/tcp --permanent  

	firewall-cmd --reload 


####Start Apache

	systemctl start httpd.service


####Start Apache on Boot

	systemctl enable httpd.service
