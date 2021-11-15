# BAZEL



mkdir test

touch WORKSPACE

mkdir mydir

cd mydir 

touch BUILD
cc_binary
(
name="myname",
srcs=["myfile.cc"],
)

touch myfile.cc
#include<iostream>

int main()
{
	std:: cout <<"Mytext"<< std::endl;

}
	

TO build 
bazel build ...  //Current Directory 
bazel build //mydir:myname //Prev Directory 
	
	
To Run 
./bazel-bin/mydir/myname
