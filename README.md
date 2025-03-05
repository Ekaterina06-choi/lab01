$ export GITHUB_USERNAME=Ekaterina06-choi
$ export GIST_TOKEN=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
$ alias edit=nano
$ mkdir -p ${GITHUB_USERNAME}/workspace
$ cd ${GITHUB_USERNAME}/workspace
/Ekaterina06-choi/workspace$ pwd
/home/Katya/Ekaterina06-choi/workspace
/Ekaterina06-choi/workspace$ cd ..
/Ekaterina06-choi$ pwd
/home/Katya/Ekaterina06-choi
Katya@ubuntu:~/Ekaterina06-choi$ mkdir -p workspace/tasks/
Katya@ubuntu:~/Ekaterina06-choi$ mkdir -p workspace/projects/
Katya@ubuntu:~/Ekaterina06-choi$ mkdir -p workspace/reports/
Katya@ubuntu:~/Ekaterina06-choi$ cd workspace
Katya@ubuntu:~/Ekaterina06-choi/workspace$ wget https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz
--2025-03-05 20:20:14--  https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz
Resolving nodejs.org (nodejs.org)... 104.20.23.46, 104.20.22.46, 2606:4700:10::6814:172e, ...
Connecting to nodejs.org (nodejs.org)|104.20.23.46|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 9356460 (8.9M) [application/x-xz]
Saving to: ‘node-v6.11.5-linux-x64.tar.xz’

node-v6.11.5-linux- 100%[===================>]   8.92M  3.66MB/s    in 2.4s    

2025-03-05 20:20:17 (3.66 MB/s) - ‘node-v6.11.5-linux-x64.tar.xz’ saved [9356460/9356460]

Katya@ubuntu:~/Ekaterina06-choi/workspace$ tar -xf node-v6.11.5-linux-x64.tar.xz
Katya@ubuntu:~/Ekaterina06-choi/workspace$ rm -rf node-v6.11.5-linux-x64.tar.xz
Katya@ubuntu:~/Ekaterina06-choi/workspace$ mv node-v6.11.5-linux-x64 node
Katya@ubuntu:~/Ekaterina06-choi/workspace$ ls node/bin
node  npm
Katya@ubuntu:~/Ekaterina06-choi/workspace$ echo ${PATH}
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/snap/bin
Katya@ubuntu:~/Ekaterina06-choi/workspace$ mkdir scripts
Katya@ubuntu:~/Ekaterina06-choi/workspace$ cat > scripts/activate<<EOF
> export PATH=\${PATH}:'pwd'/node/bin
> EOF
Katya@ubuntu:~/Ekaterina06-choi/workspace$ source scripts/activate
Katya@ubuntu:~/Ekaterina06-choi/workspace$ gem install gist
ERROR:  While executing gem ... (Gem::FilePermissionError)
    You don't have write permissions for the /var/lib/gems/3.3.0 directory.
 /usr/lib/ruby/vendor_ruby/rubygems/installer.rb:713:in `verify_gem_home'
 /usr/lib/ruby/vendor_ruby/rubygems/installer.rb:903:in `pre_install_checks'
 /usr/lib/ruby/vendor_ruby/rubygems/installer.rb:303:in `install'
 /usr/lib/ruby/vendor_ruby/rubygems/resolver/specification.rb:105:in `install'
 /usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:195:in `block in install'
 /usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:183:in `each'
 /usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:183:in `install'
 /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:215:in `install_gem'
 /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:231:in `block in install_gems'
 /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:224:in `each'
 /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:224:in `install_gems'
 /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:170:in `execute'
 /usr/lib/ruby/vendor_ruby/rubygems/command.rb:328:in `invoke_with_build_args'
 /usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:253:in `invoke_command'
 /usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:193:in `process_args'
 /usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:151:in `run'
 /usr/lib/ruby/vendor_ruby/rubygems/gem_runner.rb:52:in `run'
 /usr/bin/gem:12:in `<main>'
Katya@ubuntu:~/Ekaterina06-choi/workspace$ ^C
Katya@ubuntu:~/Ekaterina06-choi/workspace$ sudo snap install ruby
[sudo] password for Katya: 
error: This revision of snap "ruby" was published using classic confinement and
       thus may perform arbitrary system changes outside of the security
       sandbox that snaps are usually confined to, which may put your system at
       risk.
Katya@ubuntu:~/Ekaterina06-choi/workspace$ gem install gist
ERROR:  While executing gem ... (Gem::FilePermissionError)
    You don't have write permissions for the /var/lib/gems/3.3.0 directory.
 /usr/lib/ruby/vendor_ruby/rubygems/installer.rb:713:in `verify_gem_home'
 /usr/lib/ruby/vendor_ruby/rubygems/installer.rb:903:in `pre_install_checks'
 /usr/lib/ruby/vendor_ruby/rubygems/installer.rb:303:in `install'
 /usr/lib/ruby/vendor_ruby/rubygems/resolver/specification.rb:105:in `install'
 /usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:195:in `block in install'
 /usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:183:in `each'
 /usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:183:in `install'
 /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:215:in `install_gem'
 /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:231:in `block in install_gems'
 /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:224:in `each'
 /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:224:in `install_gems'
 /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:170:in `execute'
 /usr/lib/ruby/vendor_ruby/rubygems/command.rb:328:in `invoke_with_build_args'
 /usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:253:in `invoke_command'
 /usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:193:in `process_args'
 /usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:151:in `run'
 /usr/lib/ruby/vendor_ruby/rubygems/gem_runner.rb:52:in `run'
 /usr/bin/gem:12:in `<main>'
Katya@ubuntu:~/Ekaterina06-choi/workspace$ sudo gem install mygem
Fetching mygem-0.0.1.gem
Successfully installed mygem-0.0.1
Parsing documentation for mygem-0.0.1
Installing ri documentation for mygem-0.0.1
Done installing documentation for mygem after 0 seconds
1 gem installed
Katya@ubuntu:~/Ekaterina06-choi/workspace$ gem install gist
ERROR:  While executing gem ... (Gem::FilePermissionError)
    You don't have write permissions for the /var/lib/gems/3.3.0 directory.
 /usr/lib/ruby/vendor_ruby/rubygems/installer.rb:713:in `verify_gem_home'
 /usr/lib/ruby/vendor_ruby/rubygems/installer.rb:903:in `pre_install_checks'
 /usr/lib/ruby/vendor_ruby/rubygems/installer.rb:303:in `install'
 /usr/lib/ruby/vendor_ruby/rubygems/resolver/specification.rb:105:in `install'
 /usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:195:in `block in install'
 /usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:183:in `each'
 /usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:183:in `install'
 /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:215:in `install_gem'
 /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:231:in `block in install_gems'
 /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:224:in `each'
 /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:224:in `install_gems'
 /usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:170:in `execute'
 /usr/lib/ruby/vendor_ruby/rubygems/command.rb:328:in `invoke_with_build_args'
 /usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:253:in `invoke_command'
 /usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:193:in `process_args'
 /usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:151:in `run'
 /usr/lib/ruby/vendor_ruby/rubygems/gem_runner.rb:52:in `run'
 /usr/bin/gem:12:in `<main>'
Katya@ubuntu:~/Ekaterina06-choi/workspace$ sudo gem install gist
Fetching gist-6.0.0.gem
Successfully installed gist-6.0.0
Parsing documentation for gist-6.0.0
Installing ri documentation for gist-6.0.0
Done installing documentation for gist after 0 seconds
1 gem installed
Katya@ubuntu:~/Ekaterina06-choi/workspace$ (umask 0077 && echo ${GIST_TOKEN} > ~/.gist)
