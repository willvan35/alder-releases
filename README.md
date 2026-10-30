# Alder

Alder is a personal finance app that runs on your own computer. It pulls in your bank
transactions, learns your categories as you label them, builds budgets from your
paystub, and tracks how each month went. Your data stays on your computer.

This page is where Alder is downloaded from. It holds only the installers.

## Download

Open the **[latest release](https://github.com/willvan35/alder-releases/releases/latest)**
and, under **Assets**, download the file for your computer:

| Computer | File |
|---|---|
| Windows 10 or 11 | `Alder-Setup-x.y.z.exe` |
| Mac with Apple Silicon (M1 or newer) | `Alder-x.y.z-mac.dmg` |

Intel Macs aren't supported yet.

## Install

Alder isn't code-signed yet, so your computer will warn you the first time. That's
expected.

**Windows**
1. Run `Alder-Setup-x.y.z.exe`.
2. If you see "Windows protected your PC", click **More info**, then **Run anyway**.
3. Click through the installer. Alder opens when it's done, and it's in the Start menu
   from then on.

**Mac**
1. Open the `.dmg` and drag **Alder** into **Applications**.
2. Open Alder. When macOS says it can't check the app, click **Done**.
3. Go to **System Settings → Privacy & Security**, scroll down, click **Open Anyway**
   next to Alder, and confirm. After that it opens normally.

## Getting started

Alder walks you through setup the first time it opens:
- **A passphrase (optional)** encrypts your data on disk.
- **Bank data** comes from [SimpleFIN Bridge](https://bridge.simplefin.org), which
  costs $1.50 a month and is billed by SimpleFIN. In SimpleFIN, choose **Connect an
  app**, copy the setup token, and paste it into Alder.

To look around first, turn on **Demo mode** in the avatar menu (top right). It shows a
year of sample data and leaves your own data alone.

## Updates

When a new version is out, Alder shows a banner with a **Download** button. Install it
the same way as the first time:
- **Windows:** run the new installer.
- **Mac:** drag the new Alder into Applications and choose **Replace**.

Your data carries over.

## Your data

Your data stays on your computer, in this folder:

| Computer | Folder |
|---|---|
| Windows | `%APPDATA%\Alder` |
| Mac | `~/Library/Application Support/Alder` |

Updating or uninstalling Alder never deletes it. To back up or move to a new computer,
copy that folder. Alder connects to the internet for only two things: SimpleFIN, to get
your transactions, and this page, to check for a newer version. The update check sends
nothing about you.

## Something wrong?

Open an [issue](https://github.com/willvan35/alder-releases/issues) and say what
happened. Attach the log if you can: `logs/alder.log` inside the data folder above.
Look through it first, since it can include account or transaction names.
