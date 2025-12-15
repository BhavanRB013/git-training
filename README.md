# git-training
crash and learn
first time to do something in git
HI bro
first used git clone to download the repo in my local repository
after downloading i opened the downloaded folder 
used git status there is nothing to add to remote server
before this i need to use git config to set the user email and name
in already existing readme i added a line
after giving git status it gived modified
used git add which will push my changes to stagging area consider this as the entry before saving it in remote server
then used git commit to save it in remote server

--------------------------------------------
now there is a problem for pushing it in remote as because current git doesn't accept
uploading using password so it needs some key so the process is
generate a ssh key
copy the key
in github setting under deploy keys add it
as owr git is using http we need to switch it to ssh
then push

------------------------------------------------------
1. go to home directory and use the command "ssh-keygen -t ed25519 -C "your-email@gmail.com"".
2. this will be located in the ~/.ssh/ path. copy the content of .pub file
3. you can check whether the key is present or not by using the command "\eval "$(ssh-agent -s)"" followed by
ssh-add .ssh/ssh-key
4. to change from http to ssh the folloeing command is used "it remote set-url origin git@github.com:BhavanRB013/git-training.git" 
5. to check whether youa re using http or ssh the command "git remote -v" is used
