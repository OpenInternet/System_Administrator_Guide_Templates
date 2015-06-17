# System_Administrator_Guide_Templates

Publication templates for the System Administrator Guide

# Building the System Administrator Guide PDF

### Install Git

```
sudo apt-get install git
```

### Install [pretty markdown to pdf](https://github.com/elationfoundation/pretty_md2pdf)

[Use the installation instructions found here.](https://github.com/elationfoundation/pretty_md2pdf/blob/master/docs/INSTALL.md)

### Download the [System Administrator Guide Text](https://github.com/OpenInternet/System_Administrator_Guide_Text)

```
git clone https://github.com/OpenInternet/System_Administrator_Guide_Text.git
```
### Download and Install the [System Administrator Guide Theme Templates](https://github.com/OpenInternet/System_Administrator_Guide_Templates)

```
git clone https://github.com/OpenInternet/System_Administrator_Guide_Templates.git
cd System_Administrator_Guide_Templates
./install
cd ..
```

### Create the System Administrator Guide

```
./pretty_md2pdf/builddoc -i System_Administrator_Guide_Text/en/ -t System_Administrator_Guide_Templates/ -o SysAdminGuide.pdf
```
