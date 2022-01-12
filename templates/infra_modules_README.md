# Module Name

### General

* Description:
* Created By:
* Module Dependencies:
  * Stuff
  * Goes
  * Here
* Provider Dependencies:
  * Stuff
  * Goes
  * Here
* Terraform Version:


### Usage

* Terragrunt (terragrunt.hcl example):
Module is referenced in a infra repo and can be then deployed to multiple accounts.

```hcl
locals {
  version = "v0.1.0"
}

terraform {
  source = "git::git@github.com:avenuebankau/infra-modules.git//module-name?ref=${local.version}"
}

inputs = {
  env     = "prod"
  service = "burrito"
}

```

### Options

* Description: Input variable options and Outputs for other modules to consume

#### Inputs

| Variable Name           | Description                        | Options             |  Type  | Required? | Notes |
| :---------------------- | :--------------------------------- | :------------------ | :----: | :-------: | :---- |
| env                     | unique environment name            | test/staging/prod   | string |    Yes    | N/A   |


#### Outputs

| Variable Name | Description            |  Type  | Notes |
| :------------ | :--------------------- | :----: | :---- |
| id            | unique id for resource | string | N/A   |

### Lessons Learned

* Stuff
* Goes
* Here


### References

* Stuff
* Goes
* Here
