[[#update]]
[[#1 ubuntu software]]
[[ubuntu_int#2 site download]]
### ubuntu install - it-lab-x230
#### 1. ubuntu software
- VS code

#### 2. site download
- sidekick-linux-release-x64-88.8.44.8933-b349f4a.deb

#### 3. net-tools & ibus-Rime

```
sudo apt install net-tools
sudo apt-get install ibus-rime
```
- IBUS-RIME need restart the system,then language setting 

#### 4. install ZSH 
ref: https://medium.com/@wifferlin0505/%E5%9C%A8-ubuntu-16-04-lts-%E4%B8%AD%E5%AE%89%E8%A3%9D%E4%BD%BF%E7%94%A8-oh-my-zsh-cf92203ca8a2
```
sudo apt-get install zsh
sudo apt install git
cat /etc/shells
sudo apt install curl
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

```
Download 
https://raw.githubusercontent.com/caiogondim/bullet-train-oh-my-zsh-theme/master/bullet-train.zsh-theme

```
# back home folder
$cd
# move file
$sudo mv Downloads/bullet-train.zsh-theme .oh-my-zsh/themes/


$sudo nano .zshrc
# ZSH_THEME 修改成 “bullet-train”

```
install fonts
```
$sudo apt-get install powerline
$sudo apt-get install fonts-powerline
```
#### 5. snap
ref:https://www.howtoforge.com/ubuntu_snap/#install-snap

```
sudo snap install /home/it/Downloads/obsidian_0.11.13_amd64.snap --dangerous
```

#### 6. deb
```
sudo dpkg -i 軟體套件名.deb

sudo apt-get remove 軟體套件名稱
```
-----------
#### ubuntu_install 
Date: Apr'19'2021
```
sudo dpkg -i code_1.55.2-1618307277_amd64.deb
lsb_release -a #check the vesion 
sudo apt install net-tools
sidekick-linux-release-x64-88.8.44.8933-b349f4a.deb
sudo apt-get update && sudo apt-get upgrade
sudo apt install curl
sudo apt install git
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

```

[Ubuntu 20.04 need done](https://tw511.com/a/01/885.html)
[ZSH install](https://medium.com/@wifferlin0505/%E5%9C%A8-ubuntu-16-04-lts-%E4%B8%AD%E5%AE%89%E8%A3%9D%E4%BD%BF%E7%94%A8-oh-my-zsh-cf92203ca8a2)
####  Ptython @Ubuntu
VENV
> sudo apt-get install python3-venv

> mkdir pyven
```
python3 -m venv pytest
cd pytest
source bin/activate
deactivate
wget https://bootstrap.pypa.io/get-pip.py
python3 
get-pip.py
pip3 -V
python -m pip install ipykernel --force    	
````

#### update
sudo apt-get update && sudo apt-get -y dist-upgrade && sudo apt-get clean

#### R & Rstudio
> https://cran.csie.ntu.edu.tw/

> https://www.rstudio.com/products/rstudio/download/#download


```
sh: 1: make: not found
Warning in system(cmd) : error in running command
ERROR: compilation failed for package ‘mime’
```

>sudo apt-get install build-essential

```
Perhaps you should add the directory containing `libcurl.pc'
to the PKG_CONFIG_PATH environment variable
No package 'libcurl' found
Package libcurl was not found in the pkg-config search path.
Perhaps you should add the directory containing `libcurl.pc'
to the PKG_CONFIG_PATH environment variable
No package 'libcurl' found
Using PKG_CFLAGS=
Using PKG_LIBS=-lcurl
```
> sudo apt-get install libcurl4-openssl-dev

```
heaven package
readstat/spss/readstat_zsav_compress.o] Error 1

```

>sudo apt-get install zlib1g-dev

> sudo apt-getinstall libssl-dev 
lot of dep was failed to install ,when install.packages("bibliometrix")
install.packages("stringi")

sudo apt-get install r-cran-rcppeigen

sudo apt-get install r-cran-RcppArmadillo

```
sudo apt-get install gfortran
sudo apt-get install libxml2-dev
sudo apt-get install lib\*-dev


```

https://andy6804tw.github.io/2019/09/23/ubuntu-indtall-nodejs/

https://blog.csdn.net/masterbee/article/details/85205956
精辟！！/usr/bin/ld: cannot find -l\* 问题的解决方法
 /usr/bin/ld: cannot find -l\*
  sudo apt-get install lib\*-dev

```

sudo apt-get install -y nodejs
node -v
sudo apt-get install npm```
npm -v

```

#### Latex & pandoc for zettlr
sudo apt install texlive-latex-extra

```shell
$ sudo apt install texlive-base texlive-xetex # for Debian-based distributions
```

pandoc-2.14.0.1-1-amd64.deb
 
Font lost:
sudo apt-get install ttf-mscorefonts-installer

#### Drawio - desktop
https://github.com/jgraph/drawio-desktop

#### git

git clone --recursive https://github.com/jgraph/drawio-desktop.git

https://github.com/jgraph/drawio-desktop


```
rclone mount remote:path/to/files /path/to/local/mount
```

```
rclone mount phvibox:data /home/it/Documents/box_data &&
rclone mount phvibox:md /home/it/Documents/box_md --allow-non-empty
```

rclone mount phvibox:md /home/it/Documents/box_md --allow-non-empty

```
rclone --vfs-cache-mode writes mount phvibox:it_lab ~/box

```


