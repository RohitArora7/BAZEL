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

cd mydir 
```bash
touch BUILD
cc_binary
(
name="myname",
srcs=["myfile.cc"],
)
```
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
