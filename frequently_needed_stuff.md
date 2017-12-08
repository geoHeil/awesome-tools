# collection of frequently needed commands
## certificates
**get certifiacates and store in keystore**
```
# view certificates
openssl s_client -showcerts -connect my.host.com:443
# store desired ones to a file (myfile.pem)

# then base64 decode it
base64 -d myfile.pem > myfile.cer

# and add to keystore
keytool -import -alias gateway-identity -keystore mykeystore.jks -file myfile.cer
```


## spark
- assuming your cluster does not install all client code on each data node remember to ship hive-site.xml as well as the tez xml file when submitting a spark job in yarn cluster mode
- it might have worked just fine in yarn client - but will no longer work in yarn cluster without these files.
