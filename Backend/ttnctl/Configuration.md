# TTNCTL Configuration

The `ttnctl` program can be configured with command line options described in the [[ttnctl documentation|Backend/ttnctl/ttnctl]], with environment variables or with a configuration file.

## Environment

`ttnctl` can be configured using environment variables.
The format of these variables is the underscored version of the command line options that can be found in the [[ttnctl documentation|Backend/ttnctl/ttnctl]]. Environment variables are uppercase. The environment variables shown below are the default values, if these work for you, you don't have to set them.

```sh
export DEBUG=true
export TTN_ROUTER=localhost:1700
export APP_EUI=0102030405060708
export MQTT_BROKER=localhost:1883
export TTN_HANDLER=0.0.0.0:1782
export APP_TOKEN=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJUVE4tSEFORExFUi0xIiwiaXNzIjoiVGhlVGhpbmdzVGhlTmV0d29yayIsInN1YiI6IjAxMDIwMzA0MDUwNjA3MDgifQ. Qj672lwwDVmfYshpMvPwm6A8oNWJ7teGS2A
```

###### Updated on 24-Mar-2016

## Configuration File

A configuration file can be specified using the `--config` option. By default, `ttnctl` looks for the file `~/.ttnctl.yaml` (in your home directory).
The configuration file shown below contains the default values, if these work for you, you don't have to set them.

```yaml
debug: true
ttn-router: "localhost:1700"
app-eui: "0102030405060708"
mqtt-broker: "localhost:1883"
ttn-handler: "0.0.0.0:1782"
app-token: "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJUVE4tSEFORExFUi0xIiwiaXNzIjoiVGhlVGhpbmdzVGhlTmV0d29yayIsInN1YiI6IjAxMDIwMzA0MDUwNjA3MDgifQ.zMHNXAVgQj672lwwDVmfYshpMvPwm6A8oNWJ7teGS2A"

```

###### Updated on 24-Mar-2016