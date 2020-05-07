![](https://repository-images.githubusercontent.com/243465953/e8faaf80-6491-11ea-84c2-8f7116873cff)

## About

UnSAFE Bank is a core virtual banking suite designed with the aim to incorporate the cybersecurity risks and various test cases such that newbie, developers, and security analysts can learn, hack and improvise their vulnerability assessment and penetration testing skills on Web, Android and iOS application.

**Note:** Only iOS application is launched as a part of this release. Android and Web application are under development.

## Application Features

It currently consists of the following functionalities:

* Funds Transfer
* View Account Statement
* Add/View Beneficiary

**Note:** New features and vulnerability integration is under development.

## Vulnerability Coverage

Say it intentionally or unintentionally, we have introduced vulnerabilities which varies from low severity to critical severity. 

## Setting up the environment

### Dependencies

1. Install [git](https://www.atlassian.com/git/tutorials/install-git) on your system.
2. Install [docker-compose](https://docs.docker.com/compose/install/) on your system.
3. Make sure that port 80 of your laptop/desktop does not have a running service.
4. Android/iOS phone would be required for mobile application testing.

### Setting up the server

1. Clone the repository on your system (Laptop/Desktop)
`git clone https://github.com/lucideus-repo/UnSAFE_Bank.git`
2. Navigate to the UnSAFE_Bank/Backend directory
`cd UnSAFE_Bank/Backend`
3. Start docker service (if not running)
`sudo service docker start`
4. Start the containers
`docker-compose up -d`

### Installing iOS Application

1. Download and install the [Cydia Impactor](http://www.cydiaimpactor.com/) on your system.
2. Connect your iPhone to the system and open Cydia Impactor.
3. Navigate to the **/iOS** directory.
4. Drag and drop the **UnSAFE Bank.ipa** file on Cydia Impactor.
5. Follow the Cydia Impactor process to complete the installation.
6. Trust the developer profile (if required) and your application would be ready to use.

**Note:** You can always use [other methods](https://mobile-security.gitbook.io/mobile-security-testing-guide/ios-testing-guide/0x06b-basic-security-testing#installing-apps) to install the iOS application as per your convenience.

### Test Connectivity Status

1. Make sure your iPhone and System are connected to the same network.
2. Check your system IP address (ifconfig) and the port on which backend is running (Default port is 80).
3. Open the iOS Application and provide the connection strings on the top right corner to connect to the backend.
4. If there is no error message on your iPhone then "You are connected successfully".
5. If there is an error, make sure your backend is running successfully or you have provided the valid IP address/port.

### Login Credentials

Customer ID and password is required to login into the application. You can always sign up as a new user in the application.

On successful sign up:

1. You will be provided with your Customer ID corresponding to your account. Always note your Customer ID and keep it SAFE for further usage.
2. Your dummy PII and account information would be created automatically.
3. Default beneficiaries would be added in your account.
4. Virtual money would be added in your account ranging from 1 to 5 lakh.

### Existing User Bank Accounts

Following data can be used to perform actions such as add beneficiary, funds transfer etc.

| Account Holder | Account Number | IFSC Code |
| -------------- | -------------- | --------- |
| Vipul Malhotra | 003558008876 | IFSC00009 |
| Kevin Winkel | 270365500638 | IFSC00009 |
| Kelly Campbell | 533074805951 | IFSC00010 |
| Krystal Langworth | 731258783797 | IFSC00006 |
| Margarita Mann | 359502423130 | IFSC00010 |
| David Mahabir | 795554898923 | IFSC00002 |
| Boris Gerhold | 485064210112 | IFSC00006 |
| Nathaniel Runolfsson | 518569490010 | IFSC00003 |
| Yvette Cooper | 841478410516 | IFSC00007 |
| Orion Glover | 001498029143 | IFSC00003 |

### Encountered a bug or want to suggest something?

If you come across any functional bug in the application or want to suggest the improvements, [file an issue](https://github.com/lucideus-repo/UnSAFE_Bank/issues) at this repository. We will look into it at the earliest. :)

### License

This project is using the GNU General Public License v3.0.

### Contributors

[Vibhav Dudeja](https://www.linkedin.com/in/vibhavd), [Tarun Kaushik](http://linkedin.com/in/tarun-kaushik-13827229), [Chetan Kumar](https://www.linkedin.com/in/chetan-daksh-0023b66a/), [Sahil Pahwa](https://www.linkedin.com/in/sahilpahwa1/)

### Owners

[Rubal Jain]

[Lucideus Inc.](https://www.lucideus.com)
