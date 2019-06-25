# Unix like environments

## Port searching

- Find if a port is being used: `netstat -anp tcp | grep <portNumber`

- Find what application (along with PID) is using a port: `lsof -i tcp:<portNumber`
