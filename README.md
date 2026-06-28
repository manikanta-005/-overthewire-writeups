# OverTheWire: Bandit Walkthrough (Levels 0–12)
Welcome to my walkthrough and write-ups for the foundational levels of the OverTheWire Bandit wargame.
## Table of Contents
* [Bandit Level 0 → Level 1](#bandit-level-0--level-1)
* [Bandit Level 1 → Level 2](#bandit-level-1--level-2)
* [Bandit Level 2 → Level 3](#bandit-level-2--level-3)
* [Bandit Level 3 → Level 4](#bandit-level-3--level-4)
* [Bandit Level 4 → Level 5](#bandit-level-4--level-5)
* [Bandit Level 5 → Level 6](#bandit-level-5--level-6)
* [Bandit Level 6 → Level 7](#bandit-level-6--level-7)
* [Bandit Level 7 → Level 8](#bandit-level-7--level-8)
* [Bandit Level 8 → Level 9](#bandit-level-8--level-9)
* [Bandit Level 9 → Level 10](#bandit-level-9--level-10)
* [Bandit Level 10 → Level 11](#bandit-level-10--level-11)
* [Bandit Level 11 → Level 12](#bandit-level-11--level-12)
---
### Bandit Level 0 → Level 1
* **Concept:** Learn what SSH is and how to use the Linux terminal to connect to a remote host.
* **Explanation:** **SSH (Secure Shell)** is a cryptographic network protocol used to securely connect to and manage a remote computer over an unsecured network. 
```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
OverTheWire: Bandit Write-up (Levels 0–12)

 Bandit Level 0 → Level 1 :
        1. you will know about what is ssh ? how it work how we connect to it using terminal in linux ?
    ans. ssh(secure shell) it is a cryptographic network used to securely connected to and manage a remote control computer over an unsecured network
    the default port number : 22 , we can change the port number according to our privacy.
    in linux we terminal to call ssh is like ssh user@domainname or ip address it is not a default port number the add -p and that port number so the comand look like
ssh username@domain name or i.p address -p port number like this the command work 
for level 0 the command is : "ssh bandit0@bandit.labs.overthewire.org -p 2220" it worked.
![alt text](file:///c%3A/Users/jvsma/AppData/Local/Packages/Microsoft.ScreenSketch_8wekyb3d8bbwe/TempState/Snips/Screenshot%202026-06-27%20215649.png)

where the password is given there only the password is bandit0 to access bandit level1
the password is hidden in that level i am used "ls" to list-directory to display how many files and directory are there inside on file is there
to see inside what is there i run a command name called 'cat'

![alt text](file:///c%3A/Users/jvsma/OneDrive/Pictures/Screenshots/Screenshot%202026-06-27%20220523.png)

Bandit Level 1 → Level 2 :
 after entering into bandit1 using the command name replacemthe user 'ssh bandit1@bandit.labs.overthewire.org -p 2220' later entering password which is shown in bandit 0 like : password you are looking for is: 6y2kwnwK6grgvwvpvLaa2T1cpFEKOhNR
 after entering into the bandit1 user first i have use command ls : list the file and directory what are there.
 at that moment we found the file name : '-'
in this we will going to know how to see spacial symbol used file how to see in that file
normally  the file have a name , but few spacial files they put symbols  like - that is a file name.

to access that type of files we use command name cat ./- why do not use cat - and what is ./--> ?
first why normal cat not use here when we type like cat - in linux terminal thing cat - he is typing some more it do not think that file is - that the command not work.
 now ./ it tells in your current path or directory there is a file like that it come in command so terminal will understand when we give ./- ohh - is not specail case it is a file located in this current directory 
 command : cat ./-
 the next level password came shown simpily.

 ![alt text](file:///c%3A/Users/jvsma/OneDrive/Pictures/Screenshots/Screenshot%202026-06-27%20222715.png)

      the password for next one is : PK8fYLZg2hnHSz83plBL1iEPKdD3QToB

Bandit Level 2 → Level 3 :
the task is The password for the next level is stored in a file called --spaces in this filename-- located in the home directory?
  first we will enter into into this level using command name ' ssh bandit2@bandit.labs.overthewire.org -p 2220' and later password the password is already i am given in above line

first as usual i am send a command ls to know inside how may are there i mean files or directory's are there in cureen directory 

![alt text](file:///c%3A/Users/jvsma/OneDrive/Pictures/Screenshots/Screenshot%202026-06-27%20224359.png)
     
later i used this command :'cat ./"--spaces in this filename--"'
why i use this one ony why not cat file name because in cat --spaces in this filename-- if i run command like this the terminall think --spaces this one type of file in it is another type of file, this another type of file like that it thinks they are multipile files but there will only one file with space so we will get error
to skip space to tell to terminal "" --> we are used this quotation so it will know that is toataly one file name and ./ is used to tell it is there in current directory
the output came like 
![alt text](file:///c%3A/Users/jvsma/OneDrive/Pictures/Screenshots/Screenshot%202026-06-27%20225705.png)

the password for next level is 7ZZ2LFrykP2zEyvBl4m3clcL7tGYJPME

Bandit Level 3 → Level 4 :

after entering into bandit3 using the command name replacemthe user 'ssh bandit3@bandit.labs.overthewire.org -p 2220' later entering password which is shown in bandit 2

the actual question find hidden file which i there at inhere directory
first i am do ls to known whether the inhere is there or not later i am used cd called change directory to inhere using like cd directoryname 
cd inhere
like that hope better to show image to get clarity.

![alt text](file:///c%3A/Users/jvsma/OneDrive/Pictures/Screenshots/Screenshot%202026-06-27%20230806.png)

see  later i type command ls inside is there any file or directory it shows nothing there as you can observe above fig  you can understand , because in question only it told the file is hidden
to catch hidden file the command that used is ls -al which display all files and directory even they are hidden the file name get reveal with that command.

to see hidden file password we use normal cat command 

![alt text](file:///c%3A/Users/jvsma/OneDrive/Pictures/Screenshots/Screenshot%202026-06-27%20231442.png)

where the pssword for next one is xzTXq1rDJQVVAzdv5cHq1TQytTWufAMq.

Bandit Level 4 → Level 5 :

hope you catch how to connect to ssh and using password to enter into bandit3 is ok i think for you if you face error at starting kindly check starting three level how i done 

in this we are going to find the password stored file based on their size , filetype and not execute based on these all we will find that file let start.

at first i am check using ls and theere is only on directory with the help of cd i have changed the directory and later i tried ls -al.
note at first i write command like ls - al it give error because -al in between no spae we have to give if we give like that we face error
after checking that i am  enter correct command name ls -al to see all hiden file and directory all

![alt text](file:///c%3A/Users/jvsma/OneDrive/Pictures/Screenshots/Screenshot%202026-06-27%20232422.png)

later the new command file ./* is used to display all file types in current directory that directory name is called inhere because in that only the password is saved to catch we know only one thing it is human readable 
that means it consistens of ascii-text 

![alt text](file:///c%3A/Users/jvsma/OneDrive/Pictures/Screenshots/Screenshot%202026-06-27%20233313.png)

later after runningthe command name  file ./* i havefound one file that consistence humanreadable and  i simpily just given command cat the file name which shown in file 

the password is came for next level the password :6C7h9GD8M6ai5nr7wo1RonrzFjj9yIrG

Bandit Level 5 → Level 6 :

The password for the next level is stored in a file somewhere under the inhere
the hint they given to me is human-readable , 1033 bytes in size , not executable

first based on given info first i am try to serch the directry of inhere it is present in the home directory using ls command i am checked where it is 
changed the directory using command cd later i am checked inside what are or how many files or directory present in the inhere directory


to find inside the inhere how many files and directory is used 
the command name is find . -type f 
in this we are going to discuss  the new command name called find it is used when soo many file and directoryes are there but that file property , size , type remeber then using find command you can get that file 

if we use file type here then they are so amy file names and directory are there you have  to go individuaily each directory and later search it take more time to readuce this time and fast and efficient we choose the command name called file uing this you can yound easily

where the coomand i used like 
 find . -type f --> to say how many directory inside the file are there

 ![alt text](file:///c%3A/Users/jvsma/OneDrive/Pictures/Screenshots/Screenshot%202026-06-27%20235557.png)

 like this it shown 
 later the next command i am tried is 
 where he given the file size is  1033 bits 
 the command i am writen as find . -size 1033c

 ![alt text](file:///c%3A/Users/jvsma/OneDrive/Pictures/Screenshots/Screenshot%202026-06-27%20235746.png)

 the file i found based on file size hence the password that i am got is

 bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
pXa26xhMWaC2SvDotA4r9EgZkulOeSBW

hope you understand how i get this

Bandit Level 6 → Level 7 :
here the password is saved some where across the server they given a hints like :
owned by user bandit7 , owned by group bandit6 , 33 bytes in size

so at first i search ls i see nothing in that directory later try ls -al to show hidden files they are shown

i am recognized the question in that one word the password is there in server means in root
to check all file from root i have given a command find / - size 33c hence the size of the file also given so add that poin and i am try to start 
here find / --> to check while entire root
while checking then so many permission denained things seen beace in root we have only few permission to overcross this error , i mean to ignore these permission denaied files we use 2>dev/null to ignore error
so the command name : find / - size 33c 2>dev/null

![alt text](file:///c%3A/Users/jvsma/OneDrive/Pictures/Screenshots/Screenshot%202026-06-28%20001501.png)

later i am again learn the question two times to get i dea n that there is line like
owned by user bandit7 and  owned by group bandit6
so for this i am written in command like :  find . -user bandit7 -group bandit6 -size 33c 2>/dev/null

where in question only given diretorly and 2>/dev/null to ignore reaming useless error

![alt text](file:///c%3A/Users/jvsma/OneDrive/Pictures/Screenshots/Screenshot%202026-06-28%20002035.png)

after combination all those condition one file is ther ewe are open by using the command name cat ./var/lib/dpkg/info/bandit7.password that file path simpily copy and paste inside that path that there is password which we want the password for next one is :Bmnnvf82KzQlfxgAI2d1zYbr1u9pr3E3

Bandit Level 7 → Level 8 :

this task is simple there is a file name called data.txt in that the password is there next to the word millionth means where the word there that place that passwd is available

at first i used the command name ls to see is there any files or directory around that path there i found data.txt file.

![alt text](<Screenshot 2026-06-28 091552.png>)

the command i used next one is :  grep -i "millionth" data.txt
soo for this i use grep -i commad it will search all the text where that next to the word millionth located   where -i is help to ignore the case sensitive
""-->what string or alphabet you want to search enter inside of this at last filename.
the password for next level :VR1ljMayciFxbnUokuQmJFw6QC9VKtub

Bandit Level 8 → Level 9 :

the question :  password for the next level is stored in the file data.txt and is the only line of text that occurs only once

so i use the command name called uniq and sort  these things are used mainly

as usual first  used ls command to get in this path that file is there or not later

![alt text](<Screenshot 2026-06-28 093831.png>)

the command name used : sort data.txt | uniq -u
used commands name sort and uniq
sort : it will arrange all lines in order.
uniq : it will give only uniq line repeated line will not display for that use -u to display uniq line and you want to know hom many time the line repeated use -c

question why can not you use uniq command only?
because uniq it will check right of the elemnt only if both are different  it left like that
Eg : a b a a --> there inside a file you use only uniq it will just check right side and tell the output  : a b a see still duplicate line is there but it cannot sense it 
so first we use sort arrange all elements in order like a a a b now doo uniq it will display uniq value with help of -u the ans b if you want to see how many times occured use uniq -c tell hom many times came here out out like  3 a 1 b like this ok

the password for next level : EjmOSvuAu7sGAHqHVcBDPirRe9T03kxl

Bandit Level 9 → Level 10 :

question : The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

soo according to given info i am use string here 
strings  = which change the text to read in humanreadable manner help to understand inside what is there 
the hint the password before "=" this equail sybol is there
so i am used grep to find  where that is it will search and display yo me

![alt text](<Screenshot 2026-06-28 093831-1.png>)

the password for next level : B0s2khmbT9u0geKuOoVGW3JZKhndE3BG

Bandit Level 10 → Level 11 :

question : The password for the next level is stored in the file data.txt, which contains base64 encoded data?

so here i used a single command name called base64 -d for decrypt and -e for encrypt 
command : base64 -d data.txt

![alt text](<Screenshot 2026-06-28 100224.png>)

the password for the next level :pYfOY6HwUsDj5rL9UvyhU7MCmv8vN5Ro

Bandit Level 11 → Level 12:
 
question :The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions
 
 it is also a simple task only he told that 13 positon move forward 
 in this field we are using tr command tr --> translate using this we are going to solve
 the command is used :sort data.txt | tr 'A-Za-z' N-ZA-Mn-za-m
 not only this youses in differn style to get know weather the password come or not it came
 ![alt text](<Screenshot 2026-06-28 102129.png>)

 the password for next leve i mean bandit12 :GROozWPO8QyN0mGrjUkID0WCYkZiQxrN

Bandit  Level 12:
see like this we are accessed the bandit 12 
