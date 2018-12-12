# Your Everlife.AI Avatar Node

This your main Everlife.AI Avatar node. You can use it to set up your
personal avatar and connect it to the Everlife.AI network.

The Avatar Node comes in two flavors:
1. A [Docker](https://www.docker.com/) version that can be deployed on
   any VPS or Mac or Linux machine
2. A non-docker Windows version (Docker is hard to install on Windows)


![Everlife Avatar](avatar_600x600.png)


# Bringing your Avatar to life

This document contains instructions for setting up and running your
**Everlife** avatar on your own machines.

## Pre-requisites

### Docker (Mac/Linux/VPS) Pre-requisities

1. Install [Docker](http://www.docker.com/)
2. Install [Yarn](https://yarnpkg.com/)

### Windows Pre-requisities

**Windows 10**
1. Install [NodeJS](https://nodejs.org/)
   (install all the options including Python and the dotnet framework
    required by [node-gyp](https://github.com/nodejs/node-gyp)
2. Install [Yarn](https://yarnpkg.com/)

**Windows 7**
Ensure all the following are installed:
1. Windows 7 _**(Service Pack One)**_
2. Dotnet framework 4.5.2
3. VC++ 2017
4. Python 2.7
5. NodeJS 10+
6. Yarn (latest)


## Windows Setup

In order to get a working avatar with a wallet, you need to set it up
and configure it.

1. Download the correct version of Avatar Node for your environment
[Windows 64 bit Version of Avatar Node](https://github.com/everlifeai/everlife-node-releases/releases/download/v0.4.0/elife_0.4.0-windows-x64.zip) or
[Windows 32 bit Version of Avatar Node](https://github.com/everlifeai/everlife-node-releases/releases/download/v0.4.0/elife_0.4.0-windows-x32.zip)

2. Unzip the avatar into your `$HOME` directory
3. Go to the command prompt and navigate to your node directory
4. `run setup`

In order to safeguard the wallet, it is password protected. So that the
user does not need to type in this password again and again it needs to
be saved once. In order to do this the setup will ask you for a
password.

When prompted for the password, pick a good password that you are
comfortable with. PLEASE REMEMBER THIS PASSWORD AS IT **CANNOT BE
RECOVERED**.

## Docker Setup

In order to get a working avatar with a wallet, you need to set it up
and configure it. First you need to set up the required docker
containers. Perform the following steps:
1. Download the [Docker Version of Avatar Node](https://github.com/everlifeai/everlife-node-releases/releases/download/v0.4.0/elife_0.4.0-docker.tar.gz)
2. Unzip the avatar into your `$HOME` directory
3. Go to the command prompt and navigate to your node directory
4. `./run.sh setup`

In order to safeguard the wallet, it is password protected. So that the
user does not need to type in this password again and again it needs to
be saved once. In order to do this you need to do the following:

1. Load the node

        $> ./run.sh enter

2. Go to the Stellar Server

        # cd services/elife-stellar

3. Run the password manager

        # node pw

When prompted for the password, pick a good password that you are
comfortable with. PLEASE REMEMBER THIS PASSWORD AS IT **CANNOT BE
RECOVERED**.


## QWERT - The default GUI

In order to start chatting with your avatar, you can use the built-in
chatbot. To start this use:

        Windows:
            C:\Users\John\elife> run gui
        Docker:
            $> ./run.sh gui

This will launch a GUI which you can use to chat with your avatar.


## Telegram Channel

To chat with your bot 'on the go' (on your mobile phone for example) you
can use the excellent [Telegram](the://telegram.org) application. The
avatar has a communication channel that integrates with Telegram. The
steps for doing this are as follows:

1. Go to [Telegram](https://telegram.me/botfather) to create a bot by
   typing

            /newbot

    command to create your telegram bot.

1. The BotFather will ask you for a name and username, then generate an
   authorization token for your new bot. The token is a string along the
   lines of 110201543:AAHdqTcvCH1vGWJxfSeofSAs0K5PALDsaw. 
1. We now need to link this new telegram bot with your avatar. To do
   this, simply save the telegram token in
   `elife.data/cfg.env` (in Windows this is simply `cfg.env` in your
    local directory)



### Migrating old nodes (from version < 3.0.0)
If you have installed a node earlier than version 3.0.0, you will need
to migrate your stellar wallet to be compatible with the latest version.

Steps to do this:

1. Make a backup of your existing password file. You will find this
   hidden file in your `elife.data` folder with the name `.luminate-pw`:

        mv elife.data/.luminate-pw <some backup location>

2. Regenerate your Stellar Wallet password by using the same steps
   above. *You must use the same password you have used when setting up
   the node*.

        #> ./run.sh enter
        # cd services/elife-stellar
        # node pw

3. Download
   [lu-migrate](https://github.com/theproductiveprogrammer/lu-migrate)
4. Point it to your stellar account. You will find your account in the
   `elife.data/stellar/` directory. The filename will end with
   `.stellar`

        yarn start --to v2 /path/to/elife.data/stellar/wallet-...

5. Start your node and you're ready to go


## Your Data

The avatar's data always lives in the folder `elife.data` (for Docker)
and `C:\data` (for Windows). It is recommended that you backup this
folder as it contains your `Everchain`, your `database`, and your
`Stellar` wallet.

**`elife.db`** ![db](db.png)



## Starting and Chatting with Your Avatar

Now that your avatar is set up you can start him up by running

        C:\Users\John\elife> run avatar (Windows)

        $> ./run.sh avatar (Docker)


Now you can go to your interface of choice (Telegram or QWERT) and start
chatting!


## Stopping your avatar

### Windows Version
Simply type `Ctrl+C` in the terminal window to stop your avatar from
running.

### Docker Version
Your avatar will keep running in the background and is expected to run
even after you restart your machine. To stop the avatar please run:

        $> ./run.sh stop


## Next steps
1. Join the Everlife network through an **Avatar Hub**.Contact our
   support channel in discord to get your invite code to join the hub
   and inform your avatar that you would like to join this Avatar Hub by
   saying

        /use_invite xxxx

2. Install and try out various skills

        /help
        /install calculator
        /install what-wine


Feel free to provide us your feedback and issues in our [discord support
channel](https://discord.gg/TDyRSr4).

![Avatar](avatar_256x256.png)


