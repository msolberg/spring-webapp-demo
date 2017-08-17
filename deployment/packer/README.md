This directory contains packer templates for building OpenStack images. The following templates are available:

  * [image.json](image.json) - This template will build an image using the shell and file packer provisioners.
  * [image-ansible.json](image-ansible.json) - This template will build an image using the ansible provisioner.

To use these, source your openrc.sh, set the satellite server variables in [variables.json](variables.json) and build it like so:

```
packer build --var-file variables.json image.json
```
