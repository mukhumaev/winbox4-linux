# winbox4-linux
A simple helper script to install Mikrotik's Winbox4 on GNU/Linux

## Features
1. Latest Winbox4 from [Mikrotik Download](https://mikrotik.com/download/winbox)
2. Menu entry in the application launcher
3. Supports launching from the terminal

## How to Install
Copy and paste the following command into your terminal:

```bash
curl -sSL https://raw.githubusercontent.com/mukhumaev/winbox4-linux/master/winbox4-manager | sudo bash -s -- install
```

Or, if you cloned this repository, run:

```bash
./winbox4-manager install
```

## How to Remove
To remove Winbox4, run this command:

```bash
curl -sSL https://raw.githubusercontent.com/mukhumaev/winbox4-linux/master/winbox4-manager | sudo bash -s -- remove
```

If you have already installed it, you can also use:

```bash
/opt/WinBox4/uninstall.sh
```

Or, if you cloned this repository, run:

```bash
./winbox4-manager remove
```

## Run from Terminal
After installing, you can run it from the terminal with the following command:

```bash
winbox4 [HOST] [USERNAME] [PASSWORD] [WORKSPACE]
```
> **Warning:** passwords in command-line arguments may be visible to other processes — avoid in untrusted environments.

**Example:**

```bash
winbox4 192.168.88.1 admin super-password
```

