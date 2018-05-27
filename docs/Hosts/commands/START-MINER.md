## Runs the miner of your choice on your machine

### Usage
```bash
vdhost start-miner GPU_ID
```

### Options
| Name, shorthand | Default | Description |
| --------------- | ------- | ----------- |
| GPU_ID |      | ID of the GPU. |


### Description
Use this command to run the miner on your machine. You must have first executed the following command: 

`vdhost set-commands GPU_ID`

before running the start-miner command. 


### Example
```bash
$ vdhost start-miner 0
Running the miner...
```
