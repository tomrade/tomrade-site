# IIS Stuff

## Docker Container

If you are using a docker container for IIS , dont forget to use "logmonitor" from microsoft in order to echo the web logs to STDOUT for docker or map the log directory. You can do this by using a dockerfile and the "SHELL" command. 

* [](https://github.com/microsoft/windows-container-tools/tree/master/LogMonitor)