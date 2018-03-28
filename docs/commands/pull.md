## Transfer files from Vectordash machine via SCP.

### Usage
```bash
vectordash pull MACHINE_ID FROM_PATH TO_PATH
```

### Options
| Name, shorthand | Default | Description |
| --------------- | ------- | ----------- |
| MACHINE_ID |      | ID number of machine to connect to. |
| FROM_PATH |      | Path of local file or directory. |
| TO_PATH | . | Path to remote Vectordash machine directory. Defaults to current directory. |

### Description
Use this command to transfer files/directories from a rented Vectordash machine to your local machine. The `MACHINE_ID` can be found by running `vectordash list`. 


### Example
```bash
$ vectordash pull 3 
Machine exists...
Executing scp -i key ...
```
