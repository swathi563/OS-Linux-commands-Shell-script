## Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting
# NAME : SWATHI S
# REGISTER NO; 212225040449
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
cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```
### Display the content of the files
cat < file1

## OUTPUT

<img width="422" height="181" alt="627043824-85c3764f-65ca-43a5-824a-6914300a9b51" src="https://github.com/user-attachments/assets/c36986ea-45d7-49d3-8433-2653c0c3053b" />

cat < file2
## OUTPUT

<img width="382" height="197" alt="627044005-5d9e0ce6-8661-42fe-a86a-b98427fa8270" src="https://github.com/user-attachments/assets/17153ec9-4031-41aa-bc67-7b190dc4649f" />

# Comparing Files
cmp file1 file2
## OUTPUT
 
<img width="426" height="95" alt="627044245-00828879-46e6-4622-b056-ea1a970b2ba1" src="https://github.com/user-attachments/assets/98f61610-56c6-495b-91b0-e339c584daea" />

comm file1 file2
 ## OUTPUT
 
<img width="550" height="292" alt="627044504-ad47e135-1c08-4ba6-8c20-cd0195fa95a6" src="https://github.com/user-attachments/assets/6b1195b2-f81f-493f-8c46-52835dc91e88" />

diff file1 file2
## OUTPUT

<img width="455" height="317" alt="627044721-19c310b8-8818-4afe-b60f-ce390e0a3665" src="https://github.com/user-attachments/assets/9b42206c-83c1-4365-adfe-a3eb52c9b9b9" />

# Filters

### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
## OUTPUT:

<img width="415" height="92" alt="627045737-1bc131dc-7120-46d8-99d6-ef56f0cd0f79" src="https://github.com/user-attachments/assets/c9cf7694-84f4-4d66-849f-bf72101da0cf" />

cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```
## OUTPUT:

<img width="421" height="107" alt="627046047-dee9e8ec-43b6-4744-9ac1-51f263ea34ce" src="https://github.com/user-attachments/assets/928ab3cd-0a67-44d2-9067-c01615283c72" />


cut -c1-3 file11
## OUTPUT

<img width="437" height="127" alt="627045905-b731a65e-5614-4e09-a001-05b541242a06" src="https://github.com/user-attachments/assets/6c79750d-bc40-4610-9ed6-2b0a08b8b0a6" />

cut -d "|" -f 1 file22
## OUTPUT


<img width="425" height="127" alt="627046323-d815891d-1fbf-4d4d-b701-624f7c1364ce" src="https://github.com/user-attachments/assets/6cee6725-6b44-490b-b4fe-091296ba946b" />
cut -d "|" -f 2 file22
## OUTPUT

<img width="366" height="122" alt="627046605-b9048550-afb9-428d-b986-626f20325e9a" src="https://github.com/user-attachments/assets/b3bb0a1a-7a61-4872-910b-374c8e245414" />

cat < newfile 
```
Hello world
hello world
^d
````
cat > newfile 
Hello world
hello world
## OUTPUT:

<img width="437" height="112" alt="627047418-158d920b-6b0c-4485-9b47-72a3c5d97a80" src="https://github.com/user-attachments/assets/d26544ff-d682-48b7-b251-83179de36019" />

grep Hello newfile 
## OUTPUT

<img width="327" height="76" alt="627050385-b5bc6b48-9ef8-4123-9b2f-c2a2bda45df0" src="https://github.com/user-attachments/assets/ad39240a-767d-4418-b213-c58440a8ab70" />

grep hello newfile 
## OUTPUT

<img width="277" height="137" alt="627051371-51638577-c272-461f-97f8-34dc7476e844" src="https://github.com/user-attachments/assets/94ed186e-f448-451c-98c1-986f53ee32cc" />

grep -v hello newfile 
## OUTPUT

<img width="362" height="77" alt="627051621-63c5b410-455a-4a02-9b02-1c6f4e4bcec6" src="https://github.com/user-attachments/assets/98ddce59-e6b3-483a-aaa4-e368beb6a9be" />

cat newfile | grep -i "hello"
## OUTPUT

<img width="502" height="171" alt="627052060-60636515-374b-4009-8fa2-ad7990264bfd" src="https://github.com/user-attachments/assets/da0398ac-b76f-4c39-a72c-ee4c68d98fde" />

cat newfile | grep -i -c "hello"
## OUTPUT

<img width="476" height="81" alt="627052392-be97679d-1a7f-473a-8939-093ede1decbf" src="https://github.com/user-attachments/assets/5373c4df-143b-46b9-b4da-3aba4f4fe731" />

grep -R ubuntu /etc
## OUTPUT

<img width="801" height="557" alt="627052806-ae09ecc8-ebfa-4669-9361-f397f6e0b84f" src="https://github.com/user-attachments/assets/364969d7-6f81-4661-8c0b-d0cb6c1f6f54" />

grep -w -n world newfile   
## OUTPUT

<img width="422" height="132" alt="627053344-e27121b6-44a4-471f-be12-42ff8c8d08cb" src="https://github.com/user-attachments/assets/cc5d726e-624d-4080-aed7-d2366ef743d8" />

cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```

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

<img width="502" height="347" alt="627053973-69a62b1e-f677-4a9b-b98a-4115bc444250" src="https://github.com/user-attachments/assets/d168ea26-4e25-469e-85b0-6fd082e3a434" />

egrep -w 'Hello|hello' newfile 
## OUTPUT

<img width="451" height="131" alt="627054203-3d1dcac4-54e0-4663-aacb-fcbe92c2c439" src="https://github.com/user-attachments/assets/ad19844b-191d-4ab5-8c6f-ddb4b08c6c6c" />

egrep -w '(H|h)ello' newfile 
## OUTPUT

<img width="616" height="152" alt="627258404-aeaa6a14-8deb-4095-a395-1ad2528d5455" src="https://github.com/user-attachments/assets/b150d0bf-a002-4070-83f2-c20db68d4545" />

egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT

<img width="462" height="107" alt="627273649-ce8b77e5-076a-4bdc-bd26-503d1d705449" src="https://github.com/user-attachments/assets/0648b23c-2d35-4fff-b3da-f78c3a920eaf" />

egrep '(^hello)' newfile 
## OUTPUT

<img width="446" height="81" alt="627273893-d4df2506-9ba6-4a7f-9be3-b02114a2c4fe" src="https://github.com/user-attachments/assets/7588217c-4574-4d32-b8b6-3ee56fd2fd25" />

egrep '(world$)' newfile 
## OUTPUT




<img width="452" height="110" alt="627274168-3a4c5b2f-521b-48ee-92f0-1023e643f121" src="https://github.com/user-attachments/assets/4997912a-9998-423e-81c8-e89332176795" />
egrep '(World$)' newfile 
## OUTPUT

<img width="481" height="80" alt="627274362-97119d37-0589-4811-9205-139fb2a125a2" src="https://github.com/user-attachments/assets/45fe1973-5b33-4c08-ab47-b4d7c3ff94e8" />

egrep '((W|w)orld$)' newfile 
## OUTPUT

<img width="502" height="137" alt="627274604-9c1b0ea0-a206-4a2e-867e-e70da3c41580" src="https://github.com/user-attachments/assets/b9c124ea-2a6d-4916-86b2-8fe0a9ce7c34" />

egrep '[1-9]' newfile 
## OUTPUT

<img width="511" height="82" alt="627274757-3b821cd8-f37c-4f23-84cd-b35cf2e6cbfb" src="https://github.com/user-attachments/assets/873c2d07-3db1-4ef1-b8a9-36fe1074f099" />

egrep 'Linux.*world' newfile 
## OUTPUT

<img width="502" height="76" alt="627274973-a48bd0b2-40a3-416e-87c4-d1b1b8ca4d2a" src="https://github.com/user-attachments/assets/6bd0a4ca-d9de-4cdc-84e8-fd422396f750" />

egrep 'Linux.*World' newfile 
## OUTPUT

<img width="515" height="82" alt="627275196-76ed0410-e67c-49ea-be99-42f025938e6c" src="https://github.com/user-attachments/assets/d5887d31-6d53-437e-a032-f38f4d8f607a" />

egrep l{2} newfile
## OUTPUT

<img width="477" height="106" alt="627275388-1feaaeab-c7bf-4622-ade0-cc97c3b161e4" src="https://github.com/user-attachments/assets/80ee7c4c-e314-4d1b-82d8-69d084a46985" />
egrep 's{1,2}' newfile
## OUTPUT 

<img width="455" height="122" alt="627275584-d461e47f-2f8b-464d-a24c-46846960daf3" src="https://github.com/user-attachments/assets/e035f323-aae1-4964-8361-548132fd4bba" />

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


sed -n -e '3p' file23
## OUTPUT

<img width="447" height="86" alt="627275962-0b316301-f984-4433-b938-11d32f29ec9d" src="https://github.com/user-attachments/assets/fbfd2063-055a-4913-b303-da2897fa2a3c" />

sed -n -e '$p' file23
## OUTPUT

<img width="505" height="82" alt="627276131-78df2f6d-1ae7-4af9-b13a-9bb193da105d" src="https://github.com/user-attachments/assets/68de2277-a98d-41ad-b373-b2a432243a58" />

sed  -e 's/Ram/Sita/' file23
## OUTPUT


<img width="535" height="256" alt="627276348-60d0100a-6e60-4d7b-b96f-0c569716ecc5" src="https://github.com/user-attachments/assets/490909dc-7322-4664-a726-957aadda9bb0" />
sed  -e '2s/Ram/Sita/' file23
## OUTPUT

<img width="527" height="252" alt="627276614-d0d5aa8a-2d5d-4815-94ef-619f8452bac3" src="https://github.com/user-attachments/assets/98a0ab32-655b-41bf-9174-da7a456bb07a" />

sed  '/tom/s/5000/6000/' file23
## OUTPUT

<img width="602" height="257" alt="627276904-ee87ce34-cf59-4adf-a362-2d01742fed7d" src="https://github.com/user-attachments/assets/c92190fd-d03c-489a-8504-133cbebacb60" />

sed -n -e '1,5p' file23
## OUTPUT

<img width="476" height="185" alt="627277142-1b4fb9d2-56b2-4822-a00a-98f693e0a41b" src="https://github.com/user-attachments/assets/acd73f1f-ad70-431b-9201-7612fe391f8e" />

sed -n -e '2,/Joe/p' file23
## OUTPUT

<img width="500" height="132" alt="627277298-d58f0818-927e-41c0-949e-28898ce48930" src="https://github.com/user-attachments/assets/35b8d177-ba10-4c1c-b977-57e35036e5f4" />

sed -n -e '/tom/,/Joe/p' file23
## OUTPUT

<img width="486" height="107" alt="627277512-072f03aa-5e4a-4e65-b3a1-0deab6e68e5b" src="https://github.com/user-attachments/assets/0249312d-0aa8-455e-bc53-4480dcd0355d" />

seq 10 
## OUTPUT

<img width="467" height="302" alt="627277765-2c03d7de-631a-4fa2-a526-1a226196cf86" src="https://github.com/user-attachments/assets/adc87372-a5d3-473e-96ee-5d83b8281608" />

seq 10 | sed -n '4,6p'
## OUTPUT

<img width="422" height="127" alt="627277980-12edc6f2-3fab-4766-aaf6-6aac1a71577b" src="https://github.com/user-attachments/assets/4c4ad223-b5a9-4375-8c1e-9590d76ea148" />

seq 10 | sed -n '2,~4p'
## OUTPUT

<img width="425" height="125" alt="627278177-553fbaee-7bc5-463f-8968-5f6ea69e489e" src="https://github.com/user-attachments/assets/5c3a8f19-bb06-42c1-8d7c-ef9624fe5148" />
seq 3 | sed '2a hello'
## OUTPUT

<img width="517" height="155" alt="627278485-bccba5b4-df67-4b9d-8c38-cfd686b9d5a4" src="https://github.com/user-attachments/assets/8ff660c5-84c1-45ad-a6af-64ec8d1f1c0f" />

seq 2 | sed '2i hello'
## OUTPUT

<img width="452" height="125" alt="627278716-8eb2e52f-ad62-4c6b-b2d6-953ded484122" src="https://github.com/user-attachments/assets/19158af3-0ff0-42c8-995c-1ae52acb7bf5" />

seq 10 | sed '2,9c hello'
## OUTPUT

<img width="472" height="127" alt="627278942-beb197c2-f4e0-4a53-bf50-3ad2c68156b7" src="https://github.com/user-attachments/assets/4ec652be-4cd1-43a5-bff0-9fdf6073118d" />

sed -n '2,4{s/^/$/;p}' file23
## OUTPUT

<img width="491" height="131" alt="627279187-a3010957-10ce-4383-b28a-d987f97a3a75" src="https://github.com/user-attachments/assets/1e62e520-59ce-4367-9941-ac37014a5c9e" />

sed -n '2,4{s/$/*/;p}' file23
## OUTPUT

<img width="505" height="136" alt="627279432-dff09f1b-5b37-4d5a-8987-799d9461790b" src="https://github.com/user-attachments/assets/ba7ca69f-0a66-4eed-8bed-d2f0ba887630" />


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
## OUTPUT

<img width="542" height="357" alt="627279857-3edc9f60-074a-47f3-b3f5-7ed82bf6ac41" src="https://github.com/user-attachments/assets/37b179a1-142c-4769-bbf9-f1d6b078d32b" />

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
## OUTPUT

<img width="677" height="375" alt="627280300-f93c644b-5c0b-4dfc-a000-632580b51e02" src="https://github.com/user-attachments/assets/e0fa8c4d-348c-4ef6-931c-f2fc674a254e" />

#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT

<img width="532" height="252" alt="627280522-7206006a-160a-4cb1-8961-904ba78ae67e" src="https://github.com/user-attachments/assets/a5be624d-f611-4f4a-a3cf-c3604999f772" />
cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
## OUTPUT

<img width="477" height="256" alt="627281143-d1dea4a9-717b-4f2a-aac7-4ec89b04da11" src="https://github.com/user-attachments/assets/bf3ee762-9c1c-456a-bfe1-e6e3d6e63b9c" />

cat urllist.txt | tr -d ' '
 ## OUTPUT

<img width="491" height="130" alt="627281290-ff8a3926-ef09-4d71-a05c-a0acf390ac35" src="https://github.com/user-attachments/assets/9d677ce0-281a-4a37-a4d6-71a3a402cde3" />

cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT

<img width="552" height="132" alt="627281522-46099f13-9ea6-4a67-8645-9886d810b975" src="https://github.com/user-attachments/assets/35670bd8-c8ed-489d-abae-113a6fedefa7" />
#Backup commands
tar -cvf backup.tar *
## OUTPUT

<img width="670" height="702" alt="627281860-b8f70164-1807-4daa-b98b-cea5750cd332" src="https://github.com/user-attachments/assets/118c30c9-b066-4843-b3b1-2a6f8e151238" />
mkdir backupdir
 
mv backup.tar backupdir

cd backupdir
 
tar -tvf backup.tar
## OUTPUT

<img width="807" height="702" alt="627283978-0279c30b-364f-478a-9010-2f4c1578a1ed" src="https://github.com/user-attachments/assets/dd2396cb-7f08-40f6-acd6-352f03b4224c" />
tar -xvf backup.tar
## OUTPUT

<img width="738" height="693" alt="627284091-947ebe0a-8cdd-43f9-ad12-8cfc7112be7b" src="https://github.com/user-attachments/assets/bdf5b605-4bff-4821-8c19-f491c972475f" />

gzip backup.tar

ls .gz
## OUTPUT
 
<img width="738" height="693" alt="627284091-947ebe0a-8cdd-43f9-ad12-8cfc7112be7b" src="https://github.com/user-attachments/assets/a4574434-3741-464b-bc7e-ed5cef7e27a8" />
gunzip backup.tar.gz
## OUTPUT

<img width="436" height="92" alt="627284445-b496290a-72f9-4cda-a2c8-9a00e22fb8d0" src="https://github.com/user-attachments/assets/46e4528b-e324-4bad-89cf-07b935ac247f" />
# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT

<img width="516" height="227" alt="629994637-51fba364-2a53-407b-9401-f65b0ca45980" src="https://github.com/user-attachments/assets/0294478f-c774-4b77-a8c3-aca362a74f79" />
cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
## OUTPUT

<img width="452" height="272" alt="629994650-d47add4b-8c00-4b09-b970-5ab9799a53df" src="https://github.com/user-attachments/assets/83ea01f7-6aeb-423f-b8f9-8a42c78e096d" />

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

## OUTPUT

<img width="707" height="347" alt="629995157-4f052c9c-c23a-4dc6-b9a7-e8862abd075f" src="https://github.com/user-attachments/assets/3f846cec-6c95-4c0e-a0ef-f414ecaa8505" />

ls file1
## OUTPUT

<img width="293" height="74" alt="629995206-bf21dd0c-5c06-422a-8398-35b774381c51" src="https://github.com/user-attachments/assets/d3bf5003-b02e-4825-85ef-93e74a329f7b" />

echo $?
## OUTPUT 
./one
bash: ./one: Permission denied
 
echo $?
<img width="377" height="75" alt="629995239-38390637-dff0-48d0-80c0-0facf4827b10" src="https://github.com/user-attachments/assets/0613fa7c-b9e5-4a8c-9f00-f258248631dd" />

## OUTPUT 
 
<img width="367" height="80" alt="629995255-cfe4d8eb-5aad-4f0c-94f8-dc59d6378cd9" src="https://github.com/user-attachments/assets/accb6fa1-c24e-4fe3-8ebd-77a0ea634442" />
abcd
 
echo $?
 ## OUTPUT

<img width="367" height="80" alt="629995263-ff9cb5e4-90b9-4465-ba3c-5b91ded86c0e" src="https://github.com/user-attachments/assets/8eb2e4b6-5326-4c91-a083-f78bb47edf10" />

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
##OUTPUT

<img width="827" height="281" alt="629995893-b95d35a9-0c40-4073-8c49-5a2da36cb6f7" src="https://github.com/user-attachments/assets/488a1cf7-5f0e-44ac-8a8c-7764dc230eee" />

chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT

<img width="677" height="156" alt="629996143-703409e0-0a4b-475a-8de6-10ee97365d44" src="https://github.com/user-attachments/assets/9c5c03f9-1da3-44d7-8ad1-a10297936275" />

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
## OUTPUT

<img width="750" height="237" alt="629996519-b2021d18-d456-4669-b7db-5384fe4a3156" src="https://github.com/user-attachments/assets/26af8d54-2782-46a2-bd7b-af3c10b1dff0" />

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
## OUTPUT

<img width="657" height="475" alt="629996920-2e0b56e0-c8c7-406d-b79f-46d9519f8356" src="https://github.com/user-attachments/assets/efe5e192-72fd-475a-819a-fe97288aeee1" />

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
## OUTPUT

<img width="613" height="166" alt="629997341-f3433adc-ed5f-43f3-8012-e7674971cd6c" src="https://github.com/user-attachments/assets/b2f85c57-9468-44eb-adcb-224d85207a0f" />

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
## OUTPUT

<img width="791" height="200" alt="629997677-86fc2cd3-99a6-452e-b54f-e30562ed27fc" src="https://github.com/user-attachments/assets/f84dcb24-a815-49bc-a4f2-d908ff6fe20b" />


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
## OUTPUT

<img width="782" height="167" alt="629998232-ea2d12b1-7b6f-443a-969c-b2d48df7c236" src="https://github.com/user-attachments/assets/19fb4c40-6442-479e-a9cb-3d8bf2412682" />



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
## OUTPUT


<img width="890" height="177" alt="629998464-817aabcb-4be9-4746-80a4-f266fae602de" src="https://github.com/user-attachments/assets/d1f29000-49a4-4af0-a497-0baa713ceed8" />


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
## OUTPUT 

<img width="587" height="137" alt="629998719-9dede2a9-ddb1-42ea-b083-3134229e66a0" src="https://github.com/user-attachments/assets/c9a6e66d-9567-447d-9b8b-2c9d79a6f184" />

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
## OUTPUT

<img width="366" height="339" alt="629999166-70df3b4e-eec5-4e7d-bffc-ac8f141a91d3" src="https://github.com/user-attachments/assets/919d714e-4255-471a-8dd3-5c3e2fe37554" />

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
 ## OUTPUT

 <img width="671" height="237" alt="629999476-6a3147dd-ab0e-4ec1-b5d5-25c6088ed331" src="https://github.com/user-attachments/assets/47be05eb-0685-494b-a239-8d0fc67dc0d3" />

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
## OUTPUT

<img width="682" height="311" alt="629999760-167b7f63-df96-441f-badc-225d14fae7c9" src="https://github.com/user-attachments/assets/93cf1a16-13ba-48d7-bb79-13f77375aa5e" />

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
## OUTPUT
<img width="737" height="221" alt="630000026-441af616-b478-4354-8b05-3972e40fb8db" src="https://github.com/user-attachments/assets/79b95fce-4c3d-4448-9b4f-ae090bbe31bd" />

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
 

## OUTPUT

<img width="551" height="257" alt="630000782-ecf0e380-c59a-476b-886e-bd519963ff06" src="https://github.com/user-attachments/assets/977b28b5-263a-4f4c-81a7-e69143d95e9c" />

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

## OUTPUT

<img width="551" height="257" alt="630000782-ecf0e380-c59a-476b-886e-bd519963ff06" src="https://github.com/user-attachments/assets/a8ce1d7c-b3f8-41da-b83d-0e48f8faa59a" />

#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done
$ chmod 777 forinfile.sh


$ cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

## OUTPUT

<img width="517" height="257" alt="630001449-6f9acb7b-bc53-4491-9a36-18dd8d5d7888" src="https://github.com/user-attachments/assets/98a58a92-e005-4301-b60c-81e66aacbfc2" />

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

## OUTPUT

<img width="600" height="230" alt="630001700-73393767-0cfb-4fda-b8e8-8398177f77af" src="https://github.com/user-attachments/assets/11584c30-9c5e-48c3-84d4-0fb9fb989004" />

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
## OUTPUT

<img width="441" height="230" alt="630002111-29b3601e-f19e-4ad0-a24a-26ec33a785de" src="https://github.com/user-attachments/assets/38ac4a6e-68ab-46ec-9fa6-a1d8ef7f615e" />

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
 ## OUTPUT

<img width="517" height="402" alt="630002300-1d6440da-c151-415d-9017-6bdc4117a650" src="https://github.com/user-attachments/assets/d1a9e727-7ea7-4828-8aae-8546007cc6a1" />

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

## OUTPUT

<img width="720" height="155" alt="630002683-ff5a968f-14f5-4d2d-ba6e-5baba0f6a128" src="https://github.com/user-attachments/assets/6eaf7c07-f422-4e76-982e-a4eaf718f51d" />

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

## OUTPUT

<img width="532" height="197" alt="630003081-b41ea305-b848-4922-adeb-04f6c4a0c832" src="https://github.com/user-attachments/assets/8bd2c9e6-5a53-4e04-9f6f-622bf0f24179" />

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
## OUTPUT

<img width="600" height="155" alt="630003477-a6b26d7c-9aaa-4b08-ba18-1da0cdd83829" src="https://github.com/user-attachments/assets/e1ba0f7b-d92d-43cd-918b-64968adf229d" />

 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT

<img width="407" height="127" alt="630004176-859208e1-e2f5-4b7a-bd20-353060b2fecd" src="https://github.com/user-attachments/assets/650322b9-3b1e-44d2-a442-ef49282c1c7d" />

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
## OUTPUT

<img width="502" height="210" alt="630004644-ead5ecf8-e5fa-4e5b-91d3-cbddc7b0068f" src="https://github.com/user-attachments/assets/8e1cbd28-51c1-4c2d-ae17-a312c9ab6849" />

 
cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh

## OUTPUT

<img width="309" height="127" alt="630005128-4dee4714-aa72-4d2f-98d0-7cc91205629c" src="https://github.com/user-attachments/assets/2b317e00-a7b6-4a88-8dfd-50e7ad4145f2" />
$ ./argshift.sh 1 2 3
 
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
## OUTPUT




<img width="486" height="172" alt="630005439-dcc57f64-f595-4024-8914-0ea759dcde9e" src="https://github.com/user-attachments/assets/13b06866-ddfe-427d-bd58-c95c988c15c1" />

$ ./argshift.sh 1 2 3
 
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
## OUTPUT
 ./argshift.sh 1 2 3

<img width="665" height="462" alt="630006316-09ff7b62-33f8-49de-a73a-81aa5d134467" src="https://github.com/user-attachments/assets/c2cd8849-d031-4878-8483-957e881474bc" />

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
## OUTPUT 

<img width="472" height="381" alt="630006750-41aee01c-ddae-4604-8dc6-ea7e392d3c16" src="https://github.com/user-attachments/assets/a0df6147-5365-48df-a3fc-404d6a804b3f" />

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
	# Get Remainder<img width="472" height="381" alt="630006750-41aee01c-ddae-4604-8dc6-ea7e392d3c16" src="https://github.com/user-attachments/assets/c4a6d63a-0195-4096-887b-caff895bfff7" />

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
## OUTPUT 

<img width="687" height="210" alt="image" src="https://github.com/user-attachments/assets/c41351da-68f8-46a2-aa7d-40d22cd676c7" />



# RESULT:
The Commands are executed successfully.


