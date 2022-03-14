# BAZEL

```bash
sudo apt update
sudo apt install python3-dev python3-pip
pip3 install -U --user pip numpy wheel
pip3 install -U --user keras_preprocessing --no-deps


Add Bazel distribution URI as a package source
sudo apt install curl gnupg
curl -fsSL https://bazel.build/bazel-release.pub.gpg | gpg --dearmor > bazel.gpg
sudo mv bazel.gpg /etc/apt/trusted.gpg.d/
echo "deb [arch=amd64] https://storage.googleapis.com/bazel-apt stable jdk1.8" | sudo tee /etc/apt/sources.list.d/bazel.list

Install and update Bazel
sudo apt update && sudo apt install bazel
sudo apt update && sudo apt full-upgrade
sudo apt install bazel-1.0.0

bazel --version # 1.0.0

```



```bash
mkdir test
```
```bash
touch WORKSPACE
```
```bash
mkdir mydir
```
```bash
cd mydir 
```
Create a BUILD file
```bash
touch BUILD
cc_binary
(
name="myname",
srcs=["myfile.cc"],
)
```
Create a cpp file
```bash
touch myfile.cc
#include<iostream>

int main()
{
	std:: cout <<"Mytext"<< std::endl;

}
```

To build 
```bash	
bazel build ...  //Current Directory 
bazel build //mydir:myname //Prev Directory 
```	
	
To Run
```bash	
./bazel-bin/mydir/myname
```
