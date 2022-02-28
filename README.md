# LinuxLearnings
# Yum related points
cd /etc/yum.repos.d/

# will show you all packages available with tomcat in the name
sudo yum search tomcat

# find out from where this tomcat is installed from
repoquery -i tomcat
 
# list of yum repos available for packages to get downloaded from
yum repolist -v enabled

# get just the url info from yum repo list
yum repolist -v enabled | grep Repo-baseurl | cut -d\  -f 3
