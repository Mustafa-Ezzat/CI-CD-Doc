# Fastlane match

Alias for ```the sync_code_signing``` action

# Easily sync your certificates and profiles across your team

A new approach to iOS code signing: Share one code signing identity across your development team to simplify your codesigning setup and prevent code signing issues.

# Why match?

Before starting to use match, make sure to read [the codesigning.guide](https://codesigning.guide/)

# Create git repository

like this one: https://github.com/fastlane/certificates

# fastlane match setup
Navigate your terminal to your project's directory and run

```
fastlane match init
```

This will create a Matchfile in your current directory (or in your ./fastlane/ folder).

You can edit the content:

```
git_url("https://github.com/fastlane/certificates")
app_identifier("tools.fastlane.app")
username("user@fastlane.tools")
```
# Run fastlane match

After running fastlane match init you can run the following to generate new certificates and profiles:

```
# for production
fastlane match appstore
```

```
# for development
fastlane match development
```

This will create a new certificate and provisioning profile (if required) and store them in your selected storage.
If you previously ran match with the configured storage it will automatically install the existing profiles from your storage.

The provisioning profiles are installed in ~/Library/MobileDevice/Provisioning Profiles while the certificates and private keys are installed in your Keychain.

To get a more detailed output of what match is doing run:

```
fastlane match --verbose
```


