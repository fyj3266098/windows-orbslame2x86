# windows-orbslam2-x6486

#orbslam2 on windows plantform.

windows-orbslam2 only use g2o and DBow2 library.To get my project more commonly used, i remove pangolin totally and due to 
the reason that gcc Compiler is not compatible with vc for exapmle :"int size = 100; int a[size]" this is OK only compiled
with gcc,i change those codes to "int *a = new int[size]." to make this project run successfully,i do not release those
memory cos You will always restart your execution file.In my project I build a useable project but not a demo.Later i will
update it.I need mention that in g2o i have ever come across internal error with vs2013,i make some tips to fix it.

I only compile successfully in x86 structure and this project only return R&T matrix of camera.If you has the need to use x64
structure, I think you can use shared memory to communicate with x64 project.(In my project ,i use x86 orbslam to deal with the images
which is get from zed camera that only has x64 sdk)

#Build Instructions

The orbslam2byfyj.sln solution should be built with Visual Studio 2013 or greater. 

#Requirements

Windows 10
Visual Studio 2013 or higher
opencv 2.4.9 or higher 

It is very disguiting to make g2o library as a depedency, so i add all the opensource code into my project.

For detailed information on this sample, please contract:fyjzjut@hotmail.com 
