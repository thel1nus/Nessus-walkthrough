
# Nessus THM Walkthrough by MalwareBorec.
### Disclaimer
----------
This Walkthrough will not give you correct answers right away, it will be a helping hand to get the answers yourself so you will learn something!
Everything here is explained in detail so you can easily understand it and move on. I'm also skipping task 1 and task 2 because there is nothing hard.

------------

### Table of contents
## [Task 3](https://github.com/malware-borec/Nessus/-walkthrough/README.md/task-3/)
- ##### [Navigation and scan types](https://github.com/malware-borec/Nessus/-walkthrough/README.md/navigation-and-scan-types)
- ##### [What is the name of the button which is used to launch a scan?](https://github.com/malware-borec/Nessus/-walkthrough/README.md/what-is-the-name-of-the-button-which-is-used-to-launch-a-scan)
- ##### [What side menu option allows us to create custom templates?](https://github.com/malware-borec/Nessus/-walkthrough/README.md/what-side-menu-option-allows-us-to-launch-a-scan)
- ##### [What menu allows us to change plugin properties such as hiding them or changing their severity?](https://github.com/malware-borec/Nessus/-walkthrough/README.md/)
- ##### [In the ‘Scan Templates’ section after clicking on ‘New Scan’, what scan allows us to see simply what hosts are alive?](Github.com)
- ##### [One of the most useful scan types, which is considered to be 'suitable for any host'?](https://github.com/malware-borec/Nessus/-walkthrough/README.md)
- ##### [What scan is specifically used for scanning Web Applications?](https://github.com/malware-borec/Nessus/-walkthrough/README.md)
- ## [Task 4](https://github.com/malware-borec/Nessus/-walkthrough/README.md)
- ##### [Create a new ‘Basic Network Scan’ targeting the deployed VM. What option can we set under ‘BASIC’ (on the left) to set a time for this scan to run? This can be very useful when network congestion is an issue.](https://github.com/malware-borec/Nessus/-walkthrough/README.md)
- ##### [Under ‘DISCOVERY’ (on the left) set the ‘Scan Type’ to cover ports 1-65535. What is this type called?](https://github.com/malware-borec/Nessus/-walkthrough/README.md)
- ##### [What 'Scan Type' can we change to under 'ADVANCED' for lower bandwidth connection?](https://github.com/malware-borec/Nessus/-walkthrough/README.md)
- ##### [After the scan completes, which 'Vulnerability' in the 'Port scanners' family can we view the details to see the open ports on this host?](https://github.com/malware-borec/Nessus/-walkthrough/README.md/)
- ##### [What Apache HTTP Server Version is reported by Nessus?](https://github.com/malware-borec/Nessus/-walkthrough/README.md)
## [Task 5 Scanning a Web Application!](https://github.com/malware-borec/Nessus/-walkthrough/README.md)
- ##### [What is the plugin id of the plugin that determines the HTTP server type and version?](https://github.com/malware-borec/Nessus/-walkthrough/README.md/)
- ##### [What is the file extension of the config backup?](https://github.com/malware-borec/Nessus/-walkthrough/README.md)
- ##### [What vulnerability is this application susceptible to that is associated with X-Frame-Options?](https://github.com/malware-borec/Nessus/-walkthrough/README.md)
### [Conclusion](https://github.com/malware-borec/Nessus/-walkthrough/README.md)


### Task 3
-----
###Navigation and scan types

So after we installed our Nessus and we are on the site, let's find out how to control it!

#### What is the name of the button which is used to launch a scan?

So after we installed the software we are on the main page. that should be looking like this:
![](https://cdn.discordapp.com/attachments/836685062316621834/836685456963010610/main_screen.png)

If you don't see it right away, maybe you are wondering where is it? Well, lets see the hint!
![](https://cdn.discordapp.com/attachments/836685062316621834/836685288498528326/hint.png)

Still not seeing it?
Well, let me show you the area!
![](https://cdn.discordapp.com/attachments/836685062316621834/836685504106987611/scanbutton.png)

If you find this area in this screenshot I'm sure you can find the scan button!

#### What side menu option allows us to create custom templates?

You may be wondering: what are even custom templates?
Custom templates are kind of created configs or saved settings that can be applied to any scanning. You will see the settings later in this room, let's just remember it's something like scan configurations for now.

So where to find it? Let's see the hint!
![](https://cdn.discordapp.com/attachments/836685062316621834/836685303573905428/hint2.png)

Recourses? Where are even those?
If you'd ask me, I didn't know really either.
Let me give you better hint, look at the left panel
![](https://cdn.discordapp.com/attachments/836685062316621834/836685441397948446/lpannel.png)

Well, there are plenty of options. Let's use the process of elimination!
So scans/All scans neither trash won't logically be the one what are we looking for. So let's not look at the folders panel anymore.
Then there are Resources and tenable. Tenable pannel will redirect us out, that's not what we are looking for.
Well now there are Policies or Plugin Rules, What I can tell you after you see this icon, you've got bingo!
![](https://cdn.discordapp.com/attachments/836685062316621834/836685425988862072/icona.png)

#### What menu allows us to change plugin properties such as hiding them or changing their severity?

Maybe you're again wondering what are plugins? Let's say it's kind of addons for scanning that can discover server versions for an example, and you can turn them on and off, even customize them. More of that will be discovered later in this room.

Well, let's look at the hint.

![](https://cdn.discordapp.com/attachments/836685062316621834/836685317171970058/hint3.png)

Resources, wasn't it here one time already?
You are absolutely right! And it's in the same place as previously, left panel.
I assure you can find it by the pannels name!

#### In the 'Scan Templates' section after clicking on 'New Scan', what scan allows us to see simply what hosts are alive?

Hmm, look at that question. *New Scan* 
New scan pretty familiar right? Well, take a look back to the first question!
After clicking that button you're being brought to the page of 'Scan Templates'. That's exactly what we're looking for right?
Well from here you will see something like this:
![](https://cdn.discordapp.com/attachments/836685062316621834/836685516027592714/scan_types.png)

From here try searching for the 'hosts and alive'. If you did the Nmap room then you should know the -sP option (ping scan)
The Nmap will use a ping scan to discover if the host is responding and if it's up. This works on the same Principe!
Well, search for the template that seems like it! I'm sure you'll find it
*My hint*
Search for keyword host.

#### One of the most useful scan types, which is considered to be 'suitable for any host'?

This scan template is in the Vulnerabilities category in Scan Templates. 
Search for the keyword 'suitable for any host' and I'm sure you can find it!

#### What scan allows you to 'Authenticate to hosts and enumerate missing updates'?

Again, search for the Authenticate to hosts and enumerate missing updates in the Scan Templates Vulnerabilities category.

#### What scan is specifically used for scanning Web Applications? 

Look for the 'Web Applications in Scan Templates Vulnerabilities category.
My hint:
Look at the title of the template, not the description.


### Task 4

To run this we need to have the machine running, and start a scan.
The scan template is called 'Basic Network scan' and you can start it by clicking on it.
After you click on it you're bringing on configuration site and from there you can do these tasks:
![](https://cdn.discordapp.com/attachments/836685062316621834/836685229971865660/Configmenu.png)

#### Create a new 'Basic Network Scan' targeting the deployed VM. What option can we set under 'BASIC' (on the left) to set a time for this scan to run? This can be very useful when network congestion is an issue.


Let's break the question down.
So we did already create the Virtual machine, so we can ignore that part.
What option can we set under 'BASIC' (on the left)
If we look on the left we see a pannel of options, and the first option is the specified 'BASIC'
![](https://cdn.discordapp.com/attachments/836685062316621834/836685205954625586/basicpannel.png)

Now we've got specification under it, so what's the option? I'm sure you can figure it out easily now.

#### Under 'DISCOVERY' (on the left) set the 'Scan Type' to cover ports 1-65535. What is this type called?

If we look at the left panel again, we can see there are more categories than settings.
From that, we can find the DISCOVERY option that is specified in the option.
After clicking on that, we can see this:
![](https://cdn.discordapp.com/attachments/836685062316621834/836685274146537522/discovery.png)
There's also one specification in the question 'Scan Type'.
See it there? Great.
Now choose the option that fits the best to cover all ports from 1 to 65535.

#### What 'Scan Type' can we change to under 'ADVANCED' for lower bandwidth connection?

Again on the left panel, we can see the option called: 'ADVANCED'
After clicking on that, we can see this:
![](https://cdn.discordapp.com/attachments/836685062316621834/836685164020629544/advanced.png)
So let's choose the right Scan type.

Make sure you've got all the specified settings selected and hit Scan!
After we launch the scan you will wait about 5/10 minutes for the scan to complete. The speed of the scan depends on your internet connection and hardware.

So we have the scan completed and it should look something like this:
results 1

#### After the scan completes, which 'Vulnerability' in the 'Port scanners' family can we view the details to see the open ports on this host?

So here from the panel we will click into the Vulnerabilities redirect
![](https://cdn.discordapp.com/attachments/836685062316621834/836685523606044702/vurns.png)

from here we are looking for details of the ports. 
If you click any of these it will show the basic information about the found Vulnerability.
My hint:
Look at the 'Family' category and search for something related to 'ports'.


####  What Apache HTTP Server Version is reported by Nessus?

From here we will navigate in the Vulnerabilities tab again.
We need to find information about the HTTP server version. 
So now look for the 'version' or 'HTTP' scan. I'm sure you can find this one pretty easily.


### Task 5 Scanning a Web Application!
----
From here we will run the scan on the same Virtual machine as before,
but 'Web Application Tests'. If you don't know how to run a scan, refer to Task 4 explanation.
![](https://cdn.discordapp.com/attachments/836685062316621834/836685559224205352/webscan.png)
#### What is the plugin id of the plugin that determines the HTTP server type and version?


HTTP Server Type and Version, let's check out our vulnerabilities tab!
![](https://cdn.discordapp.com/attachments/836685062316621834/836685532137259028/vurns2.png)
Hmm, it isn't there right?
Well, it's hidden behind the other folder! If it has the folder icon it means more vulnerabilities in one scan.
After you find the right folder and scan info, how do we obtain the ID?
It's on the right side under Plugin Details.
Details.png

#### What authentication page is discovered by the scanner that transmits credentials in cleartext?

Let's see the hint.

![](https://cdn.discordapp.com/attachments/836685062316621834/836685329351704576/hint4.png)

Security of low, what does that mean?
Let's see the vulnerabilities tab real quick.
![](https://cdn.discordapp.com/attachments/836685062316621834/836685546670784542/vurnsss.png)
This means that Low will have the color green.
But there isn't anything that has something like that next to it.
Well, there has to be one, and it's hidden again!
![](https://cdn.discordapp.com/attachments/836685062316621834/836685468133097533/mixed.png)
The purple color or 'Mixed' tab means there are multiple types of vulnerabilities.
If there isn't Green color anywhere it has to be in it.
![](https://cdn.discordapp.com/attachments/836685062316621834/836685481230991370/ningo.png)

Bingo!
Well, now we have to find the authentication page.
*My hint:*
Look at the output.

#### What is the file extension of the config backup?

The hint here says:
![](https://cdn.discordapp.com/attachments/836685062316621834/836685344896057374/hint5.png)

Let's look at the Medium (orange) tabs then.
We are looking for backup, and I'm pretty sure you already see the right one.
To see the answer, you need to take a look at the output again.

#### Which directory contains example documents? (This will be in a php directory) 

And the hint is:
![](https://cdn.discordapp.com/attachments/836685062316621834/836685357156139050/hint6.png)
Browsable directories tab, let's enroll in!
We are looking for example documents, and we can already see some relative paths there!
![](https://cdn.discordapp.com/attachments/836685062316621834/836685256580661289/dirs.png)

Let's choose the right one.
Note:
Make sure you answer the message without the HTTP information.



#### What vulnerability is this application susceptible to that is associated with X-Frame-Options?

Let's see the hinty hint:
![](https://cdn.discordapp.com/attachments/836685062316621834/836685377544257566/hint7.png)

Medium - orange tabs, let's take a look at them.
So we are looking for directly exploitable vulnerability. 
One of them is already in the tab name.
Right after we clicked on the right one, we can see the X-Frame written in Description.
Now we are in the right place!

### Conclusion

I hope you learned something and you like the non-direct answer format!
If you liked this Walkthrough make sure to star the Repository and follow me for more Walkthroughs.
Something is wrong in here or do you need help to explain something further? Feel free to contact me on Discord - @Malware Borec#6385
