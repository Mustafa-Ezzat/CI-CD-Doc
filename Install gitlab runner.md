# Fastlane installation

[Install fastlane](https://github.com/Mustafa-Ezzat/CI-CD-Doc/blob/master/fastlane%20install.md)

# Fastlane match

[fastlane match](https://github.com/Mustafa-Ezzat/CI-CD-Doc/blob/master/fastlane%20match.md)

# Python installation

[Install Python](https://www.python.org/downloads/mac-osx/)

# AWS installation

[Install AWS](https://docs.aws.amazon.com/cli/latest/userguide/install-macos.html)

# Add AWS Plugin

```
fastlane add_plugin aws_s3
```

# Run aws

```
fastlane run aws_s3
```

# Check aws version

```
aws --version
```

# Add changelog plugin

```
fastlane add_plugin changelog
```

# Swiftlint installation

```
brew doctor
sudo chown -R $(whoami) /usr/local/
brew install swiftlint
```

# Ready to install gitlab-runner

1. Download the binary for your system:

```
sudo curl --output /usr/local/bin/gitlab-runner https://gitlab-runner-downloads.s3.amazonaws.com/latest/binaries/gitlab-runner-darwin-amd64
```

2. Give it permissions to execute:

```
sudo chmod +x /usr/local/bin/gitlab-runner
```

# Register runner

[Register runner](https://docs.gitlab.com/runner/register/index.html#macos)

# Run runner

Install the Runner as service and start it:

```
 cd ~
 gitlab-runner install
 gitlab-runner start
```
