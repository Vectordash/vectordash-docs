## Sets the commands associated with the miner of your choice

### Usage
```bash
vdhost set-commands GPU_ID
```

### Options
| Name, shorthand | Default | Description |
| --------------- | ------- | ----------- |
| GPU_ID |               | ID of the GPU. |


### Description
Use this command to set the miner for a specific GPU. Please note, in order to run the miner on all GPUs on a machine, you must run this command for each GPU (id). 

This command will ask you to provide the absolute path to a bash script that starts the miner of your choice.  You will run `vdhost start-miner` afterwards to run your miner. 


### Example
```bash
$ vdhost set-commands 0
Please enter the path to a bash script that, 
when run, will start mining on the GPU with id 0:
```
