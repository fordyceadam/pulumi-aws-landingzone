# pulumi-aws-landingzone
Create a landing zone in AWS using Pulumi

## Open in Gitpod

[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/fordyceadam/pulumi-aws-landingzone)

## Get started

### Install pulumi (could be installed when container is created)
```bash
curl -fsSL https://get.pulumi.com | sh
```

### Create new aws-python project
```
mkdir pulumi
cd pulumi
pulumi new aws-python
```
Setup notes:
 - Log into the pulumi dashboard and generate a token, enter it when prompted
 - The dialogue will take you through the settings that are required
 - I used eu-west-1
 - My environment is called `dev`

### Authorise AWS
```bash
export AWS_ACCESS_KEY_ID=<YOUR_ACCESS_KEY_ID>
export AWS_SECRET_ACCESS_KEY=<YOUR_SECRET_ACCESS_KEY>
```

### Deploy the code
```
pulumi up
```

# TODO

- Add AWS Credentials to the gitpod profile
- Install pulumi as part of the container build
- Add VSCode python plugin to the .gitpod.yaml configuration `@id:ms-python.python`
- Add Black Formatter python plugin to the .gidpod.yaml configuration `@id:ms-python.black-formatter`
- Add `@id:donjayamanne.python-extension-pack` to .gitpod.yaml configuration

# Author

Adam Fordyce - 2022