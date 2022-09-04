# Cloud-note

# My learning track in cloud Engineering

----
# Cloud 
## Linux


Processes are applications that are currently running 
The request that processes make are called sys-call also called system calls 

There are other places to learn more on the north canal links below in Altschool Africa video 3

Installing Linux 
You need hosting machine also called bare metals eg are your desktop 
Laptop and server, embedded devices and so on, in this case your OS will be dealing with physical hardware 

VM also called Virtual machine- they use visualization software to emulate hardware 
Let say you have a windows OS on your system and you want Linux too 
You can install VM and install Linux on the VM 
To use both windows on your laptop and Linux on VM 
You can have a lot of VM on the host machine and this way sharing nothing with the host machine except if you configure it to share resources 
Types of visualization software or virtual machines 
*Most common are virtual box and VMware 
 
Cloud Platforms like AWS (Amazon web services )and GCP (google computing platform)
Uses visualization software to spin up all the VMs you buy online and host your services 
So your fav website might be running on a VM in a cloud platform 

Container 
Container on the other hand allows you to isolate different workload with everything they need 

For example 
Everything they need to run 
An application wants to run a Java application. 
What it needs is Java compiler and Java run time 
So a container get everything it needs to run 
It’s not like windows that comes with everything things you need and what you don’t need 
But in the case of a container just what you need are what comes with it nothing else 
Unlike VM- containers are not totally isolated from the host 
They still share resources with the system 

Next is how to get the operating system software 
The distribution is done via image before we use CDs 
Which can be ISO images containing installation files or VM images which are often already installed OS packed for easy deployment in a VM somewhere that you have installed 
Unlike ISO images VM images contain contain the VM configuration to get the OS running not just the Installation files itself 
All you need to do is import and viola you’re running 
You can build your own installation from source code and deploy but you must know what you’re doing to do that 
You can get images from different places just be careful where you download from 
Verify your download 
Most distribution website provide an hashes(checksums) -it is like a code for you to verify the download you have done against 
So if it differs it means something is wrong or something is different in installation and if it is the same that means there’s nothing wrong, probably something has been edited or some new code has been added or something else.
Ubuntu part of Debian family 
20.04LTS and this means Long Term support 
Ubuntu releases every 6months 
4th and 10th month 
But it is only those that have LTS that have  long term support that for update for security and all other things 
But other ones without LTS get outdated.

We need set up a VM(an emulator) called virtual box and it software called vagrant


Linux shell and command 
The prompt often comes as a dollar sign in the terminal and is powered by Linux shell and Linux shell is the program that allows you to interact with the kernel 
When you issue a command shell processes and pass this command where necessary and make syscalls to the kernel and provide output to the user 
Types of Linux shell

1. bash aka Bourne again shell-it originated from SH which is short for borne shell 

2. ZSH for Mac users 

Knowing where you’re is crucial on Linux shell 
Two of the most common location are the ROOT directory (/)which is often 

represented by forward slash and the HOME directory of the current login user which is represented by the $HOME 

you can also add PWD 
Remove is delete in Linux 

The key folders we will use 
1. /home where all user home directory are located 

2. /mnt - where all files system are mounted 

3. /var /log-this shows various source on the system, it document on your system, keeping folders 

# Linux commands
Some command can be on their own while others need argument
Some command esp the one with output can be generating files and you can use them to send message to another place 

## Examples

1.  $uname-with this you can identify what kind of operating system you’re using, the version of Linux and others and Uname -A gives me more detail about my OS 
When you’re doing scripting you will need to know what kind of OS to use so this is important.




2. $date -You can check your system date and time 
Uptime tells you how long your system have been up probably something happen and it restarted 
You should know how long you have been using it 
An uptime is also an indication that everything is going fine
You might hear people say their server is 99.999 percent uptime it means the system has been on all the time and it only goes off maybe when an update wants to happen 

**Ass**

*Learn how to set time zones*


3. $whomai- You get to know who is the current login user

4. $export VAR =VALUE 
you can set a variable in the terminal with export variable 

5. $echo VAR 
And display the variable using echo command 
Like echo the content of this variable, echo this text and the rest 
You can use echo to display the lateral values 

6. $ps
You can view running managers called processes with ps 

7. $top
You can use top to get the information about that processes running 

8. $df-h
This tells you more about the storage that you have 

## Moving around linux 
1. PWD -Present working directory 


2. Cd change directly 


3. ls list shell 


4. ls -l list more details

