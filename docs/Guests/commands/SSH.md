## Connect to Vectordash machine via SSH.

### Usage
```bash
vectordash ssh MACHINE_ID
```

### Options
| Name, shorthand | Default | Description |
| --------------- | ------- | ----------- |
| MACHINE_ID |      | ID number of machine to connect to. |

### Description
Use this command to connect to a rented Vectordash machine. The `MACHINE_ID` can be found by running `vectordash list`. 


### Example
```bash
$ vectordash ssh 4
Machine exists. Connecting...
Executing ssh ...
```
