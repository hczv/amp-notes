
# Notes about minecraft servers hosted on AMP

## Setup Resource pack on server

Go to server settings

`configuration/Server Settings`

![](img/resource-pack.png)

1. Insret the direct download url for the resource pack into `Resource Pack URL`

2. The 2nd field `Resource Pack Hash` is for a [SHA1 hash](https://brilliant.org/wiki/secure-hashing-algorithms/) of the resource pack.
   This is used by the client to verify that it has downloaded the correct file.

To calculate the SHA1 hash do the following:

1. Download the resource pack
2. Go to [SHA1 File Checksum](https://emn178.github.io/online-tools/sha1_checksum.html)
3. Upload the resource pack to the site
4. The resulting seemingly random string of letters and numbers is the SHA1 hash, and should be copied to the `Resource Pack Hash` field

![](img/sha1-sum2.png)


---

# Troubleshooting

## 1. Cannot connect to running server

Some servers may experience running but no users being able to connect,

check the console:

![](img/arrow-console.png)

And check if the following is located in the log:

![](img/unable-to-access-address-of-buffer.png)

If so, a fix is to disable 'Use-Native-Transport' option on the server, this option

Go to `Configuration/Server Settings`

And ensure that this option is disabled:

![](img/use-native-transport.png)

Now restart the server, and connect to the server.

---