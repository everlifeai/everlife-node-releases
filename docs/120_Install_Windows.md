# Installing the Avatar on Windows

Compared to the Linux and MacOS versions of the Avatar node, the Windows version is not Docker based, this is due to the complexity of running Docker on Windows.

## Pre-requisites

### Windows 10

1. Install [NodeJS](https://nodejs.org/) - LTS Version 10, make sure to install all the options including Python and the .NET Framework which required by [node-gyp](https://github.com/nodejs/node-gyp)
2. Install [Yarn](https://yarnpkg.com/)

### Windows 7

1. Windows 7 _**(Service Pack One)**_
2. .NET Framework 4.5.2
3. Visual C++ 2017
4. [Python 2.7](https://www.python.org/downloads/)
5. Install [NodeJS](https://nodejs.org/) - LTS Version
6. Install [Yarn](https://yarnpkg.com/)

## Download

Your windows version might be of a 64-bit or a 32-bit type. See this [Microsoft support article](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you do not know which type you have.

Download the latest **Windows** package, 64-bit or 32-bit, from the [Releases page](https://github.com/everlifeai/everlife-node-releases/releases).

## Install

**First: If you are upgrading first [stop the existing Avatar](300_Stopping_Avatar.md) if it is running.**

1. Unzip the downloaded package in your HOME directory.

## Setup you Avatar Wallet

In order to safeguard your wallet, it is password protected. The password is stored once within the Avatar to avoid having to retype it every time the Avatar is restarted.

1. Open the `Command Prompt` application (command line shell, `cmd.exe`).
2. At the prompt, navigate to the directory what was created by unzipping the files above.
3. At the prompt enter the command `run setup`.

**IMPORTANT:** When prompted for a wallet password, pick a good password that you are
comfortable with. PLEASE REMEMBER THIS PASSWORD AS IT **CANNOT BE RECOVERED**

## Next step

[Setup Telegram Channel](130_Setup_Telegram.md)
