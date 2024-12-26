This file used for understanding the concept of GitHub.

1) By adding user name and password like below :

ubuntu@ip-172-31-22-63:~/github/git-for-devops$ git push
Username for 'https://github.com':  shubhamnalwade
Password for 'https:// shubhamnalwade@github.com': <token generated from github account>
(how to generate token : https://github.com/settings/tokens and then click on Generate token and check the checkbox for repo and use it)

2) By changing the origin/remote url like below :

ubuntu@ip-172-31-22-63:~/github/git-for-devops$ git remote set-url origin  https://<token>@github.com/shubhamnalwade/git-for-devops.git
ubuntu@ip-172-31-22-63:~/github/git-for-devops$ git remote -v
ubuntu@ip-172-31-22-63:~/github/git-for-devops$ git push origin main
*note : we can use only <git push> as well to push the changes to remote repo.

3) Using ssh key :

Generate the public and private key using ssh-keygen under .ssh folder and 
copy the public key and add here https://github.com/settings/keys and
also change the origin url like below :
ubuntu@ip-172-31-22-63:~/github/git-for-devops$ git remote set-url origin git@github.com:shubhamnalwade/git-for-devops.git
