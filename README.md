# rancher-utilities

 This repo contains some useful scripts to use with Rancher 2.
 For use them, you need python and rancher-cli binary file.

## copy-resources-between-projects

 This script allows to copy TLS certificates and Registries Credentials between two different Rancher projects.   
 It reads every resource for every namespace of the source project and copy it to the destination project.   
 The new resource will be created without namespace, so it will be available for all namespaces in the destination project.   

 Parameters:
 ```
  --server SERVER       Set rancher instance url
  --source SOURCE       Set the rancher project ID from where to read data
  --dest DEST           Set the rancher project ID to copy data
  --token TOKEN         Set the rancher auth token
  --rancher-path RANCHER_PATH
                        Set rancher binary path (default to ./rancher)
  --copy-mode COPY_MODE
                        Copy tls certificates, registries credentials or both. Accepted
                        values: tls, creds, all
```
