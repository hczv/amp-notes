
# Notes about fixes on minecraft servers hosted on AMP


## 1. Cannot connect to running server

Some servers may experience running but no users being able to connect,

check the console:

![](img/arrow-console.png)

And check if the following is located in the log:

![](img/unable-to-access-address-of-buffer.png)

If so, a fix is to disable 'Use-Native-Transport' option on the server, this option

Go to `configuration/Server Settings`

![](img/arrow-configuration.png)

![](img/arrow-server-settings.png)

And ensure that this option is disabled:

![](img/use-native-transport.png)

Now restart the server, and connect to the server.
