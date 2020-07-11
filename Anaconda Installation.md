# How to install Anaconda on Ubuntu
This tutorial for installing Anaconda is written based on
[Anaconda Documentation!](https://docs.anaconda.com/anaconda/install/linux/)
.

1. Go to 
[this page!](https://www.anaconda.com/products/individual#linux) 
and download **Anaconda installer for Linux**.

The downloaded file will usually be place in your *Download* directory which will be addressed as
```sh
~/Downloads/
````
in what follws. If the file is placed in another directory, e.g. *Desktop* etc., then you would need to modify the address ( or simply cut and paste the file into 
```sh
~/Downloads/
````
directory.

2. Open a terminal *(ctrl + alt + t)*. You see something like this:
![Image of a terminal](https://github.com/Shenavar/pics/blob/master/1.jpg)
   1. To install Anaconda for **Python 3.7**, enter the following command in your terminal:
   >  bash ~/Downloads/Anaconda3-2020.02-Linux-x86_64.sh
   2. To install Anaconda for **Python 2.7**, enter the following command in your terminal:
   >  bash ~/Downloads/Anaconda2-2019.10-Linux-x86_64.sh
   
Because we need to run PLUTO code, you would need to install Anaconda for **Python 3.7**. So, you should run the first command in your terminal:
![Image of a terminal](https://github.com/Shenavar/pics/blob/master/2.jpg)


3. Then you would see the following message 
  > In order to continue the installation process, please review the license agreement.
  
  Click Enter to view license terms. Then, Scroll down to the bottom and enter **Yes** to accept the terms.
  
  
4. Next, the installer asks you to press **Enter** to accept the default install location. We strongly recommend you to choose the default install location. Specially, **Do not** choose the path as **/usr** for the Anaconda/Miniconda installation because you will be in trouble shortly!

After accepting the default directory, the installer shows the next message: 
> PREFIX=/home/<user>/anaconda<2 or 3>”
   
The installation process continues for a few minutes; then it will be completed.

5. You see the next message:
  > Do you wish the installer to initialize Anaconda3 by running conda init?
  
Write **yes**.  
  
