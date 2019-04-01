# Packer GCE Example

This repo includes a packer build template to build a GCE image with a the Hello World example from Nginx for Docker: https://github.com/nginxinc/NGINX-Demos/tree/master/nginx-hello

This example illustrates how you can pass in variables into the packer script.

`WARNING: Never pass in secrets or sensitive configuration data into a Packer build as this will bake in your secrets into the image.`