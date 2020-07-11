# How to install Anaconda on Ubuntu

This tutorial for installing **Anaconda** is written based on
[Anaconda Documentation](https://docs.anaconda.com/anaconda/install/linux/)
. To install **Anaconda**

1. Go to 
[this page](https://www.anaconda.com/products/individual#linux) 
and download **Anaconda installer for Linux**. If you are from Iran, and you encounter some problems in downloading this source file, you would have two options:

   1. Go to 
   [fumdrive](https://fumdrive.um.ac.ir/index.php/s/eFzf63ZHn8WPLqF) 
   and download Anaconda. This link is provided to you from **AstroGroup** of *Ferdowsi University of Mashhad*.
   
   2. Install an application for open internet such as *Lantern*. This is explained in detail below (See **Updating Anaconda**). Then download anaconda from the 
[this page](https://www.anaconda.com/products/individual#linux).

Once downloaded, the file will be usually placed in your *Download* directory which, in what follows, will be addressed as
```sh
~/Downloads/
````
If the file is placed in another directory, e.g. *Desktop* etc., then you would need to modify the address in the following commands. Or, you may simply cut and paste the file into *Downloads* directory.

2. Now, open a terminal by simply press *(ctrl + alt + t)* simultaneously. You see something like this:
![Image of a terminal](https://github.com/Shenavar/pics/blob/master/1.jpg)

The part 
```sh
hossein@Chortkeh2:~$
````
in green font, and on the top left, is my laptop's name! So, you would see something else instead. Now

   - To install Anaconda for **Python 3.7**, enter the following command in your terminal:
   >  bash ~/Downloads/Anaconda3-2020.02-Linux-x86_64.sh
   
   or
   
   - To install Anaconda for **Python 2.7**, enter the following command in your terminal:
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
  
6. The installer finishes by showing the next message:
  > Thank you for installing Anaconda 3
  
7. The installer provides a link to install **PyCharm** for Anaconda at https://www.anaconda.com/pycharm. However, installing **PyCharm** depends to you. We do not need **PyCharm** for this workshop.

# Updating Anaconda

This part is written based on
[Updating from older versions](https://docs.anaconda.com/anaconda/install/update-version/) from 
[Anaconda Documentation](https://docs.anaconda.com/anaconda/install/linux/)
.

To update anaconda to the latest version, you can simply run one of the following commands in your *terminal*:
> conda update conda

Or 

> conda update --all


In Iran, you will probably encounter some problems in updating or even installing Anaconda due to filtering. If so, we recommend you to install Lantern. To do so,

1. You need to have wget installed. If you don't have it, simply run:

> sudo apt-get install wget

2. Next, download the source of Lantern by running this command in your terminal:

> wget https://lantern.io/lantern-installer-64-bit.deb


3. Go to the directory which includes the downloaded file (usually Home directory ) and execute the following command in terminal:

> sudo apt install ./lantern-installer-64-bit.deb

Enter your *password* and Lantern will be installed. 

4. Once installed, you could update *Anaconda* by 

> conda update conda

Or 

> conda update --all

as mentioned above.

5. We strongly encourage you to read 
[Updating from older versions](https://docs.anaconda.com/anaconda/install/update-version/) 
to get familiar with other forms of updating Anaconda. You might need it some day.
