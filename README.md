## IdP deployment

All k8s assets for deployment are here except for a secret for the keystore
password. You can create this using the following template

apiVersion: v1
kind: Secret
metadata:
  name: ccidp-keystore
data:
  backchannel_ssl_keystore_password: changeme
