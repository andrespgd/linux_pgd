# LINUX COMMANDS

List all attached drives
```
sudo lsblk -o NAME,FSTYPE,SIZE,MOUNTPOINT,LABEL
```

Find a folder
```
find / -xdev 2>/dev/null -name "GeographicLib"
```

Count # files
```
ls -l *jpeg | wc -l
```

RM recursively delete folders or files by name
```
rm -rf `find -type d -name tmp*`
rm -rf `find -type f -name *.csv`
```

Remove characters from filenames
ex: will remove the "(" character from all files
```
for file in *; do mv "${file}" "${file/"("/}"; done
```
ex: will find empty spaces and replace them for _ character
```
for file in *; do mv "${file}" "${file/" "/"_"}"; done
```

APT-GET update
```
sudo apt-get update
sudo apt-get upgrade
sudo apt-get dist-upgrade
sudo apt-get autoremove
```

PIP upgrade version
```
sudo -H pip install --upgrade pip
```

CURL lets you use wildcards to specify the URLs you want to download
```
curl -L https://s3-us-west-1.amazonaws.com/udacity-robotics/Term+2+Resources/P3+Resources/models.tar.gz | tar zx -C ~/.gazebo/
```

WGET can be used recursively and can recover when a download fails
```
https://github.com/andrespgd/linux_pgd/edit/master/README.md
```

List all available HDDs/Partitions
```
sudo lsblk -o NAME,FSTYPE,SIZE,MOUNTPOINT,LABEL
```

GIT setup account
```
sudo apt-get update
sudo apt-get install git
git config --global user.name  "Your Name"
git config --global user.email "youremail@domain.com"
git config --list
```

BASH previous commands execution
```
CTRL-R   and   type nmap   and  start typing
ex.
CTRL-R  , type nmap, type git....
```

Find a word inside a file in a directory
```
grep -r word_on_file *
OR
grep -rnw -e 'word_on_file'
```

# UBUNTU

UBUNTU install notepad-plus-plus</br>
-set alias on .bashrc to npp

UBUNTU install nano text editor
```
sudo apt install nano
```

UBUNTU install screen recorder
```
sudo add-apt-repository ppa:fossproject/ppa
sudo apt update
sudo apt install green-recorder
```

UBUNTU install conda</br>
https://github.com/andrespgd/python_pgd/blob/master/_CONDA_README.md


UBUNTU Screenshot shortcuts (pre-installed)
```
Prt Scrn - desktop.
Alt+Prt Scrn - window.
Shift+Prt Scrn - area you select.
```
