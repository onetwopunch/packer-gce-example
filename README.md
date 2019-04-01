# Packer GCE Example

This repo includes a packer build template to build a GCE image with a the Hello World example from Nginx for Docker: https://github.com/nginxinc/NGINX-Demos/tree/master/nginx-hello

This example illustrates how you can pass in variables into the packer script.

`WARNING: Never pass in secrets or sensitive configuration data into a Packer build as this will bake in your secrets into the image.`

To run create a JSON file called `vars.json` with the following format to pass in your own variables:

```
{
    "project_id" : "my-project",
    "zone" : "us-west2-a"
}

```

Then to execute a packer build:

```
packer build -var-file vars.json template.json
```