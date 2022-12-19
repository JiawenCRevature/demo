## Deploy command

## getting the sofeware on your instance
```cli
sudo yum install git # this installs git on your instance

sudo amazon-linux-extras install java-openjkd11 # this installs java 11

sudo yum install maven # this installs maven (might not be up to date)
```
## clone the repo of source doe to your instance

git clone (repo link)

## use maven to build your app

mvn package ## build plugin versions might need to be adjusted

## run your app

java -jar target/{jar file} # this runs the app directly in your terminal. prevents you from interacting further

nohup java -jar target/{jar file} & ##this runs the app in the background and redirects all std output to a file call nohup.out in the same directory you executed the command in


## move foreground app into background
ctr + z # this will stop the process and move it into the background

## move backgound process into foreground
jobs #this will give you the job number of the background process

fg %{job number} #this will move the job from the background into foreground

## killing a process

ps # returns all current processes and their PID numbers

kill {pid of job to kill} # this tells unix to try and stop the process

kill -9 {pid of job to kill} # this force unix to end the process. can cause issues if there are supposed to be shundown 

## Detail
use man with  command name to get details