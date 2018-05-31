# Getting Started

Welcome to [Vectordash](https://vectordash.com/) command line docs! Here you'll find information on how to interact with your Vectordash instances via the official Vectordash command line interface. We do our best to make this documentation clear and user friendly, but if you have unanswered questions, feel free to email us at [contact@vectordash.com](mailto:contact@vectordash.com).


The Vectordash command line interface is on open source on GitHub at [vectordash-cli](https://github.com/Vectordash/vectordash-cli). Feel free to submit a pull request or open an issue.


## Installation

The vectordash-cli library is installable via the Python package manager `pip`.


#### Install with Python 2
`pip install vectordash -U`


#### Install with Python 3
`pip3 install vectordash -U`


#### Authentication
To authenticate your client, retrieve your secret key from the [verification page](https://vectordash.com/edit/verification/) and save your key with the following command:

`vectordash secret <secret_key>`


## Usage
Here are the supported Vectordash commands which allow you to interact with your GPU instances via the command line. You will need to have entered a valid secret key beforehand.


## Listing your GPU instances
Use the list command to view all of your active GPU instances by ID and hostname.

```bash
vectordash list
```
#### Example
```bash
$ vectordash list
[1] tensorflow-convnet
[2] openai-gym
[3] fastai
```

## Connecting to an instance
Use this command to connect to one of your GPU instances via SSH without having to manually build an SSH command
or manage SSH keys.
Your instance's  `machine_id` can be found by running `vectordash list`.

```bash
vectordash ssh <machine_id>
```

| Name | Description |
| --------------- | ----------- |
| machine_id | ID number of machine to connect to via SSH. |




#### Example
```bash
$ vectordash ssh 1
Connecting via SSH to tensorflow-convnet...
```


## Sending files to an instance

Use this command to transfer files/directories from your local machine to a rented Vectordash machine. This builds an `scp` command for you under the hood. The `machine_id` can be found by running `vectordash list`.

```bash
vectordash push <machine_id> <from_path> <to_path>
```

| Name | Description |
| --------------- | ----------- |
| machine_id | ID number of machine to push files to. |
| from_path | Path of local file or directory. |
| to_path | Remove path on Vectordash instance. Defaults to the Ubuntu user's home directory. |


#### Example
```bash
$ vectordash push 2 train.py /home/ubuntu/scripts/
Copying data...
```



## Getting files from an instance

Use this command to transfer files/directories from a Vectordash instance to your local machine. This builds an `scp` command for you under the hood. The `machine_id` can be found by running `vectordash list`.

```bash
vectordash pull <machine_id> <from_path> <to_path>
```

| Name | Description |
| --------------- | ----------- |
| machine_id | ID number of machine to pull the files from. |
| from_path | Path located on the Vectordash instance. |
| to_path | Path of local file or directory. Defaults to the current directory. |




#### Example
```bash
$ vectordash pull 3 /home/ubuntu/model.dat ~/Desktop/
Copying data...
```

## Updating your secret key

Use this command to store your secret token for authentication.
If a previous token had been stored, it will be overwritten with the new token.
You can retrieve your token from the [verification page](https://vectordash.com/edit/verification/).

```bash
vectordash secret <secret_key>
```

| Name | Description |
| --------------- | ------- |
| secret_key | Your Vectordash account's secret token. |




#### Example
```bash
$ vectordash secret c0nv01utiOnaln3uraln3tw0rk
Secret successfully updated.
```
