# Exercise - Connect using SSH

You will be using the SSH method in this exercise to connect to the virtual machine that was deployed in the last exercise.

> [!Note]
>
>This method is best suited for Windows and for learners working on other operating systems, can follow that method that best works for you

To do so, your first step will be to download PuTTY. PuTTY is an SSH and telnet client, developed originally by Simon Tatham for the Windows platform. PuTTY is open-source software that is available with source code and is developed and supported by a group of volunteers.

1. Download PuTTY, use the following link:
    [PuTTY](https://www.putty.org/)

2. Search for PuTTY on your PC and select to open it.

    ![Screenshot that shows the selections for configuring a breaking scenario.](/media/5.1-PuTTY-config.png)

    A small window called PuTTY Configuration will open with some fields to fill in.

3. Fill the first field, i.e., Host name (or IP address), go back to Azure portal and select the ‘Resource group’ under navigate section.  

4. From the resources, select on the Quorum Dev QuickStart resource you developed. Upon selecting, you will be able to visualise multiple sub-resources listed.  

5. Select the virtual machine resource from the list.

    ![Screenshot that shows the selections for configuring a breaking scenario.](/media/5.2-Public-IP-Address.png)

6. Copy the Public IP address from the essentials section.

    ![creenshot that shows the selections for configuring a breaking scenario.](/media/5.3-PuTTY-config-filled.png)

7. Paste the Public IP address in the Host Name field on the PuTTY configuration window.

    The other fields must be filled with the following details:

    ----------------------------------------------------------------------------------------------------
    |  |  |
    | :---: | :---: |
    | Host Name (or IP Address) | Paste the Public IP address from the Microsoft Azure portal |
    | Port | Leave it to the default value 22 |
    | Connection Type | Keep the default choice SSH and from the dropdown keep the default selection Telnet |
    |Close Window on exit | Keep the default option ‘Only on clean exit’ |

8. Select to Open

    ![creenshot that shows the selections for configuring a breaking scenario.](/media/5.4-PuTTY-security-alert.png)

    By clicking on Open, another window opens with a pop up named PuTTY Security Alert.

9. Click on Accept to close the pop-up window.

    ![Screenshot that shows the selections for configuring a breaking scenario.](/media/5.5-PuTTY-login.png)

    > [!NOTE]
    >
    > While entering the password, the terminal does not display any characters or asterisks as symbol. Hence, enter the password carefully even though there are no characters seen on the screen. The password still gets entered as we type. This is a security feature.

    PuTTY terminal asks for login username and password.  

10. Use the username and password that you used while deploying Quorum Dev QuickStart. Here quorumdev is used as sample.
    
    ![Screenshot that shows the selections for configuring a breaking scenario.](/media/5.6-virtual-machine-accessed.png)

<br>

Once you enter the username and password, you will get access to the Virtual Machine through which you will get the RPC endpoint in the next unit.
