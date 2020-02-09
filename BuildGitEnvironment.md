How to build git environment!

Hello, I am y-monaca!

Now today, I will write how to build git environment on CentOS8
as practicing to write in English.

1. git install  
root# dnf install -y git

2. initial setting  
root# git config --global user.name "hoge"  
root# git config --global user.email hoge@hoge.com  

3. making test file  
root# su - hoge //changing user  
hoge$ cd /home/hoge  
hoge$ echo "TEST" >> TEST.txt  

4. initializing  
hoge$ git init  
Initialized empty Git repository in /home/hoge/git/.git/  

5. adding the file to staging  
hoge$ git add TEST.txt  

6. adding the file to local repository from statging  
hoge$ git commit -m "first commit!!!"  

7. registering remote repository  
hoge$ git remote add origin https://github.com/xxx/test.git //name:origin  
(You should make repository "/test" on github in advance.)  

8. Confiming repository  
hoge$ git remote -v  
origin	https://github.com/xxx/test.git (fetch)  
origin	https://github.com/xxx/test.git (push)  

9. uploading the file from local repository to remote repository  
hoge$ git push -u origin master //branch:master  


Thank you!!!
