# Getting Started

Register by creating an account at [Vectordash](http://vectordash.com/)! Confirm your email and fill out some personal information. Navigate through the pages to understand our service and [Terms and Conditions](http://vectordash.com/terms/). 


## Dear hosts

As of now, we only support Ubuntu 16.04 machines. To use Vectordash Host, you must install it on your machine. In Ubuntu 16.04, you can install it through  `pip`. You must first install `pip` if you have not already done so. We recommend using `pip3`, however, the `pip` is also fine.


#### Python 2.7

`sudo apt-get install python-pip`

`pip install vdhost --upgrade`


#### Python 3

`sudo apt-get install python3-pip`

`pip3 install vdhost --upgrade`


## Host Configuration

Now that you have downloaded the python package, it is time to configure your machine for onboarding to Vectordash. Please make sure you follow the instructions properly. If you do not execute them as instructed, there may be an issue with your machine that will delay the process of listing your machine on our site. 


#### Installing Dependencies

First, you must install all required dependencies. Download the vectordash-host tarball from [here](https://vectordash.com/verified_hosts). Please note, you will not be able to access these dependencies until AFTER you have become a verified host. 

When you have downloaded the vectordash-host.tgz file, navigate to the directory it is in. Then run the following commands:


`dpkg -i vectordash-host.tgz`

`cd vectordash-host/`

`vdhost install`


If any prompts come up on the screen, simply hit ENTER or select the default value. The installation script should take a few minutes. Please do not interrupt the installation script, or you will have to start over. 

After the installation script is finished, it will ask you to reboot your machine. Please save all of your data before rebooting. Once you have saved and backed up all of your data, run the following command:

`sudo reboot`


## List the machines

When you successfully complete the steps above, you are ready to list your machines. Simply run:

`vdhost start-hosting`

This will launch the client script and bring your machine online for communication with Vectordash!


#### Set GPU IDs

The last step is simple. You must tell Vectordash which GPUs you want to list on the site. Your machine must have the appropriate upload/download speeds. Each GPU must have the appropriate RAM, SSD, and CPU.

You must determine what GPUs you would like to list on Vectordash. To do this, go to the [host dashboard](http://vectordash.com/machines) and click on the machine whose GPUs you want to add to Vectordash. Select done.

Your machine and GPUs should now be listed!



** If you encounter any issues, please feel free to email us at [contact@vectordash.com](mailto:contact@vectordash.com).