# Your Everlife.AI Avatar Node

This your main Everlife.AI Avatar node. You can use it to set up your
personal avatar and connect it to the Everlife.AI network.

![Everlife Avatar](avatar_600x600.png)

This document contains instructions for setting up and running your
**Everlife** avatar on your own machines by following the steps below. When installing for the first time we recommend that you follow all the steps carefully to install, configure, start and familiarize yourself with your Avatar.

Should you run into problems we are [here](docs/9_Feedback.md) to help you!

## 1. Installing

Depending on which Operating System you are on, please select the corresponding installation path:

### [Install on Linux](docs/100_Install_Linux.md)

### [Install on MacOS](docs/110_Install_MacOS.md)

### [Install on Windows](docs/120_Install_Windows.md)

### Upgrading

If you already have the Avatar node installed you can switch to a newer version just by extracting the new version in parallel to the old files and then [start it](docs/130_Start_Avatar.md) using the new files.

#### Upgrading from versions < 3.0.0 (Linux and MacOS only)

Due to changes in the Avatar Wallet management the wallet needs to be upgraded when upgrading an Avatar node with version less than 3.0.0. In this case follow [these instructions to upgrade it](docs/115_Setup_Wallet_Docker.md#migrating-from-an-earlier-wallet-version-avatar-node-version--300).

## [2. Setup Telegram Channel](docs/130_Setup_Telegram.md)

Configure Telegram as a communication channel for your Avatar.

## [3. Start the Avatar](docs/200_Start_Avatar.md)

Awaken the Avatar.

## [4. Start the QWERT Chat GUI](docs/210_Starting_Chat_GUI.md)

Use the QWERT Chat GUI as a communication channel for your Avatar.

## [5. Join an Avatar Hub](docs/220_Join_Hub.md)

Get connected to the Avatar network.

## [6. Add Avatar Skills](docs/230_Add_Skills.md)

Extending the Avatar by adding to its skillset.

## [7. Stopping the Avatar](docs/300_Stopping_Avatar.md)

When you need to stop the Avatar.

## [8. Feedback and Support](docs/900_Feedback.md)

Get in touch with us.

## Notes on Avatar maintenance

### Backup your Avatar data

The avatar's data always lives in the folder `elife.data` (for Linux/MacOS)
and `C:\data` (for Windows). It is recommended that you backup this
folder as it contains your `Everchain`, your `database`, and your
`Stellar` wallet.

**`elife.db`** ![db](db.png)

![Avatar](avatar_256x256.png)


