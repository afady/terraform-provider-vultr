## 1.0.6 (Unreleased)
## 1.0.5 (October 24, 2019)

- Initial release under the terraform-providers/ namespace

## [v1.0.4](https://github.com/vultr/terraform-provider-vultr/compare/v1.0.3..v1.0.4) (2019-08-09)
### Fixes
- Fixes issue where using a snapshot would cause drift [#96](https://github.com/vultr/terraform-provider-vultr/issues/96)
### Enhancements
- You will now not have to define the `os_id` for the following server options
    - `app_id`
    - `iso_id`
    - `snapshot_id`

## [v1.0.3](https://github.com/vultr/terraform-provider-vultr/compare/v1.0.2..v1.0.3) (2019-07-18)
### Fixes
- Fixes issue where you could not use `os_id` and `script_id` together [#92](https://github.com/vultr/terraform-provider-vultr/issues/92)
### Breaking Changes
- You will now need to provide the `os_id` on each corresponding option
    - `app_id` - uses os_id `186`
    - `iso_id` - uses os_id `159`
    - `snap_id` - uses os_id `164`
    - `script_id` - uses os_id `159` or any os specific id
    
## [v1.0.2](https://github.com/vultr/terraform-provider-vultr/compare/v1.0.1..v1.0.2) (2019-07-15)
### Dependencies
* Updated dependencies [PR #89](https://github.com/vultr/terraform-provider-vultr/pull/89)
  * Govultr `v0.1.3` -> `v0.1.4`
  
## [v1.0.1](https://github.com/vultr/terraform-provider-vultr/compare/v1.0.0..v1.0.1) (2019-07-08)
### Fixes
- Fixed bug where scriptID was not being 
properly handled in server creation [#82](https://github.com/vultr/terraform-provider-vultr/issues/82)
### Enhancements 
- Added error handler on protocol case sensitivity [#83](https://github.com/vultr/terraform-provider-vultr/issues/83)
### Docs
- Typo in doc firewall_rule doc for protocol [#83](https://github.com/vultr/terraform-provider-vultr/issues/83)

## v1.0.0 (2019-06-24)
### Features
* Initial release
* Supported Data Sources
    * Account
    * Api Key
    * Application
    * Backup
    * Bare Metal Plan
    * Bare Metal Server
    * Block Storage
    * DNS Domain
    * Firewall Group
    * Iso Private
    * Iso Public
    * Network
    * OS
    * Plan
    * Region
    * Reserved IP
    * Server
    * Snapshot
    * SSH Key
    * Startup Script 
    * User
* Supported Resources
    * Bare Metal Server
    * Block Storage
    * DNS Domain
    * DNS Record
    * Firewall Group
    * Firewall Rule
    * ISO
    * Network
    * Reserved IP
    * Server
    * Snapshot
    * SSH Key
    * Startup Scripts
    * User
