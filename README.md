# lab01
$ export GITHUB_USERNAME=Ekaterina06-choi 
$ export GIST_TOKEN=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
$ alias edit=nano
$ mkdir -p ${GITHUB_USERNAME}/workspace
$ cd ${GITHUB_USERNAME}/workspace
/Ekaterina06-choi/workspace$ pwd
/home/Katya/Ekaterina06-choi/workspace
/Ekaterina06-choi/workspace$ cd ${GIST_TOKEN}/workspace
bash: cd: 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/workspace: No such file or directory
/Ekaterina06-choi/workspace$ cd 
$ pwd
/home/Katya
$ mkdir -p workspace/tasks/
$ mkdir -p workspace/projects/
$ mkdir -p workspace/reports/
$ cd workspace
/workspace$ wget https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz
--2025-03-04 15:41:39--  https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz
Resolving nodejs.org (nodejs.org)... 104.20.22.46, 104.20.23.46, 2606:4700:10::6814:162e, ...
Connecting to nodejs.org (nodejs.org)|104.20.22.46|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 9356460 (8.9M) [application/x-xz]
Saving to: ‘node-v6.11.5-linux-x64.tar.xz’

node-v6.11.5-linux- 100%[===================>]   8.92M  6.00MB/s    in 1.5s    

2025-03-04 15:41:41 (6.00 MB/s) - ‘node-v6.11.5-linux-x64.tar.xz’ saved [9356460/9356460]
/workspace$ tar -xf node-v6.11.5-linux-x64.tar.xz
/workspace$ rm -rf node-v6.11.5-linux-x64.tar.xz
/workspace$ mv node-v6.11.5-linux-x64 node
/workspace$ ls node/bin
node  npm
/workspace$ echo ${PATH}
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/snap/bin
/workspace$ export PATH=${PATH}:'pwd'/node/bin
/workspace$ echo ${PATH}
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/snap/bin:pwd/node/bin
/workspace$ mkdir scrips
/workspace$ cat > scripts/active<<EOF
> export PATH=\${PATH}:'pwd'/node/bin
> EOF
bash: scripts/active: No such file or directory
/workspace$ source scripts/activate
bash: scripts/activate: No such file or directory
/workspace$ gem install gist
Command 'gem' not found, but can be installed with:
sudo snap install ruby           # version 3.4.2, or
sudo apt  install ruby-rubygems  # version 3.4.20-1
See 'snap info ruby' for additional versions.
/workspace$ (umask 0077 && echo ${GIST_TOKEN} > ~/.gist)
