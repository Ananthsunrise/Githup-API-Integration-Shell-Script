# Githup-API-Integration-Shell-Script

**Description:**
In this project I find list of users who having access to particular githup repository using github api integration in shell script.
for that, you need to create organizations and create repositories inside your github account to practice this project.

**Explanation fo attached shell scriipt:**
In this, I put github api url to integrate githup api integration.
Then I soft coded github username and token in script to integrate our github account.(we need to export username and token in inux terminal)
Then I passe 2 command line arguments (i.e) organization name and repository name 
Then I wrote a code to get list of users in my github repository.
Here also I am using jq command to filter only  specific details form json.

**How to execut shell script file?**
1.Go to aws console and create one ec2 linuc server.
2.login server using putty
3.enter below commands
  export username = "<your github account name> "
  export token    = "<token url>"    (to get token url, go to github account->click setting->click developers settings->click personal access tokens->click generate token)
  chmod 777 list-users.sh   (to give permissios for file)
  sudo apt install jq -y   (to install jq, if it is not in linux machine)
  ./list users.sh <oraganization name> <repository name>  (to execute file)
