# Fastlane

The easiest way to automate beta deployments and releases for your iOS.

# Install the latest Xcode command line tools:

```
xcode-select --install
```

# Install fastlane:

```
# Using RubyGems
sudo gem install fastlane -NV

# Permission issue
gem install fastlane -NV --user-install

# Alternatively using Homebrew
brew cask install fastlane

```

# fastlane setup

Navigate your terminal to your project's directory and run

```
fastlane init
```

# Running iOS tests using fastlane

To run your unit tests or UI tests using fastlane, add the following to your Fastfile

```
lane :tests do
  run_tests(workspace: "Example.xcworkspace",
            devices: ["iPhone 6s", "iPad Air"],
            scheme: "MyAppTests")
end
```

To use the newly created lane, just run

```
fastlane tests
```

