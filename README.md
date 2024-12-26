Hello Dosto

this file is for understanding the concept of Github for Devops.

# there are 3 steps to push the changes in github

1) by adding user name and password like below :
ubuntu@ip-172-31-22-63:~/github/git-for-devops$ git push
Username for 'https://github.com':  shubhamnalwade
Password for 'https:// shubhamnalwade@github.com': <token generated from github account>

2) By changing the origin/remote url like below :
ubuntu@ip-172-31-22-63:~/github/git-for-devops$ git remote set-url origin  https://<secret-token>/shubhamnalwade/git-for-devops.git
ubuntu@ip-172-31-22-63:~/github/git-for-devops$ git remote -v
origin  https://<token>/shubhamnalwade/git-for-devops.git (fetch)
origin  https://<token>/shubhamnalwade/git-for-devops.git (push)
ubuntu@ip-172-31-22-63:~/github/git-for-devops$ git push origin main
