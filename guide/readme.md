## Securing Your Codebase with GitLeaks: A Comprehensive Guide

**Introduction:**

As software developers, we all know the importance of keeping our codebase secure. One of the most critical steps in securing your codebase is to ensure that sensitive information, such as passwords and keys, is not accidentally committed to your code repository. This is where GitLeaks comes in.

**What is GitLeaks?**

GitLeaks is an open-source tool that scans your code repository for sensitive information that may have been accidentally committed. It scans your codebase for various types of sensitive information. These secrets could be passwords, API keys, tokens, private keys or suspicious file names, or file extensions like id_rsa, .pem, htpasswd. Furthermore, gitleaks can scan your whole repository’s history with all commits up to the initial one. This allows you to take immediate action to remove sensitive information and secure your codebase.

**How Does GitLeaks Work?**

GitLeaks works by scanning your code repository for files that match a set of predefined patterns. These patterns are designed to match various types of sensitive information, such as password and key files. Once GitLeaks finds a match, it alerts you, and you can take action to remove the sensitive information.

**Installing and Configuring GitLeaks**

GitLeaks is a command-line tool that can be easily installed on your development machine. It requires Python 3.6 or higher and can be installed using pip. Once you have installed GitLeaks, you will need to configure it to scan the code repository that you want to secure. This is done by creating a configuration file that specifies the location of your code repository and the patterns that GitLeaks should scan for.

**MacOS**

`brew install gitleaks`

**From Source**

git clone

`https://github.com/zricethezav/gitleaks.git`

`cd gitleaks`

`make build`

**Running a Scan**

Once you have installed and configured GitLeaks, you can run a scan by executing the following command:

`Usage:`

`gitleaks [command]`
 
Available Commands:

Command — Description

`completion` — generate the auto completion script for the specified shell

`detect` — detect secrets in code

`help`	— Help about any command

`protect` — protect secrets in code

`version` — display gitleaks version

Get all the available commands

`Gitleaks –help`
 
Detect the secrets in code base

`gitleaks detect –report-path`

`gitleaks-report.json –no-git`
