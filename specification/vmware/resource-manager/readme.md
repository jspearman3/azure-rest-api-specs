# VMware Solution

> see https://aka.ms/autorest

This is the AutoRest configuration file for VMware Solution.

## Getting Started
To build the SDK for VMware Solution, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`
---

## Configuration

### Basic Information
These are the global settings for the VMware Solution API.

``` yaml
openapi-type: arm
tag: package-2019-08-09-preview
```

### Tag: package-2019-08-09-preview

These settings apply only when `--tag=package-2019-08-09-preview` is specified on the command line.

``` yaml $(tag) == 'package-2019-08-09-preview'
input-file:
- Microsoft.AVS/preview/2019-08-09-preview/vmware.json
```

---
# Code Generation

## Swagger to SDK

This section describes what SDK should be generated by the automatic system.
This is not used by Autorest itself.

``` yaml $(swagger-to-sdk)
swagger-to-sdk:
  - repo: azure-sdk-for-js
  - repo: azure-sdk-for-python
  - repo: azure-sdk-for-net
```

## TypeScript

See configuration in [readme.typescript.md](./readme.typescript.md)

## Python

See configuration in [readme.python.md](./readme.python.md)

## C#

See configuration in [readme.csharp.md](./readme.csharp.md)
## Multi-API/Profile support for AutoRest v3 generators 

AutoRest V3 generators require the use of `--tag=all-api-versions` to select api files.

This block is updated by an automatic script. Edits may be lost!

``` yaml $(tag) == 'all-api-versions' /* autogenerated */
# include the azure profile definitions from the standard location
require: $(this-folder)/../../../profiles/readme.md

# all the input files across all versions
input-file:
  - $(this-folder)/Microsoft.AVS/preview/2019-08-09-preview/vmware.json

```

If there are files that should not be in the `all-api-versions` set, 
uncomment the  `exclude-file` section below and add the file paths.

``` yaml $(tag) == 'all-api-versions'
#exclude-file: 
#  - $(this-folder)/Microsoft.Example/stable/2010-01-01/somefile.json
```
