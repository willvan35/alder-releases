# Alder

A personal finance app that runs on your own computer. Alder brings in your bank
transactions, learns your categories as you label them, builds your budget from your
paystub, and shows how each month went. Nothing is stored online.

This repository is where you download Alder. It holds only the installers.

## Download

Open the **[latest release](https://github.com/willvan35/alder-releases/releases/latest)**
and, under **Assets**, download the file for your computer:

| Computer | File |
|---|---|
| Windows 10 or 11 | `Alder-Setup-x.y.z.exe` |
| Mac with Apple Silicon (M1 or newer) | `Alder-x.y.z-mac.dmg` |

Intel Macs aren't supported yet.

## Installing

Alder isn't code-signed yet, so your computer warns you the first time. That's expected.

**Windows:** run the installer. If you see "Windows protected your PC", click
**More info**, then **Run anyway**. Alder opens when it's done and stays in the Start menu.

**Mac:** open the `.dmg` and drag **Alder** into **Applications**, then open it. When
macOS says it can't check the app, click **Done**. Go to **System Settings → Privacy &
Security**, scroll down and click **Open Anyway** next to Alder. After that it opens
normally.

## Getting started

The first time it opens, Alder asks for two things:

1. **A passphrase**, if you want one. It encrypts your data on disk.
2. **Your bank data.** Connect [SimpleFIN Bridge](https://bridge.simplefin.org) ($1.50 a
   month, billed by SimpleFIN): choose **Connect an app**, copy the setup token and
   paste it into Alder. You can also import CSV files from your bank, Venmo, Tiller,
   Mint or YNAB.

To look around first, turn on **Demo mode** in the avatar menu (top right). It uses
sample data and leaves yours alone.

## Updating

When a new version is out, Alder shows a banner with a **Download** button. Install the
new version over the old one (on a Mac, drag it into Applications and choose
**Replace**). Your data carries over, and it's backed up before anything changes.

## Your data

| Computer | Folder |
|---|---|
| Windows | `%APPDATA%\Alder` |
| Mac | `~/Library/Application Support/Alder` |

Updating or uninstalling Alder never deletes this folder. To back up, or to move to a
new computer, copy it.

Alder goes online for only two things: SimpleFIN, to get your transactions, and this
page, to check for a newer version. The update check sends nothing about you.

## Something wrong?

Open an [issue](https://github.com/willvan35/alder-releases/issues) and describe what
happened. If you can, attach `logs/alder.log` from the data folder above. Read it first,
because it can include account or transaction names.
