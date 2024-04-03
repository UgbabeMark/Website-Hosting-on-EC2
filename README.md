# Website-Hosting-on-EC2

This project demonstrates how to deploy a website on an Amazon EC2 instance using Linux commands.

This repository contains resources and instructions for hosting a website on an AWS EC2 instance. Follow the steps outlined below to deploy your website successfully.

# Prerequisites:

. AWS Account

. Basic knowledge of AWS services

. Basic knowledge of Linux commands

# Steps:

# 1. Create an EC2 Instance

![Ec2 creation](EC2.png)

. Navigate to the EC2 dashboard on AWS Management Console.
. Launch a new EC2 instance, choosing an appropriate instance type, AMI, and configuration.

27. ![website](securitygroup.png)
. Ensure to configure security groups to allow inbound traffic on ports 80 (HTTP) and 22 (SSH) from anywhere.

# 2. Connect to EC2 Instance

![instance_connect](Instance_connect.png)


Connect to your EC2 instance using SSH or Instance Connect.

# 3. Update the System

![instance_connect](Update_system.png)


# 4. Install Web Server (Apache HTTP Server)
![instance_connect](Install_webserver.png)

hit y to install Apache


# 5. Check Status of HTTPD (Apache)

![website](httpd_statuscheck.png)

# 6. Enable HTTPD

![website](httpd_enable.png)

# 7. Check system running

![website](systemccheck_running.png)


# 8. Create a Directory

![website](Create_directory.png)
 cd temp/ after creating temp directory

# 9. Download Website zip Files

 ![website](download_websitesip.png)

 
# 10. list and Unzip Website Files

 ![website](list_directory.png)
 ![website](Unzip_website.png)


# 11. Navigate to the Unzipped Directory

![website](Unzippedfile.png)
use ls -lrt to see the file carvilla-v1.0



# 12. Check Files in the Directory

![website](check_directory.png)
cd carvilla-v1.0 and ls -lrt to see the available files



# 13. Move Files to Web Server Directory

 ![website](move_directory_files.png)
 

# 14. Verify Files Moved Successfully

 ![website](verify_moved.png)
 
 
# 15. Copy the public IP address of your EC2 instance.

 ![website](copy_publicip.png)

# 16. Paste it into a web browser and hit enter to access your website.

![website](paste_browser.png)

# 17. Test Your Website

 ![website](Test_website.png)

# 18. Linux Commands Used:

sudo yum update -y

sudo yum install -y httpd

systemctl status httpd

sudo systemctl enable httpd

mkdir temp

cd temp

wget https://www.free-css.com/assets/files/free-css-templates/download/page296/carvilla.zip

unzip carvilla.zip

cd carvillaV1.0

ls -lrt

sudo mv * /var/www/html/


Follow these instructions carefully to successfully deploy your website on an AWS EC2 instance. For any issues or further customization, refer to the AWS documentation or seek assistance from AWS support. reach me on Github: https://github.com/UgbabeMark


   
