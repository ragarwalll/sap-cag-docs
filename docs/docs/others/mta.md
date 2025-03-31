### About

If you choose `cloud deployment`, an `mta.yaml` file will be automatically generated, containing all the necessary configurations for the selected packages, including any required destinations. To generate a deployable `*.mtar` (Multi-Target Application Archive) file for `SAP BTP` (Business Technology Platform), you can easily build it.

If XSUAA is selected, a `xs-security.json` file will also be generated

### Usage Instructions

!!! note "Before Building"
    
    Please make sure you have the `mbt` installed in you PC. You can also use `npm i -g mbt` to install  

To build a deployable `MTAR`, simply run
```console
mbt build
```

!!! note "Before Deploying"
    
    Please make sure you have the `cf` installed in you PC. You can also use [link](https://github.com/cloudfoundry/cli/releases) to download & install

To deploy the `MTAR` to `SAP BTP`, simply run
```console
cf deploy mta_archives/<file_name>.mtar
```