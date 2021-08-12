## Security Issues in Cloud Computing

# Project Description

Cloud computing is a set of services that provided by different IT vendors for rental to perform our activities in software era. Usually cloud computing services are delivered by a third party provider who owns the infrastructure.Cloud computing offers an innovative business model for organizations to adopt IT services without upfront investment. But as more and more information on individuals and companies are placed in the cloud, concerns are beginning to grow about just how safe an environment it is. 

# Features list
In every cloud paltforms below services are common and accessable based on the role we have created. Below is the common diagram of basic services in cloud platform

![image](https://user-images.githubusercontent.com/77629263/127060122-57ca2244-fd0e-453d-a466-695999e32dd3.png)

* Infrastructure as a Service (IaaS)

* Software as a Service (SaaS)

*  Platform as a service (PaaS)

*  Cryptography

# Project Motivation
Moving to the cloud provides an easy way to archive data without investing in an on-premise infrastructure. Many organizations are moving infrequently accessed data (archive data) to the cloud to meet compliance regulations. In the past, tape storage was a common way to store data offsite, but the technology itself had a lot of issues, such as managing tape rotations, constantly changing technology and deterioration of tapes in storage.

when i was working in top MNC company they moved from IBM servers to cloud but earlier we had so many security walls to reach single word inside the server. So, what about if we move our data to cloud

why move your company data to the cloud? What's so special about it? What's the security that third party providing to you? How about personal data?

Based on these questions i started research on cloud platforms

# Cloud Configuaration

**How to create Microsoft Azure Account**

To create a new work account for your company, follow the steps below. You may need to request assistance from whoever has administrative permissions on your company's Microsoft Azure account.

1.Sign in to the Microsoft Azure portal (https://portal.azure.com).

2.From the left navigation menu, select the Azure Active Directory > Users.

3.Select New user and create a new Azure work account by entering a name and work email address. Ensure the Directory role is set as per the User requirement and select the Show Password checkbox at the bottom to view and make a note of the auto-generated password.

4.Complete the other required fields and select Create to save the new user.

The email address for the user account must be a verified domain name in your directory. You can list all the verified domains in your directory by selecting Azure Active Directory > Custom domain names in the left-navigation menu.

**How to create AWS Cloud Account**

1. Open the AWS website(http://aws.amazon.com/) and click Sign Up.

2. Follow the on-screen instructions. Part of the sign-up procedure involves receiving a phone call and entering a PIN using your phone keypad.

Next, create an IAM user and download (or copy) its secret access key.

3. Go to the IAM console (you may need to sign in to AWS first).

4. Click Users in the sidebar to view your IAM users.

5. If you don’t have any IAM users set up, click Create New Users to create one.

6 Select the IAM user in the list that you’ll use to access AWS.

7. Open the Security Credentials tab, and click Create Access Key.

9. On the resulting dialog box, click the Download Credentials button to download the credential file to your computer, or click Show User Security Credentials to view the IAM user’s access key ID and secret access key (which you can copy and paste).


# Operating Instructions
you will create an Amazon Virtual Private Cloud (Amazon VPC). When you create the Amazon VPC, you will create a public and a private subnet to manage the
flow of traffic between the subnet and the internet gateway. Below is a diagram of the infrastructure you will build:

![image](https://user-images.githubusercontent.com/77629263/128557652-9321f50d-acd0-4ee3-942d-2339f6aef2fb.png)

**Create a non-default Amazon VPC**
1. In the AWS Management Console find the VPC dashboard.
2. Click on Your VPCs.
3. Click Create VPC.
4. Configure the following settings, leaving other fields at their default values:
* VPC name: MyVPC
* Public subnet's IPv4 CIDR: 10.0.0.0/16
* IPv6 CIDR Block: No IPV6 CIDR Block
* Tenancy: Default
5. Click Create to create your Amazon VPC.
6. Click Close to return to your VPC Dashboard.

**Create a public subnet**
1. In the VPC dashboard, click Subnets in the left sidebar.
2. Click Create subnet.
3. Enter a Name tag: Public Subnet 1.
4. Select the Amazon VPC you just created from the dropdown list.
5. Save the Availability Zone as No preference.
6. IPv4 CIDR Block: 10.0.1.0/24
7. Click Create.

**Create an internet gateway**
1. In the VPC dashboard, click Internet gateways in the left sidebar.
2. Click Create internet gateway.
3. Enter a Name tag: MyVPC_IG.
4. Click Create
Attach your internet gateway to your Amazon VPC
1. In the VPC dashboard, click internet gateways in the left sidebar.
2. Find your internet gateway and notice the state: detached.
3. Select your internet gateway and Go to Actions  Attach to VPC.
4. Select the non-default Amazon VPC names MyVPC from the list and click Attach.
5. Click Close.

**Task1:** Create an Amazon S3 bucket and store an image file Let’s being by creating an Amazon S3 bucket and then store a file. The Amazon S3 buckets
needs to be configured to be publicly accessible.
1. In the AWS Management Console, on the Services menu, click S3.
2. In the Amazon S3 console, click Create bucket then configure:
Bucket name: Select/create a globally unique bucket name here
* Region: US East (N. Virginia)
* Click Next
* Tags:
* Key – Name
* Value – CloudFront Acceleration
* Click Next
* Click Next
* Click Create bucket
3. On the Amazon S3 Buckets page, click and highlight the Amazon S3 bucket you created.
4. Locate and click the Permissions option. The Block all public access setting is set to On. This needs to be changed.
5. Click Edit to change the settings.
6. Deselect the Block all public access option. Leave all other options deselected
7. Click Save
A dialogue box opens asking you to confirm your changes.
8. Type in the field, and then click Confirm
9. Click Overview tab.
10. Click Upload
11. Click Add files
12. Navigate to http://tinyurl.com/s3static to download and save these files to your desktop. Select an image from your computer that you would like to upload. If you don’t have a file prepared, visit https://unsplash.com/ to find and download an image to your desktop or use one of your own images. Then use that file for this step.
13. Click Next
14. To upload, set the permissions step, locate the Manage public permissions option, and click the dropdown arrow. Choose the Grant public read access to this object(s) option from the dropdown window selections. The following notification should display:
15. Click Next
16. Click Next
17. Click Upload
18. Copy the name of your file to your text editor for later use. For example, the name of your file could be “sample.png.”
19. Click and highlight the file that you uploaded.
20. In the slide out modal, locate the Overview section. Find and locate the Object URL, click it, and then copy the link to your clipboard
21. Paste the link in a new browser tab. Press Enter.


# Bugs list
If we gonna create cloud front without having privilege access we will get below error and for my student account i don't have some access to create security groups but i tried to create it in AWS cloud but it throws below errors.

![image](https://user-images.githubusercontent.com/77629263/128560975-32b3b0be-83ae-4059-9759-b08d21b1467b.png)

For creating DNS firewall we have to create the security role for each user or public in student access we are seeing unkown errors like below but still we are able to access the S3 bucket how it will be possible? is it a bug? 
![image](https://user-images.githubusercontent.com/77629263/128561514-8a735746-d7ff-47ee-a3c5-9cc54b921717.png)


# Troubleshooting
As per internet please reachout to AWS customer support {support@awseducate.com} they will answer and resolve any issues related to the cloud services.I sent couple of mails to them regarding error and access to different i got reply within 24 working hours.

# News
News on cloud security and issues in 2020 and 2021.Below listed articles referred apart from the references listed

* [The 5 Biggest Cloud Computing Trends In 2021](https://www.forbes.com/sites/bernardmarr/2020/11/02/the-5-biggest-cloud-computing-trends-in-2021/?sh=7b0546e412d9)
* [Top 5 Cloud Security Trends for 2021](https://www.bmc.com/blogs/cloud-security-trends/)
* [Top Cloud Security Challenges for 2021, Hear from Mark Nunnikhoven, VP of Cloud Research at Trend Micro, on the top cloud security challenges that will be faced in 2021.](
https://www.trendmicro.com/en_us/devops/21/b/top-cloud-security-challenges-for-2021.html)
* [Insights of 25 cloud trends for 2021 and beyond ](https://www.accenture.com/nl-en/blogs/insights/cloud-trends)
* [Pretty much every company has suffered some kind of cloud data breach ](https://www.techradar.com/news/pretty-much-every-company-has-suffered-some-kind-of-cloud-data-breach)
* [Cybersecurity Stocks To Buy As Wave Of Ransomware Attacks Raises Alarm ](https://www.investors.com/news/technology/cybersecurity-stocks/)
* [What Is A Cloud Security Review And Why Do I Need It? ](https://www.forbes.com/sites/forbestechcouncil/2020/07/16/what-is-a-cloud-security-review-and-why-do-i-need-it/?sh=75c3482a4be4)
* [Understanding the landscape of cloud security By Chris Deverill ](https://www.techradar.com/news/understanding-the-landscape-of-cloud-security)
* [Security In The Cloud Is Enhanced By Artificial Intelligence ](https://www.forbes.com/sites/davidteich/2021/04/01/security-in-the-cloud-is-enhanced-by-artificial-intelligence/?sh=38d418563967)
* [Cloud security: How to block and tackle ](https://www.ibm.com/blogs/cloud-computing/2014/11/30/cloud-security-how-to-block-and-tackle/)

# RESEARCH QUESTIONS:
RQ1: Why AWS throwing Errors inside Educate account?

RQ2: How key management procedures are there in Cloud Environment?

RQ3:  What are the standardized cloud-specific security metrics that cloud customers can use to monitor the security status of their cloud resources.

# Manifest:

* Journal i have prepared for my research 
* ReadMe.md file to know about my research

