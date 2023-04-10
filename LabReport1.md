# Lab Report 1
Welcome future **CSE 15L** students or future self in this guide I will guide you in logging into a course specific account on *iegn16*

---
## VS-CODE Installation  
---
 1.  [VS-Code download](https://code.visualstudio.com/download) This link will guide you in downloading **VS-CODE**
      * all major operation will be supported(mac OS and windows(PC's)
      * select download that best fits your operating system (see figure 1.1)
      * ![figure 1.1](<img width="1512" alt="Screenshot 2023-04-09 at 4 13 23 PM" src="https://user-images.githubusercontent.com/125671517/230800963-585b24f4-d716-415c-bfeb-273bfb3c9f56.png">
)	
  
      
 2. Open VS-CODE start up screens will differ(color...etc) depending on operation system(see figure 1.2 for an example)
      * ![figure 1.2(mac OS)](<img width="1512" alt="Visual Studio Code startup" src="https://user-images.githubusercontent.com/125671517/230800135-b65fc142-950b-45bf-8d90-68f2710e423c.png">
)	

---
## REMOTELY Connecting  
---
For **REFERENCE**- non Higlighed ```
                                 <code>
                                 ```is a command to remote server and highlighted(purple) is to own device
```  
$ command outputed to remote server 
```  
```ruby
$ command to own device 
```
                    
 3. To **SSH** into remote server **Open** a new terminal(*2 ways*)
      * ctrl + ` is a short cut to open a terminal
      * manually open it by scrolling up to **terminal** and clicking **New Terminal**(see figure 1.3)
      * ![figure 1.3](<img width="1504" alt="Screenshot 2023-04-09 at 4 24 43 PM" src="https://user-images.githubusercontent.com/125671517/230801491-2674c363-a037-4656-871b-1b0865a52a8e.png">
)	
 4. After type in command line(replace <username>)
```ruby
$ ssh cse15lsp23<username>@iegn6.ucsd.edu
```
 **Note**- After this line it will display a question (see figure 1.4) type
 ```ruby
 yes
 ```
 this message is prompted after connecting to a server for the first time.  
 
 ![figure 1.4](<img width="522" alt="Screenshot 2023-04-09 at 6 13 10 PM" src="https://user-images.githubusercontent.com/125671517/230806499-fe5b2cad-e685-477d-bfd5-a4aa6d9703ed.png">
)  
 
Then you should proceed in typing your password
 **Note**- you may question why isn't your password showing up. This is done on purpose for security measures when you type no characters will appear in command prompt.
 
 ---
  ## SIDE NOTE
 ---
 
 I enocunter many issues with reseting my course specific account password [RESET CSE 15L PASSWORD](https://sdacs.ucsd.edu/~icc/index.php). After Reseting my password and processing with Remotely connecting I could not login using my password it would the remote sever would output
```
permission denied
``` 
**OR**
```
connection issues
``` 
 
I recommend taking a screen shot of what the terminal outputed. Also discussing with your lab group if they as well encounter this issue. This can occur by putting "cse15<sp>l> instead of "sp" for spring. I inputed "wi" for winter can be inputed a mistake I did and any username misinputs can make this problem occur. I will try my best to guide you but mishaps along the way are inevitable for so many users logging in, issues will happen. So alert an IA or tutor of any issues that arise that you can not resolve. Even to have an IA sit with you along the process is completely fine.
 
 ---
 ## TRYING Commands
 ---
 Using the VS-CODE terminal type in commands in the termial and take note on what they produced and any errors if any
```ruby
cd~
```
```ruby
cd 
```
```ruby
ls -lat
```
```ruby
ls -a
```
```ruby
ls <directory> (replace with an aboslute path to another users account name remember the first 9 characters are the same for everyone)
```
```ruby
cp /home/linux/ieng6/cs15lsp23/public/hello.txt~/
```
```ruby
cat /home/linux/ieng6/cs15lsp23/public/hello.txt
```
**Note**- mess with the commands attempt to produce errors or different outcomes than group members take note what different outputs  
 produced between your lab members.
 
      

