# BAZEL


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
