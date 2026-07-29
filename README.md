# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1
```
chanchal singhvi
c.k. shukla
s.n. dasgupta
sumit chakrobarty
^d
```
## OUTPUT:
<img width="377" height="150" alt="image" src="https://github.com/user-attachments/assets/077b7a9b-88ac-491f-b814-6a41da64abc3" />

cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```
## OUTPUT:
<img width="467" height="196" alt="image" src="https://github.com/user-attachments/assets/2d51ef67-0930-4106-83bd-b730b16695ab" />

### Display the content of the files
cat < file1
## OUTPUT:
<img width="490" height="190" alt="image" src="https://github.com/user-attachments/assets/cc74891e-6371-4aca-8cf9-1aa73a96fb7e" />

cat < file2
## OUTPUT:
<img width="405" height="146" alt="image" src="https://github.com/user-attachments/assets/e3857e72-cce1-4e91-afc2-562416bacd71" />

# Comparing Files
cmp file1 file2
## OUTPUT:
 <img width="382" height="76" alt="image" src="https://github.com/user-attachments/assets/00ed7f99-7a3e-4cad-9271-f413aee50e49" />

comm file1 file2
 ## OUTPUT:
<img width="442" height="296" alt="image" src="https://github.com/user-attachments/assets/fe0c232f-1cac-4c7e-82b3-8f2d6d4ff351" />

diff file1 file2
## OUTPUT:
<img width="442" height="325" alt="image" src="https://github.com/user-attachments/assets/7f395d23-1bee-442c-b8d2-bd68cf3f3013" />

### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
## OUTPUT:
<img width="407" height="107" alt="Screenshot 2026-07-27 085725" src="https://github.com/user-attachments/assets/97319438-c4b2-481d-bf94-632cb35ab4b5" />

cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```
## OUTPUT:
<img width="421" height="180" alt="Screenshot 2026-07-27 085851" src="https://github.com/user-attachments/assets/d6258cbd-8e43-47d4-b129-437a388c124f" />

cut -c1-3 file11
## OUTPUT:
<img width="405" height="102" alt="image" src="https://github.com/user-attachments/assets/6bdc356b-0548-40d2-b47d-61fa947c1d6c" />

cut -d "|" -f 1 file22
## OUTPUT:
<img width="405" height="125" alt="image" src="https://github.com/user-attachments/assets/4133fba4-252a-4190-a227-592c0dcea257" />

cut -d "|" -f 2 file22
## OUTPUT:
<img width="392" height="150" alt="image" src="https://github.com/user-attachments/assets/e0bfdeee-9708-4e66-8a3c-a7be59204aab" />

cat < newfile 
```
Hello world
hello world
^d
````
## OUTPUT:
<img width="472" height="117" alt="image" src="https://github.com/user-attachments/assets/6d7622bc-7c0b-493a-a904-0d3d57dc62ac" />

cat > newfile
```
Hello world
hello world
 ```
grep Hello newfile 
## OUTPUT:
<img width="435" height="147" alt="image" src="https://github.com/user-attachments/assets/aa611e98-e824-4f9f-abf7-20701ca6d2ad" />

grep hello newfile 
## OUTPUT:
<img width="425" height="81" alt="image" src="https://github.com/user-attachments/assets/302c6cb6-443d-438e-b0f5-52536af40b54" />

grep -v hello newfile 
## OUTPUT:
<img width="390" height="127" alt="image" src="https://github.com/user-attachments/assets/41b49670-bb16-4a71-946c-1e5fd8591071" />

cat newfile | grep -i "hello"
## OUTPUT:
<img width="420" height="123" alt="image" src="https://github.com/user-attachments/assets/92f59a02-c7a6-453b-9a69-7cbf67e45063" />

cat newfile | grep -i -c "hello"
## OUTPUT:
<img width="387" height="71" alt="image" src="https://github.com/user-attachments/assets/a7281396-5f44-4691-a507-ee1c3bd262d0" />

grep -R ubuntu /etc
## OUTPUT:
<img width="871" height="720" alt="image" src="https://github.com/user-attachments/assets/fbc0aa4b-41ce-4f76-a683-fe7a74224285" />

grep -w -n world newfile   
## OUTPUT:
<img width="412" height="95" alt="image" src="https://github.com/user-attachments/assets/897158ac-090c-4525-8aea-1dca2f61d9be" />

cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```
## OUTPUT:
<img width="458" height="182" alt="image" src="https://github.com/user-attachments/assets/1525f28b-db86-4af2-a7dc-32d2645eb4fe" />

cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
 ```
## OUTPUT:
<img width="397" height="182" alt="image" src="https://github.com/user-attachments/assets/5c00c439-5a71-46e1-8dc8-682c174b2e3c" />

egrep -w 'Hello|hello' newfile 
## OUTPUT:
<img width="397" height="100" alt="image" src="https://github.com/user-attachments/assets/e8c2e3e5-3cac-4088-815f-fc64a3570e33" />

egrep -w '(H|h)ello' newfile 
## OUTPUT:
<img width="382" height="97" alt="image" src="https://github.com/user-attachments/assets/0a99c3a0-8ab6-445b-a5ed-d280589b4db7" />

egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT:
<img width="458" height="102" alt="image" src="https://github.com/user-attachments/assets/b362fc44-efa0-4f7d-af0e-650d76f1a225" />

egrep '(^hello)' newfile 
## OUTPUT:
<img width="400" height="77" alt="image" src="https://github.com/user-attachments/assets/59244541-e77d-4e5b-a465-60360427a00b" />

egrep '(world$)' newfile 
## OUTPUT: 
<img width="382" height="100" alt="image" src="https://github.com/user-attachments/assets/e236661f-adee-4963-b875-05dc62697a3b" />

egrep '(World$)' newfile 
## OUTPUT:
<img width="443" height="81" alt="image" src="https://github.com/user-attachments/assets/f18009a0-2a21-4368-9e3f-eefecfb9ee92" />

egrep '((W|w)orld$)' newfile 
## OUTPUT:
<img width="472" height="126" alt="image" src="https://github.com/user-attachments/assets/367ff5de-725e-4edc-8365-a7f1fe3fd476" />

egrep '[1-9]' newfile 
## OUTPUT:
<img width="377" height="71" alt="image" src="https://github.com/user-attachments/assets/cd4bf9c0-5411-4198-aba2-9eac7c55824d" />

egrep 'Linux.*world' newfile 
## OUTPUT:
<img width="405" height="75" alt="image" src="https://github.com/user-attachments/assets/bef08788-2f60-4fff-8225-82f00693bf7b" />

egrep 'Linux.*World' newfile 
## OUTPUT:
<img width="405" height="75" alt="Screenshot 2026-07-27 094104" src="https://github.com/user-attachments/assets/cd897df6-3cc9-415c-a220-fd5b1b7bfb97" />

egrep l{2} newfile
## OUTPUT:
<img width="392" height="100" alt="image" src="https://github.com/user-attachments/assets/9685f46a-9e39-4d72-acc5-42aacdea1905" />

egrep 's{1,2}' newfile
## OUTPUT:
<img width="396" height="127" alt="image" src="https://github.com/user-attachments/assets/b6a32606-f2e2-47a8-bf44-b0447177d20e" />

cat > file23
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
1003 | Joe |  7000 | Developer
1001 | Ram | 10000 | HR
^d
```
## OUTPUT:
<img width="432" height="256" alt="image" src="https://github.com/user-attachments/assets/1dbf0a97-d507-4dea-af72-e66e970e6121" />

sed -n -e '3p' file23
## OUTPUT:
<img width="415" height="81" alt="image" src="https://github.com/user-attachments/assets/73726399-b66d-41b4-935a-3c5e2a728627" />

sed -n -e '$p' file23
## OUTPUT:
<img width="380" height="75" alt="image" src="https://github.com/user-attachments/assets/f7f0cea3-7c62-4230-8dcd-2ae36f2d6854" />

sed  -e 's/Ram/Sita/' file23
## OUTPUT:
<img width="428" height="265" alt="image" src="https://github.com/user-attachments/assets/9d09250a-def0-45d1-9889-06ddebbe7564" />

sed  -e '2s/Ram/Sita/' file23
## OUTPUT:
<img width="427" height="277" alt="image" src="https://github.com/user-attachments/assets/76298102-2470-4451-88c5-1d266cae21ff" />

sed  '/tom/s/5000/6000/' file23
## OUTPUT:
<img width="407" height="270" alt="image" src="https://github.com/user-attachments/assets/aff5e657-42bb-4c64-9524-9c1a5f6bec29" />

sed -n -e '1,5p' file23
## OUTPUT:
<img width="417" height="192" alt="image" src="https://github.com/user-attachments/assets/757a809e-446f-4fe5-a1ce-c6f733083ec8" />

sed -n -e '2,/Joe/p' file23
## OUTPUT:
<img width="398" height="125" alt="image" src="https://github.com/user-attachments/assets/2d104af1-5205-443c-923d-394a88a0675d" />

sed -n -e '/tom/,/Joe/p' file23
## OUTPUT:
<img width="400" height="96" alt="image" src="https://github.com/user-attachments/assets/82b251aa-ae01-4b44-a510-624ae478b0cd" />

seq 10 
## OUTPUT:
<img width="388" height="297" alt="image" src="https://github.com/user-attachments/assets/7cc3a3c5-fae8-4a81-a37c-be84c45de3f6" />

seq 10 | sed -n '4,6p'
## OUTPUT:
<img width="375" height="127" alt="image" src="https://github.com/user-attachments/assets/978e462a-9e6c-4baa-931f-da7941b7afed" />

seq 10 | sed -n '2,~4p'
## OUTPUT:
<img width="385" height="123" alt="image" src="https://github.com/user-attachments/assets/fceb2646-c101-498c-8c44-6cc3571649d0" />

seq 3 | sed '2a hello'
## OUTPUT:
<img width="405" height="147" alt="image" src="https://github.com/user-attachments/assets/9aa015d0-7ec0-4cf4-9e8d-0d47ccf8ba12" />

seq 2 | sed '2i hello'
## OUTPUT:
<img width="370" height="125" alt="image" src="https://github.com/user-attachments/assets/6f4e404b-ae20-44b1-94de-b90a97ce9cc3" />

seq 10 | sed '2,9c hello'
## OUTPUT:
<img width="352" height="125" alt="image" src="https://github.com/user-attachments/assets/bcf5a1b1-3119-41b3-9394-7e8ae902bc99" />

sed -n '2,4{s/^/$/;p}' file23
## OUTPUT:
<img width="366" height="125" alt="image" src="https://github.com/user-attachments/assets/6953fcb6-556b-4ff2-a4c1-2ddca70a9f67" />

sed -n '2,4{s/$/*/;p}' file23
## OUTPUT:
<img width="387" height="117" alt="image" src="https://github.com/user-attachments/assets/41bc2816-509d-46cd-ab83-222fdad2c035" />

#Sorting File content
cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
sort file21
## OUTPUT:
<img width="406" height="380" alt="image" src="https://github.com/user-attachments/assets/cbb53029-3a57-465e-bde5-7ddec3c887c3" />

cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
uniq file22
## OUTPUT:
<img width="436" height="401" alt="image" src="https://github.com/user-attachments/assets/42291110-63a1-42ae-8579-8583b76f5f46" />

#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT:
<img width="437" height="262" alt="image" src="https://github.com/user-attachments/assets/a2b48789-4ce7-465c-9b60-88c441ca5711" />

cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^dcat < urllist.txtcat < urllist.txt
 ```
cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
cat urllist.txt | tr -d ' '
 ## OUTPUT:
<img width="455" height="427" alt="image" src="https://github.com/user-attachments/assets/cf72585b-223a-4238-a1a3-7e631cd0b16a" />
 
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT
<img width="492" height="107" alt="image" src="https://github.com/user-attachments/assets/962445ee-91d4-4d04-b24a-a86661f6b9cc" />

#Backup commands
tar -cvf backup.tar *
## OUTPUT:
<img width="391" height="277" alt="image" src="https://github.com/user-attachments/assets/23baf387-7068-40ab-9dd7-4b184a9a0207" />

mkdir backupdir
mv backup.tar backupdir
cd backupdir
tar -tvf backup.tar
## OUTPUT:
<img width="800" height="447" alt="image" src="https://github.com/user-attachments/assets/224c8081-d7ab-4c26-803b-6066683a2ce1" />

tar -xvf backup.tar
## OUTPUT:
<img width="483" height="272" alt="image" src="https://github.com/user-attachments/assets/7bae2b2f-0d6a-49a2-8344-c1fa5a1e7d85" />

gzip backup.tar
ls .gz
## OUTPUT:
 <img width="567" height="125" alt="image" src="https://github.com/user-attachments/assets/19ec6132-e8f2-4639-97b9-9681f21048ac" />

gunzip backup.tar.gz
## OUTPUT:
<img width="505" height="50" alt="image" src="https://github.com/user-attachments/assets/b6a14517-12e1-46b9-bf3e-d436db83667d" />

# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT:
<img width="522" height="223" alt="image" src="https://github.com/user-attachments/assets/97e7354e-0723-4d9b-a7ce-354533cdfdea" />

cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```
cat herecheck.txt
## OUTPUT:
<img width="496" height="271" alt="image" src="https://github.com/user-attachments/assets/92a7b50e-5c7c-45ff-91f3-34d353fcee09" />

cat < scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
^d
 ```
cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps
```
chmod 777 scriptest.sh
./scriptest.sh 1 2 3

## OUTPUT:
<img width="497" height="403" alt="image" src="https://github.com/user-attachments/assets/1b40a462-6fee-457d-ae75-a8649fa9def0" />

ls file1
## OUTPUT:
<img width="497" height="77" alt="image" src="https://github.com/user-attachments/assets/9d7279ab-b8fc-471b-97c4-c82c93b7df8b" />

echo $?
## OUTPUT: 
<img width="501" height="67" alt="image" src="https://github.com/user-attachments/assets/e1b0a17b-15b5-4faa-a363-d3256195a563" />
./one
bash: ./one: Permission denied
echo $?

abcd
echo $?
 ## OUTPUT:
 <img width="463" height="72" alt="image" src="https://github.com/user-attachments/assets/4c6e5aff-0fa0-4f9e-9740-76cfc8c45915" />

# mis-using string comparisons

cat < strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
^d
```
cat strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```
## OUTPUT:
<img width="476" height="282" alt="image" src="https://github.com/user-attachments/assets/b63594c6-6e97-4517-8a2a-6ae3cb4620b5" />

chmod 755 strcomp.sh
./strcomp.sh 
## OUTPUT
<img width="475" height="127" alt="image" src="https://github.com/user-attachments/assets/652dab8c-8e77-4127-ab9b-687c42cfb62c" />

# check file ownership
cat < psswdperm.sh 
```bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
^d
```
cat psswdperm.sh 
```bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```
./psswdperm.sh
## OUTPUT:
<img width="600" height="295" alt="image" src="https://github.com/user-attachments/assets/d377bfad-088f-4fa8-b4ba-4df577f0ce72" />

# check if with file location
cat>ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```
cat ifnested.sh 
```
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```
./ifnested.sh 
## OUTPUT:
<img width="515" height="548" alt="image" src="https://github.com/user-attachments/assets/1e535999-6daf-4b84-8094-8a6eb79f361c" />

# using numeric test comparisons
cat > iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
^d
```
cat iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
```

$ chmod 755 iftest.sh
 
$ ./iftest.sh 
## OUTPUT:
<img width="495" height="541" alt="image" src="https://github.com/user-attachments/assets/9d0d3cd6-7ca6-4c82-8a60-f797ddee90d4" />

# check if a file
cat > ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```

cat ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```
$ chmod 755 ifnested.sh
$ ./ifnested.sh 
## OUTPUT:
<img width="531" height="125" alt="image" src="https://github.com/user-attachments/assets/b2404079-2d85-43c1-9685-51bc5e72f191" />

# looking for a possible value using elif
cat elifcheck.sh 
```bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi
```
$ chmod 755 elifcheck.sh
$ ./elifcheck.sh 
## OUTPUT:
<img width="323" height="130" alt="image" src="https://github.com/user-attachments/assets/83946f8f-6712-40ad-96c6-5e0db53262a9" />

# testing compound comparisons
cat> ifcompound.sh 
```bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh
$ ./ifcompound.sh 
## OUTPUT:
<img width="452" height="132" alt="image" src="https://github.com/user-attachments/assets/7f1ba4ed-2dc1-4d05-867c-6164c49e073e" />

# using the case command
cat >casecheck.sh 
```bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac
```
$ chmod 755 casecheck.sh 
$ ./casecheck.sh 
 ## OUTPUT:
 <img width="620" height="446" alt="image" src="https://github.com/user-attachments/assets/77cd2cff-b07b-4ce3-9f29-09effa7f65b1" />

cat > whiletest
```bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```
$ chmod 755 whiletest.sh
$ ./whiletest.sh
 ## OUTPUT:
 <img width="351" height="572" alt="image" src="https://github.com/user-attachments/assets/b5637131-ed32-42a7-9e7c-ef4eb7879bdd" />

cat untiltest.sh 
```bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
``` 
$ chmod 755 untiltest.sh
## OUTPUT:
 <img width="338" height="445" alt="image" src="https://github.com/user-attachments/assets/9de82d20-5db9-47df-817e-b7b102b4370d" />

cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ``` 
$ chmod 755 forin1.sh
 ## OUTPUT:
 <img width="668" height="455" alt="image" src="https://github.com/user-attachments/assets/426ddd0b-ed47-478b-8f30-d5d61fa47d3a" />

cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ``` 
$ chmod 755 forin2.sh
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
```
$ chmod 755 forin2.sh
$ ./forin2.sh 
## OUTPUT:
<img width="543" height="377" alt="image" src="https://github.com/user-attachments/assets/bc22337d-d83d-4e4a-83ee-cc0da52eb23c" />

cat forin3.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```
$ ./forin3.sh  
cat forin1.sh 
```bash
#!/bin/bash
# basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
```
$ chmod 755 forin1.sh
## OUTPUT:
<img width="737" height="522" alt="image" src="https://github.com/user-attachments/assets/034a06c7-c032-4072-b4f6-0682331d0aa1" />

cat forinfile.sh 
```bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done
```
$ chmod 777 forinfile.sh
$ cat cities
```
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam
```
## OUTPUT:
<img width="301" height="222" alt="image" src="https://github.com/user-attachments/assets/48d11ad5-f7bc-4ac3-852b-8f1f4f53a439" />

cat forctype.sh 
```bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
````
$ chmod 755 forctype.sh
$ ./forctype.sh 
## OUTPUT:
<img width="356" height="400" alt="image" src="https://github.com/user-attachments/assets/0d90342c-173e-4d0d-b05a-9e936405fd1f" />

cat forctype1.sh 
```bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```
$ chmod 755 forctype.sh
$ ./forctype1.sh 
## OUTPUT:
<img width="378" height="172" alt="image" src="https://github.com/user-attachments/assets/41390a60-884d-402a-a942-7abb80dd4f03" />

cat fornested1.sh 
```bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done
```
$ chmod 755 fornested1.sh
$ ./fornested1.sh 
 ## OUTPUT:
<img width="335" height="403" alt="image" src="https://github.com/user-attachments/assets/f5fdbbc4-36c8-45d7-8c07-15811b8bd747" />
 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```
$ chmod 755 forbreak.sh
$ ./forbreak.sh 
## OUTPUT:
<img width="407" height="551" alt="image" src="https://github.com/user-attachments/assets/5494822b-b4aa-40e8-89df-dde3ea15d12f" />

cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
``` 
$ chmod 755 forcontinue.sh
$ ./forcontinue.sh 
## OUTPUT:
 <img width="350" height="262" alt="image" src="https://github.com/user-attachments/assets/7439bcd7-d8b8-4c74-aa88-b046e5d99eb8" />

cat exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
$ chmod 755 exread.sh 
$ ./exread.sh 
## OUTPUT:
<img width="305" height="188" alt="image" src="https://github.com/user-attachments/assets/a481b41e-295f-441d-8671-4292f4fee3ca" />

 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 
$ ./exread1.sh
## OUTPUT:
<img width="476" height="273" alt="image" src="https://github.com/user-attachments/assets/0d969881-c382-4a97-8dee-9a1820bf1a48" />
 
cat funcex.sh
```bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi
```
 ./funcex.sh 
 ./funcex.sh 1 2
## OUTPUT:
<img width="656" height="501" alt="image" src="https://github.com/user-attachments/assets/b0bd7087-3d04-4941-a984-80779965eb6f" />

cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh
$ ./argshift.sh 1 2 3
## OUTPUT:
<img width="325" height="402" alt="image" src="https://github.com/user-attachments/assets/9a8e181c-a5c3-46b5-af62-e102f10e14d7" />
 
 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
```
$ chmod 777 argshift.sh

$ ./argshift.sh 1 2 3
## OUTPUT:
<img width="381" height="477" alt="image" src="https://github.com/user-attachments/assets/0c38c09a-911e-4ed6-97d0-5c733cb04f09" />

cat argshift.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x
```
 ./argshift.sh 1 2 3
 ## OUTPUT:
 <img width="311" height="405" alt="image" src="https://github.com/user-attachments/assets/dfd47426-5ad1-42b8-9727-99c03248d841" />

cat > nc.awk
```bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 ```
cat>data.dat
```bash
bcdfghj
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj
```
awk -f nc.awk data.dat
## OUTPUT:
 <img width="338" height="181" alt="image" src="https://github.com/user-attachments/assets/392c8eec-8edd-4e2d-b267-23da59462bff" />

cat > palindrome.sh
```bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi
```
## OUTPUT: 
<img width="290" height="177" alt="image" src="https://github.com/user-attachments/assets/49afacea-1971-4392-aaaa-2e37d2971b3d" />

# RESULT:
The Commands are executed successfully.
