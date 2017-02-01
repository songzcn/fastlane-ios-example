# fastlane-ios-example
## Fastlane iOS Example for Beta, Release

### Simple Descriptions
* Compatibility with two differnt scheme (debug, release)
* Automatically distribute Crashlytics in Beta, Tesflight in Release using Development provisioning in beta, Distribute provisioning in release
* Automatically increment build number (e.g.4.10.19/iosbeta/4.10.19(3) -> 4.10.19/iosbeta/4.10.19(4))
* If you want to increment version number, use `increment_version_number`
* Automatically make git tag group with your build version (e.g. 4.10.19/iosbeta/4.10.19(3)) if you distribute with fastlane
* Get commit message between former version tag and HEAD

### Used Features
* `ensure_git_status_clean`
* `get_info_plist_value`
* `increment_build_number`
* `get_build_number`
* `get_version_number`
* `set_info_plist_value`
* `cert`
* `sigh`
* `pem`
* `gym`
* `commitMessage`
* `testflight`
* `crashlytics`
* `commit_version_bump`
* `add_git_tag`
* `push_to_git_remote`

### Installation
* add `.gitignore` and change your settings in Appfile, Fastfile and Deliverfile

### Trouble shooting
* If you use Firebase Push Service with different project like Debug, Release use `cert` `sigh` `development: true` for beta like this example. It will use development provisioning profile for development push.
* Git tag does not recognize "()" so I used -b (e.g. 4.10.19-b1)

### Develop with me
* Fork, Suggestions, Issues will welcome :)
