## Security Issues in Cloud Computing

# project Description

Cloud computing is a set of services that provided by different IT vendors for rental to perform our activities in software era. Usually cloud computing services are delivered by a third party provider who owns the infrastructure.Cloud computing offers an innovative business model for organizations to adopt IT services without upfront investment. But as more and more information on individuals and companies are placed in the cloud, concerns are beginning to grow about just how safe an environment it is. Customers must demand transparency, avoiding vendors that refuse to provide detailed information on security programs. Ask questions related to the qualifications of policy makers, architects, coders and operators, risk-control processes and technical mechanisms and the level of testing that's been done to verify that service and control processes are functioning as intended, and that vendors can identify unanticipated vulnerabilities.

# Features list

![image](https://user-images.githubusercontent.com/77629263/127060122-57ca2244-fd0e-453d-a466-695999e32dd3.png)

* Infrastructure as a Service (IaaS)

* Software as a Service (SaaS)

*  Platform as a service (PaaS)

*  Cryptography

# project Motivation
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


# operating Instructions
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
# Troubleshooting
# News


RESEARCH QUESTIONS:
RQ1: First, virtualized networks offer insufficient networkbased controls.Given the nature of cloud services, the administrative access to IaaS network infrastructure and the ability to tailor network infrastructure are typically limited
![image](https://user-images.githubusercontent.com/77629263/127060358-a7a89f87-94e9-45d6-b8d8-7fc23d4df46b.png)

for example, friendly scans can’t be distinguished from attacker activity.

RQ2: The second challenge is in poor key management procedures.

RQ3: there are no standardized cloud-specific security metrics that cloud customers can use to monitor the security status of their cloud resources.


SUMMARY:
Cloud computing has started new era in the internet world not only for data storage but also on the availability, Security
and maintenance. However we need to understand the security
issues or any challenges among all cloud based technologies
before committing the code or data in third party. In this
paper I have concentrated major security issues and few
vulnerabilities in different models and services.
Vulnerabilities that are relevant for all cloud computing
components typically concern the provider or rather users’
inability to control cloud infrastructure as they do their own
infrastructure. Among the control challenges are insufficient
security audit possibilities, and the fact that certification
schemes and security metrics aren’t adopted to cloud computing.
Further, standard security controls regarding audit,
certification, and continuous security monitoring can’t be
implemented effectively.



References:
[1]. B. Grobauer, T. Walloschek and E. Stöcker, "Understanding Cloud Computing
Vulnerabilities," IEEE Security and Privacy, vol. 99, 2010.
[2]. J. Brodkin. (2008, Jun.). “Gartner: Seven cloud-computing security risks.” Infoworld,
Available: <http://www.infoworld.com/d/security-central/gartner-seven-cloudcomputingsecurity-
risks-853?page=0,1> [Mar. 13, 2009].
[3]. SO Kuyoro, F Ibikunle, O Awodele  “Cloud computing security issues and challenges”
[4]. S. Subashini, and V. Kavitha. (2010) “A survey on security issues in service delivery
models of cloud computing.” J Network Comput Appl doi:10.1016/j.jnca.2010.07.006. Jul.,
2010.
[5]. Global Netoptex Incorporated. “Demystifying the cloud. Important opportunities, crucial
choices.” pp4-14. Available: http://www.gni.com [Dec. 13, 2009].
[6]. S. Arnold (2009, Jul.). “Cloud computing and the issue of privacy.” KM World, pp14-22.
Available: www.kmworld.com [Aug. 19, 2009].
[7]. ISO/IEC 27005:2007 Information Technology—Security Techniques—Information Security Risk Management, Int’l Org. Standardization, 2007.
[8]. P. Mell and T. Grance, “Effectively and Securely Using the Cloud Computing Paradigm (v0.25),” presentation, US Nat’l Inst. Standards and Technology, 2009; http:// csrc.nist.gov/groups/SNS/cloud-computing.
[9]. L. Youseff, M. Butrico, and D. Da Silva, “Towards a Unified Ontology of Cloud Computing,” Proc. Grid Computing Environments Workshop (GCE), IEEE Press, 2008; doi: 10.1109/GCE.2008.4738443.
[10]. M. A. Morsy, J. Grundy and Müller I. “An Analysis of the Cloud Computing Security
Problem” In PROC APSEC 2010 Cloud Workshop. 2010.
[11]. R. K. Balachandra, P. V. Ramakrishna and A. Rakshit. “Cloud Security Issues.” In PROC
‘09 IEEE International Conference on Services Computing, 2009, pp 517-520.
[12]. Cloud Computing Use Case Discussion Group. "Cloud Computing UseCases Version 3.0,"
2010.
[13]. “Sampling issues we are addressing”, http://cloudsecurityalliance.org/issues.html#15, accessed on April 09, 2009.
[14]. “Service Level Agreement Definition and contents”, http://www.service-level-agreement.net, accessed on March 10, 2009.
[15]. http://www.cloudsecurity.org, accessed on April 10, 2009.
[16]. E. Grosse, “Security at Scale,” invited talk, ACM Cloud Security Workshop (CCSW), 2010; http://wn. com/2010_Google_Faculty_Summit_Security_at_Scale.
[17]. A Platform Computing Whitepaper. “Enterprise Cloud Computing: Transforming IT.”
Platform Computing, pp6, 2010.
[18]. N. Leavitt. “Is Cloud Computing Really Ready for Prime Time?” Computer, vol. 42, pp. 15-
20, 2009.
[19]. P. Kresimir and H. Zeljko "Cloud computing security issues and challenges." In PROC
Third International Conference on Advances in Human-oriented and Personalized
Mechanisms, Technologies, and Services, 2010, pp. 344-349.
[20]. R. K. Balachandra, P. V. Ramakrishna and A. Rakshit. “Cloud Security Issues.” In PROC
‘09 IEEE International Conference on Services Computing, 2009, pp 517-520.

