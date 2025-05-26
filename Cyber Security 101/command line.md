# Command Line
Learn the command line and MS PowerShell in Windows by practising various essential commands. Then, discover the use of Bash in the Linux OS.

# Windows Command Line
 graphical user interface (GUI)
 command-line interface (CLI)
 
**Lower resource usage:** CLIs require fewer system resources than graphics-intensive GUIs. In other words, you can run your CLI system on older hardware or systems with limited memory. If you are using cloud computing, your system will require lower resources, which in turn will lower your bill.

**Automation:** While you can automate GUI tasks, creating a batch file or script with the commands you need to repeat is much easier.

**Remote management:** CLI makes it very convenient to use SSH to manage a remote system such as a server, router, or an IoT device. This approach works well on slow network speeds and systems with limited resources.

**ver** command to determine the operating system (OS) version
 
**systeminfo** command to list various information about the system such as OS information,

# Network Configuration
You can check your network information using **ipconfig**. The terminal output below shows our IP address, subnet mask, and default gateway.
![image](https://github.com/user-attachments/assets/bcd48039-4226-46d8-8e98-a7fb8de5cbb2)

Network Troubleshooting
One common troubleshooting task is checking if the server can access a particular server on the Internet. The command syntax is **ping target_name**
Inspired by ping-pong, we send a specific ICMP packet and listen for a response. If a response is received, we know that we can reach the target and that the target can reach us.

![image](https://github.com/user-attachments/assets/ee079d89-a239-401f-b28b-1288169c85d7)

**tracert**, which stands for _trace route_. The command tracert target_name traces the network route traversed to reach the target.

**nslookup**. It looks up a host or domain and returns its IP address. The syntax nslookup example.com will look up example.com using the default name server

![image](https://github.com/user-attachments/assets/4c1dcc67-970d-4538-9de7-c9036adcaeaa)

**netstat**. This command displays current network connections and listening ports. 
A basic netstat command with no arguments will show you established connections

![image](https://github.com/user-attachments/assets/602ef059-30f3-40f0-bd1b-623264939702)

If you are curious about the other options, you can run netstat -h, where -h displays the help page. We opted for the following options:

**-a** displays all established connections and listening ports
**-b** shows the program associated with each listening port and established connection
**-o** reveals the process ID (PID) associated with the connection
**-n** uses a numerical form for addresses and port numbers

We combine these four options and execute the netstat -abon command. 
![image](https://github.com/user-attachments/assets/553ae649-6008-432e-abc4-0d95b94c65ea)

# File and Disk Management
Working With Directories
You can use **cd** without parameters to display the current drive and directory. It is the equivalent of asking the system, where am I?

![image](https://github.com/user-attachments/assets/68bcc0a1-0225-4e01-a466-f2c79650a4d0)

You can view the child directories using **dir**.

![image](https://github.com/user-attachments/assets/a3c99284-3ae6-4b0d-8286-2b43206c70b4)

# Windows PowerShell
PowerShell is a cross-platform task automation solution made up of a command-line shell, a scripting language, and a configuration management framework.

In programming, an object represents an item with properties (characteristics) and methods (actions). For example, a car object might have properties like Color, Model, and FuelLevel, and methods like Drive(), HonkHorn(), and Refuel()

Get-Content: Retrieves (gets) the content of a file and displays it in the console.
Set-Location: Changes (sets) the current working directory.

To list all available cmdlets, functions, aliases, and scripts that can be executed in the current PowerShell session, we can use **Get-Command**. It’s an essential tool for discovering what commands one can use.

For each CommandInfo object retrieved by the cmdlet, some essential information (properties) is displayed on the console. It’s possible to filter the list of commands based on displayed property values. For example, if we want to display only the available commands of type “function”, we can use -CommandType "Function"

**Get-ChildItem** lists the files and directories in a location specified with the -Path parameter.

If no **Path** is specified, the cmdlet will display the content of the current working directory.




































