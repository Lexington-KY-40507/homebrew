# homebrew

## Overview

This script installs Homebrew on a Linux system. Homebrew is a popular package manager that simplifies the installation and management of software on Unix-like operating systems. This customized version of the Homebrew installation script is configured to install everything under the `/home/versbottomlex/.dev/lib/brew` directory. 

> **Note:** This script is intended for personal use and is currently in the testing phase.

## Script Details

The script performs the following tasks:

1. **System Compatibility Check**: Ensures that the script is being run on a supported operating system (macOS or Linux) and checks for necessary permissions and configurations.

2. **Non-Interactive Mode Detection**: Configures the script to run non-interactively if required, which is useful for CI/CD environments.

3. **User and Group Setup**: Determines the current user and group to set appropriate permissions for the installation directories.

4. **Directory Creation and Permissions**: Creates necessary directories under `/home/versbottomlex/.dev/lib/brew` and sets the appropriate permissions. These directories include:
    - `/home/versbottomlex/.dev/lib/brew/bin`
    - `/home/versbottomlex/.dev/lib/brew/etc`
    - `/home/versbottomlex/.dev/lib/brew/include`
    - `/home/versbottomlex/.dev/lib/brew/lib`
    - `/home/versbottomlex/.dev/lib/brew/sbin`
    - `/home/versbottomlex/.dev/lib/brew/share`
    - `/home/versbottomlex/.dev/lib/brew/var`
    - `/home/versbottomlex/.dev/lib/brew/opt`
    - `/home/versbottomlex/.dev/lib/brew/share/zsh`
    - `/home/versbottomlex/.dev/lib/brew/share/zsh/site-functions`
    - `/home/versbottomlex/.dev/lib/brew/var/homebrew`
    - `/home/versbottomlex/.dev/lib/brew/var/homebrew/linked`
    - `/home/versbottomlex/.dev/lib/brew/Cellar`
    - `/home/versbottomlex/.dev/lib/brew/Caskroom`
    - `/home/versbottomlex/.dev/lib/brew/Frameworks`

5. **Sudo Access**: Checks for sudo access to perform actions that require elevated privileges.

6. **Command Line Tools Installation**: Installs necessary command line tools if they are not already present.

7. **Git and Curl Verification**: Ensures that the required versions of Git and cURL are installed.

8. **Homebrew Repository Setup**: Clones the Homebrew repository into the designated directory and sets up the Homebrew environment.

9. **Post-Installation Configuration**: Provides instructions for adding Homebrew to your system’s PATH and other environment variables.

## Usage

To use this script, simply execute it in your terminal:

```sh
/bin/bash /path/to/your/script.sh
```

Make sure to replace `/path/to/your/script.sh` with the actual path to the script file.

## Important Notes

- **Personal Use Only**: This script is for personal use and is currently being tested. It may not work as expected in all environments.
- **Permissions**: Ensure you have the necessary permissions to create directories and install software on your system.

## Disclaimer

This script is provided "as is" without any warranty. Use it at your own risk. The author is not responsible for any damage or data loss resulting from its use.