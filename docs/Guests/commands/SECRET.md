## Store the Vectordash secret token.

### Usage
```bash
vectordash secret SECRET_TOKEN
```

### Options
| Name, shorthand | Default | Description |
| --------------- | ------- | ----------- |
| SECRET_TOKEN |      | Secret key of the user. |

### Description
Use this command to locally store the user's secret token in order to be able to do any of the other vectordash commands. If a previous token had been stored, this will replace it with the new token.


### Example
```bash
$ vectordash secret t3st5ecretw0rd
Secret successfully updated.
```
