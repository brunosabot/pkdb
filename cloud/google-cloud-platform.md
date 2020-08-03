# Google Cloud Platform

## Contents

 - [Config - List and change zone](#config_list_and_change_zone)

## <a name="config_list_and_change_zone"></a>Config - List and change zone

List all available zone (might be filtered with grep)

```shell
gcloud compute zones list
gcloud compute zones list | grep us-central1
```

Change the zone by updating the config
```shell
gcloud config set compute/zone us-central1-c
```

## <a name="compute_create_vm"></a>Compute engine - Create a VM

VM can be created with gcloud compute instances.
- `--image-project`: The project against which all image and image family references will be resolved
- `--image`: Specifies the boot image for the instances
- `--machine-type`: Specifies the machine type used for the instances (`gcloud compute machine-types list`)
- `--subnet`: The subnet where we want to be attached (default: default)

```shell
gcloud compute instances create "my-vm-2" \
  --machine-type "n1-standard-1" \
  --image-project "debian-cloud" \
  --image "debian-9-stretch-v20170918" \
  --subnet "default"
```
