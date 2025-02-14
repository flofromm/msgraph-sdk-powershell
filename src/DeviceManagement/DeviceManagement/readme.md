<!-- region Generated -->
# Microsoft.Graph.DeviceManagement
This directory contains the PowerShell module for the Device service.

---
## Status
[![Microsoft.Graph.DeviceManagement](https://img.shields.io/powershellgallery/v/Microsoft.Graph.DeviceManagement.svg?style=flat-square&label=Microsoft.Graph.DeviceManagement "Microsoft.Graph.DeviceManagement")](https://www.powershellgallery.com/packages/Microsoft.Graph.DeviceManagement/)

## Info
- Modifiable: yes
- Generated: all
- Committed: yes
- Packaged: yes

---
## Detail
This module was primarily generated via [AutoRest](https://github.com/Azure/autorest) using the [PowerShell](https://github.com/Azure/autorest.powershell) extension.

## Development
For information on how to develop for `Microsoft.Graph.DeviceManagement`, see [how-to.md](how-to.md).
<!-- endregion -->

### AutoRest Configuration

> see https://aka.ms/autorest

``` yaml
require:
  - $(this-folder)/../../readme.graph.md
  - $(this-folder)/../../../profiles/$(title)/readme.md
title: $(service-name)
subject-prefix: ''
```

### Directives

> see https://github.com/Azure/autorest/blob/master/docs/powershell/directives.md

``` yaml
directive:
# Remove invalid paths.
  - remove-path-by-operation: ^deviceManagement.(deviceManagementScripts.userRunStates.deviceRunStates_.*|groupPolicyConfigurations.definitionValues.presentationValues_.*|deviceShellScripts.userRunStates.deviceRunStates_.*)$

# Remove cmdlets.
  - where:
      verb: New
      subject: ^DeviceManagement(Managed|Comanaged)DeviceLogCollectionRequest$
    remove: true
  - where:
      verb: Update
      subject: ^DeviceManagementComanagedDevice$
    remove: true

# Rename cmdlets.
  - where:
      subject: ^(DeviceManagementUserExperienceAnalyticAppHealthApplicationPerformance)$
      variant: ^Create1$|^CreateExpanded1$|^Get1$|^GetViaIdentity1$|^List1$|^Delete1$|^DeleteViaIdentity1$|^Update1$|^UpdateExpanded1$|^UpdateViaIdentity1$|^UpdateViaIdentityExpanded1$
    set:
      subject: $1ByAppVersion
  - where:
      subject: ^(DeviceManagementUserExperienceAnalyticAppHealthApplicationPerformance)$
      variant: ^Create2$|^CreateExpanded2$|^Get2$|^GetViaIdentity2$|^List2$|^Delete2$|^DeleteViaIdentity2$|^Update2$|^UpdateExpanded2$|^UpdateViaIdentity2$|^UpdateViaIdentityExpanded2$
    set:
      subject: $1ByAppVersionDetail
  - where:
      subject: ^(DeviceManagementUserExperienceAnalyticAppHealthApplicationPerformance)$
      variant: ^Create3$|^CreateExpanded3$|^Get3$|^GetViaIdentity3$|^List3$|^Delete3$|^DeleteViaIdentity3$|^Update3$|^UpdateExpanded3$|^UpdateViaIdentity3$|^UpdateViaIdentityExpanded3$
    set:
      subject: $1ByAppVersionDeviceId
  - where:
      subject: ^(DeviceManagementUserExperienceAnalyticAppHealthApplicationPerformance)$
      variant: ^Create4$|^CreateExpanded4$|^Get4$|^GetViaIdentity4$|^List4$|^Delete4$|^DeleteViaIdentity4$|^Update4$|^UpdateExpanded4$|^UpdateViaIdentity4$|^UpdateViaIdentityExpanded4$
    set:
      subject: $1ByOSVersion
  - where:
      subject: ^(DeviceManagementAndroid)$
      variant: ^Create$|^CreateExpanded$|^Get$|^GetViaIdentity$|^List$|^Delete$|^DeleteViaIdentity$|^Update$|^UpdateExpanded$|^UpdateViaIdentity$|^UpdateViaIdentityExpanded$
    set:
      subject: $1ForWorkAppConfigurationSchema
  - where:
      subject: ^(DeviceManagementAndroid)$
      variant: ^Get1$|^Delete1$|^Update1$|^UpdateExpanded1$
    set:
      subject: $1ForWorkSetting
```
### Versioning

``` yaml
module-version: 1.9.3
release-notes: See https://aka.ms/GraphPowerShell-Release.
```
