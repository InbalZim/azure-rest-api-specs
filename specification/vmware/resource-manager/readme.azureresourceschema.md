## AzureResourceSchema

These settings apply only when `--azureresourceschema` is specified on the command line.

### AzureResourceSchema multi-api

``` yaml $(azureresourceschema) && $(multiapi)
batch:
  - tag: package-2020-03-20
  - tag: package-2019-08-09-preview
```

### Tag: package-2020-03-20 and azureresourceschema

These settings apply only when `--tag=package-2020-03-20 --azureresourceschema` is specified on the command line.
Please also specify `--azureresourceschema-folder=<path to the root directory of your azure-resource-manager-schemas clone>`.

``` yaml $(tag) == 'package-2020-03-20' && $(azureresourceschema)
output-folder: $(azureresourceschema-folder)/schemas
```

### Tag: package-2019-08-09-preview and azureresourceschema

These settings apply only when `--tag=package-2019-08-09-preview --azureresourceschema` is specified on the command line.
Please also specify `--azureresourceschema-folder=<path to the root directory of your azure-resource-manager-schemas clone>`.

``` yaml $(tag) == 'package-2019-08-09-preview' && $(azureresourceschema)
output-folder: $(azureresourceschema-folder)/schemas
```

