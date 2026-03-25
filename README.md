# OPEN-SOURCE-EX-5

#### NAME : GURURAGHAV PONJEEVITH V
#### REG NO : 21223220027

## AIM:
To configure, verify, and manage scheduled automated tasks for the user harry using crontab and system services, and to validate their execution through system logs.

## ALGORITHM:


STEP 1 : sudo -i

STEP 2 : crontab -u harry -e

STEP 3 : # Run daily at 12:30 PM

30 12 * * * /bin/echo "hello"

##### Run every 2 minutes
*/2 * * * * /bin/echo "Hi I'm Running"


##### Run daily at 2:23 PM
23 14 * * * /usr/bin/logger "RHCSA EXAM TRAINING"


##### Run daily at 12:00 PM
0 12 * * * /usr/bin/logger "EX200 in Progress"

STEP 4 : crontab -u harry -l

STEP 5 : systemctl status cron

STEP 6 : systemctl start crond systemctl enable crond

STEP 7 : sudo -u harry /bin/echo "hello" sudo -u harry /usr/bin/logger "RHCSA EXAM TRAINING"

STEP 8 : journalctl | grep RHCSA


## OUTPUT:
<img width="1309" height="976" alt="image" src="https://github.com/user-attachments/assets/0549b9bf-c898-4eaf-b61c-f10a4e4f1d70" />


## RESULT :
The commands are successfully compiled in RetHat Lab(Terminal)
