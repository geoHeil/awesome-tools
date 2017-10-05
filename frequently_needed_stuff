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
