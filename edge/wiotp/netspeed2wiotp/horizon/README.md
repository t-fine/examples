This directory contains an input file template to create a Horizon Exchange workload definition for the netspeed2wiotp docker image.

Fill in the values of the variables in the template with commands like:

```
export DOCKER_HUB_ID=openhorizon   # or your own docker hub id
export ARCH2=amd64    # or arm or arm64
export NETSPEED2WIOTP_VERSION=2.6.1
export HZN_ORG_ID=abcdef
export WIOTP_DOMAIN=internetofthings.ibmcloud.com

envsubst < netspeed2wiotp-template.json > netspeed2wiotp.json
```
