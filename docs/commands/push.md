## Transfer files to Vectordash machine via SCP.

### Usage
```bash
vectordash push MACHINE_ID FROM_PATH TO_PATH
```

### Options
| Name, shorthand | Default | Description |
| --------------- | ------- | ----------- |
| MACHINE_ID |      | ID number of machine to connect to. |
| FROM_PATH |      | Path of local file or directory. |
| TO_PATH | ~ | Path to remote Vectordash machine directory. Defaults to home directory. |

### Description
Use this command to transfer files/directories from your local machine to a rented Vectordash machine. The `MACHINE_ID` can be found by running `vectordash list`. 


### Example
```bash
$ vectordash push 2 
Machine exists...
Executing scp -i key ...
```
