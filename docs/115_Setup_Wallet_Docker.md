# Setup you Avatar Wallet

In order to safeguard your wallet, it is password protected. The password is stored once within the Avatar to avoid having to retype it every time the Avatar is restarted.

**IMPORTANT:** When prompted for a wallet password, pick a good password that you are
comfortable with. PLEASE REMEMBER THIS PASSWORD AS IT **CANNOT BE RECOVERED**

| Step                        | Linux/MacOS                 |
| --------------------------- | --------------------------- |
| 1. Enter configuration mode | `./run.sh enter`            |
| 2. Navigate to wallet       | `cd services/elife-stellar` |
| 3. Run the password manager | `node pw`                   |
| 4. Exit configuration mode  | `exit`                      |

## Migrating from an earlier Wallet version (Avatar node version < 3.0.0)

If you have installed an Avatar node earlier than version 3.0.0, you will need
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

## Next step

[Setup Telegram Channel](130_Setup_Telegram.md)
