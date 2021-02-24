fastlane documentation
================
# Installation

Make sure you have the latest version of the Xcode command line tools installed:

```
xcode-select --install
```

Install _fastlane_ using
```
[sudo] gem install fastlane -NV
```
or alternatively using `brew install fastlane`

# Available Actions
### xcode
```
fastlane xcode
```
Download and install a specific Xcode version
### reset
```
fastlane reset
```
Reset environment
### get_version
```
fastlane get_version
```
Get current version of the project
### dependencies
```
fastlane dependencies
```
Install project dependencies
### tests
```
fastlane tests
```
Runs all the tests
### build
```
fastlane build
```
Build app

----

This README.md is auto-generated and will be re-generated every time [fastlane](https://fastlane.tools) is run.
More information about fastlane can be found on [fastlane.tools](https://fastlane.tools).
The documentation of fastlane can be found on [docs.fastlane.tools](https://docs.fastlane.tools).
