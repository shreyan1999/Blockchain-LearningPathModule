# Quorum QuickStart - Setting up blockchain

In the last unit, you connected to the virtual machine. In this unit, you will setup blockchain using a few commands. Let’s discuss about the steps to run the virtual machine and get RPC endpoint in this unit.

To run the virtual machine, you will need to install Quorum Developer Quickstart.  

There are two ways to install this setup on your local machine. You can follow any one of the methods and both will have the same result.

<br>

**Method 1:** 

*Step-1:* Enter the following code line in the PuTTY terminal once you have logged in:

	`npx quorum-dev-quickstart`

*Step-2:* You will be asked a few questions in the process of installation. Answer the questions based on what you want in your installation.

> [!Note]  
>
>The questions which are asked as follows:
>
>- Which Ethereum client would you like to run? Default:[1]
>    1. Hyperledger Besu
>    2. GoQuorum
>- Do you want to try out Codefi Orchestrate? [Y/n]
>- Do you want to try out Quorum Key Manager? [Y/n]
>- Do you wish to enable support for private transactions? [Y/n]
>- Do you wish to enable support for logging with Splunk or ELK (Elasticsearch, Logstash &      Kibana)? Default: [1]
>    1. None
>    2. Splunk
>    3. ELK
>You will have to answer these questions in the form of choice selection by entering the number of selection or in the form of answering Yes or No by entering the alphabets Y or N.
>
>To know more before you answer these questions, click on the following links below:
>
>- [Hyperledger Besu](https://github.com/ConsenSys/quorum-dev-quickstart/blob/master/files/besu/README.md);
>- [GoQourum](https://github.com/ConsenSys/quorum-dev-quickstart/blob/master/files/goquorum/README.md);
>- [Codefi Orchestrate](https://github.com/ConsenSys/quorum-dev-quickstart/blob/master/files/orchestrate/README.md);
>- [Quorum Key Manager](https://github.com/ConsenSys/quorum-dev-quickstart/blob/master/files/quorum-key-manager/README.md)

<br>

**Method 2:**  

*Step-1:* To avoid answering all the questions one by one and directly get to the next steps in the setup, run the following code in the terminal: 

    `npx quorum-dev-quickstart --clientType besu --outputPath ./quorum-test-network --monitoring default --privacy true --orchestrate false --quorumKeyManager false`

In our setup, we have used method 2. You can choose to work with any method, since both have same result.  

To know in detail about what you have installed, click on the following link:
[Quorum Developer Quickstart](https://github.com/ConsenSys/quorum-dev-quickstart)

![Screenshot that shows the selections for configuring a breaking scenario.](/media/6.1-entering-directory.png)

<br>
*Step-2:* Once you have installed the Quorum Developer Quickstart, enter the directory ‘quorum-test-network’. To do so, enter the following code in the terminal:

    `cd quorum-test-network`

*Step-3:* Upon entering the directory, run the following command to run the virtual machine and obtain an RPC endpoint:

	`./run.sh`
<br>

![Screenshot that shows the selections for configuring a breaking scenario.](/media/6.2-running-command-part1.png)

![Screenshot that shows the selections for configuring a breaking scenario.](/media/6.3-running-command-part2.png)

Once the process is completed, you have successfully activated your RPC endpoint which is in the form:  <http://[IP]:8545>, while the IP address is taken from the azure portal.  

The RPC endpoint we obtained in our demo is as follows: <http://52.174.48.168:8545>

![creenshot that shows the selections for configuring a breaking scenario.](/media/6.4-Public-IP-Address.png)

<br>
The part of the RPC endpoint which is marked in red, is copied from the Public IP Address from the Azure portal.