![Image from file](/activity/devops/devops-title.png)

# DevOps CI/CD Pipeline Integration with Velocity
 
### Overview
This demo provides a look into how Velocity can integrate into a full/end-to-end DevOps CI/CD pipeline. Please familiarize yourself with the process by going through the following links.

| Links |
| ----- |
| [Demo Video][YT1] |
| [PowerPoint][YT1] |

![Image from file](/activity/devops/devops-demo-flow-30.png)

### How To Demo

#### Part 1: Setup - do this once for each demo
> 1. Reserve the Topology specified in this catalog.
> 2. SSH into any of the Development Environments in the Topology.
> 3. cd to `/home/spirent/projects/color-of-the-day` and issue the `git pull` command to ensure you have the latest code.
> 4. Keep the following tabs open in the browser:
>> * GitHub - [Link][GH]
>> * Jenkins - [Link][JN]
>> * Velocity Execution Page - [Link][VE]
>> * Internal Server - [Link][IS]
>> * External Server - [Link][ES]

#### Part 2: Positive Flow - Simulate a code change by developer
> 1. In the same Development Environment as in Part 1, cd to `/home/spirent/projects/color-of-the-day/webapp/src/main/webap` folder.
> 2. Issue `nano index.jsp` command to edit the file.
> 3. Change the color speicified in the file to something __other__ than RED.
> 4. Issue `Ctrl+X` and then `Y` to save file and exit editor.
> 5. Issue `git add .` to stage the file.
> 6. Issue `git commit -m "changed color"` to commit the file.
> 7. Issue `git push origin master` to push commited changes to master branch.

#### Part 3: Walk users through the entire CI/CD process to show what is happening
> 1. Show the new commit in github.
> 2. Show the new build being kicked-off in Jenkins - wait till Jenkins reaches Velocity integration.
> 3. Show the Runlist that is being executed - point the topology that is being used and walk through the tests that ran.
> 4. Go back to the Jenkins tab, and show how Velocity gave a __GO__ decision to Jenkins, and the Ansible tasks have started.
> 5. Go to the __internal__ server and show the new color as well as the new build number.
> 6. Go to the __external__ server and show the new color as well as the new build number.

#### Part 4: Negative Flow - Velocity gives a NO-GO verdict to Jenkins
> 1. Repeat __Positive Flow__ this time with the color `RED` to demo how Velocity issues __NO-GO__ verdict to Jenkins to abort the pipeline.
> 2. The flow will be the same as Positive Flow, except:
>> * The Runlist will fail
>> * Jenkins will abort the pipeline, and
>> * The color on the external server will be unchanged


[GH]: <https://github.com/spirentdemocloud/color-of-the-day>
[JN]: <http://ps-prod-tools2.spirenteng.com:8080/>
[VE]: <https://ps-production-velocity.spirenteng.com/velocity/reports/executions?period=PAST_1_YEAR&type=RUNLIST>
[IS]: <http://sdc-devops-docker-host.spirenteng.com:8080/webapp/>
[ES]: <http://3.133.135.84:8080/webapp/>
[YT1]: <https://www.youtube.com/watch?v=tWxziRYwnn4>
[RDP]: <https://10.142.16.222/terminal/#/?hostname=10.40.102.20&protocol=rdp&port=3389>
[S1]: <mailto:posevals@spirent.com>

