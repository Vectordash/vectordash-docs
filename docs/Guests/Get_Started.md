# Getting Started

Register by creating an account at [Vectordash](https://vectordash.com/)! Confirm your email and fill out some personal information. Navigate through the pages to understand our service and Terms & Conditions.  


## Dear guests

To use Vectordash CLI, you must install it on your machine. For Mac, Linux, and Windows machines, you can install it through  `pip`. You must first install `pip` if you have not already done so. We recommend using `pip3`, however, the `pip` is also fine.


#### Python 2.7

`sudo apt-get install python-pip`

`pip install vectordash --upgrade`


#### Python 3

`sudo apt-get install python3-pip`

`pip3 install vectordash --upgrade`


Visit the [vectordash-cli github](https://github.com/Vectordash/vectordash-cli) for the Vectordash Host source code.


## Account Configuration

In order to be able to connect to your rented machines, you have to first configure your account secret key on your machine. To do so, create an account, verify your email address, and log in to Vectordash. 

*Our users have reported some issues with some domain email addresses. We are working on finding a solution but in the meantime, we recommend using a gmail email address.*

Navigate to the [verification page](https://vectordash.com/edit/verification/) to find your current secret key, or generate a new one. To store the token on your machine, copy the token from the page and run the following command on your machine:

`vectordash secret <token>`

You have successfully configured your machine with your Vectordash account. You can now see the instances you are using and interact with them using the vectordash commands. Please note that you will have to run the above command after every time you have generated a new secret key. 

For a more detailed explanation of each vectordash command, please visit the commands section.


** If you encounter any issues, please feel free to email us at [contact@vectordash.com](mailto:contact@vectordash.com).