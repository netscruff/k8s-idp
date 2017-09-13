## IdP deployment

All k8s assets for deployment are here except for a secret for the keystore
password. You can create this using the following template command. Password
is contained within the file.

kubectl create secret generic ccidp-keystore --from-file=./JETTY_BACKCHANNEL_SSL_KEYSTORE_PASSWORD
