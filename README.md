# ios-ci

Resources to enable or improve CI/CD stack for iOS apps.

### Requirements

To distribute iOS apps, you need to have sign your apps using certificate and provisioning profiles.
So, you need to have an account connected to an Apple Developer Program.

For CI/CD purpose, it's not recommended to have 2FA enabled.
Otherwise, you'll need to put the 2FA code every 30 days.

Also, it's not recommended to use an account that belogs to the account holder (for security reasons).
### Tooling

* Ruby
* Jenkins
* Gitlab
* Fastlane
* Carthage
* SonarQube

### Environment variables reference

**FASTLANE_USER**
Your App Store Connect / Apple Developer Portal user, if your fastlane setup accesses App Store Connect or the Apple Developer Portal (e.g. submit a TestFlight build, create a profile, ...)

**FASTLANE_PASSWORD**
Your App Store Connect / Apple Developer Portal password, usually only needed if you also set the

**MATCH_PASSWORD**
You need to provide the password of your match encryption if you use match

**FASTLANE_APPLE_APPLICATION_SPECIFIC_PASSWORD**
You need to provide an application specific password if you have 2-factor enabled and use pilot or deliver to upload a binary to App Store Connect

**FASTLANE_SESSION**
You need to provide a pregenerated session via fastlane spaceauth if you have 2-factor authentication enabled and want to use any actions that communicates with App Store Connect.

**LANG** and **LC_ALL**
These set up the locale your shell and all the commands you execute run at. fastlane needs these to be set to an UTF-8 locale to work correctly, for example en_US.UTF-8. Many CI systems come with a locale that is unset or set to ASCII by default, so make sure to double-check whether yours is set correctly.
