# Commands
Below, you can find specific documentation on the Vectordash-CLI commands. These commands allow you to interact with your rented Vectordash GPU instances. 

## List
```bash
vectordash list
```

Use this command to list all of the machines and their ID numbers you are currently renting. You will need to have run `vectordash secret SECRET_TOKEN` beforehand.

#### Example
```bash
$ vectordash list
[1] Vectordash Origin
[2] Tensorbox
[3] Mining Rig
```


## Pull
```bash
vectordash pull MACHINE_ID FROM_PATH TO_PATH
```

| Name, shorthand | Default | Description |
| --------------- | ------- | ----------- |
| MACHINE_ID |      | ID number of machine to pull files from. |
| FROM_PATH |      | Path to remote Vectordash machine directory. |
| TO_PATH | . | Path of local file or directory. Defaults to current directory. |


Use this command to transfer files/directories from a rented Vectordash machine to your local machine. The `MACHINE_ID` can be found by running `vectordash list`. 

#### Example
```bash
$ vectordash pull 3 
Machine exists...
Executing scp -i key ...
```


## Push
```bash
vectordash push MACHINE_ID FROM_PATH TO_PATH
```

| Name, shorthand | Default | Description |
| --------------- | ------- | ----------- |
| MACHINE_ID |      | ID number of machine to push files to. |
| FROM_PATH |      | Path of local file or directory. |
| TO_PATH | ~ | Path to remote Vectordash machine directory. Defaults to home directory. |


Use this command to transfer files/directories from your local machine to a rented Vectordash machine. The `MACHINE_ID` can be found by running `vectordash list`. 

#### Example
```bash
$ vectordash push 2 
Machine exists...
Executing scp -i key ...
```


## Secret
```bash
vectordash secret SECRET_TOKEN
```

| Name, shorthand | Default | Description |
| --------------- | ------- | ----------- |
| SECRET_TOKEN |      | Secret key of the user. |


Use this command to locally store the user's secret token in order to be able to do any of the other vectordash commands. If a previous token had been stored, this will replace it with the new token.

#### Example
```bash
$ vectordash secret t3st5ecretw0rd
Secret successfully updated.
```


## SSH
```bash
vectordash ssh MACHINE_ID
```

| Name, shorthand | Default | Description |
| --------------- | ------- | ----------- |
| MACHINE_ID |      | ID number of machine to connect to. |


Use this command to connect to a rented Vectordash machine. The `MACHINE_ID` can be found by running `vectordash list`. 

#### Example
```bash
$ vectordash ssh 4
Machine exists. Connecting...
Executing ssh ...
```



