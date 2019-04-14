# Your Everlife.AI Avatar Node

[This](https://github.com/everlifeai/everlife-node-releases/releases) is your main Everlife.AI Avatar node. You can use it to set up your
personal avatar and connect it to the Everlife.AI network.

![Everlife Avatar](avatar_600x600.png)

This document contains instructions for setting up and running your
**Everlife** avatar on your own machines by following the steps below. When installing for the first time we recommend that you follow all the steps carefully to install, configure, start and familiarize yourself with your Avatar.

Should you run into problems we are [here](docs/9_Feedback.md) to help you!

[Download the latest release here](https://github.com/everlifeai/everlife-node-releases/releases)

## Existing Avatar Node Upgrade

If you already have an Avatar node installed, make sure you stop it. You can switch to a newer version just by extracting the new version in parallel to the old files and then [start it](docs/130_Start_Avatar.md) using the new files.


## 1. New Avatar Node Install

Depending on which Operating System you are on, please select the corresponding installation path:

### [Install on Linux](docs/100_Install_Linux.md)

### [Install on MacOS](docs/110_Install_MacOS.md)

### [Install on Windows](docs/120_Install_Windows.md)



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

## [7. Feedback and Support](docs/900_Feedback.md)

Get in touch with us.

## Personalizing your Avatar

Your avatar has the ability to talk to you and learn about you. Some of
this information - like your skills and work history - it will use to chat
with other avatars and network. Other information - like your life story -
it will keep as an encrypted record for the future.

You have the ability to extend the avatar's ability to gather
information so it will store information that you feel is important to
you. For now, the avatar comes with three sets of information storage
that you can try out and experiment with:

    you> Ask about me
    avatar> (Gathers information about you)

    you> Ask about school
    avatar> (Gathers information about your school life)

    you> Ask about love
    avatar> (Gathers information about your love life)

For now the avatar stores this information in a text file `kb.txt` ever
few minutes. Shortly, however, this information will be stored encrypted
on the Everchain and hence be available to talk with other avatars and
immune from destruction.


## Notes on Avatar maintenance

### Backup your Avatar data

To find your avatar's data storage run the start script with `--info`
skip. For example:

        $> ./run-mac.sh --info

And it will give you the location of your data.  It is recommended that
you backup this folder as it contains your `Everchain`, your `database`,
and your `Stellar` wallet.

**`elife.db`** ![db](db.png)

![Avatar](avatar_256x256.png)


