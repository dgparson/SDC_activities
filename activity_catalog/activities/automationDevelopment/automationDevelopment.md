
![Image from file](/activity/automationDevelopment/images/iTest.png)   

## **iTest - Rapid Automation Solution**

This is a shared environment that allows engineers to develop automation scenarios via iTest without the setup overhead. This activity will automatically create a user account and supports RDP for a good IDE user experience. This is open to all Spirent SEs and PS teams for demos and prototyping.

Owner: Mike Barfield

## Use case Overview

 1. Reserve topology at the bottom of the page - set to desired time (default is 4 hours)
 2. **FIRST TIME USERS ONLY** - Run automation to setup your user account: [link](https://ps-production-velocity.spirenteng.com/velocity/library/run/automation-assets/PCDE%2Fai_spirent_demo_assets%2Ftest_cases%2Ftasks%2Flinux%2FcreateNewUseriTestDev.fftc/parameters?rerun=false)
  
  -Note update parameter "username" with your windows login, expand the parameter list to expose the username (example: jsmith)
 3. RDP from the Velocity GUI using shortcut in topology or your preferred RDP tool to server listed in topology (example: ps-prod-tools.spirenteng.com)
 4. Login with your username/password (password = username)
  
  -Initial login ignore errors in your desktop environment (dismiss them they aren't important)
 5. Run iTest shell script located in your desktop environment:

Dismiss desktop errors:

![Image from file](/activity/automationDevelopment/images/ignore_desktop_error.png)

![Image from file](/activity/automationDevelopment/images/launch_itest.PNG)

![Image from file](/activity/automationDevelopment/images/run_itest_scripts.PNG)
 
 
 
 6.Set your workspace to match your user account (Note: workspace folder is created for your convenience)
  
  -Example: /home/jsmith/workspace
 
![Image from file](/activity/automationDevelopment/images/itest_workspace.png)


# Tips and Tricks

1. Use Git to manage your automation assets
  
  -Spirent Developer Community w/links to GitHub: [link](https://developer.spirent.com/)
  
  -Spirent internal GitLab: [link](https://git-ito.spirenteng.com/)
  
2. Free iTest training online, internal or external customer use, learn to automate: [link](https://support.spirent.com/SC_KnowledgeView?cid=null&id=TRN11001)
3. Get with your APT automation specialist to learn more about Git and this environment


# Videos

Video overview of Solution:  [link](https://spirent1.sharepoint.com/portals/hub/_layouts/15/PointPublishing.aspx?app=video&p=p&chid=53d4d0a3-c5de-4429-9f93-d131dea5d01a&vid=612a9f0f-7397-444c-b165-13f312d241d3)
    
# Automation IDE

![Image from file](/activity/automationDevelopment/images/itest_ide.png)
