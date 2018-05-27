## Stops the miner on your machine

### Usage
```bash
vdhost stop-miner GPU_ID
```

### Options
| Name, shorthand | Default | Description |
| --------------- | ------- | ----------- |
| GPU_ID |      | ID of the GPU. |

### Description
Use this command to stop the miner on your machine. You must have first executed `vdhost start-miner GPU_ID` for this command to work.


### Example
```bash
$ vdhost stop-miner 0
Stopping the mining process now...
```
