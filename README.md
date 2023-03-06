# Fuck Edge

Some sane defaults for Macroshit Edge browser. Fuck you, WebXT Edge team.

## Windows

Click `install.reg`.

## macOS

### Method 1

Use [timsutton/mcxToProfile](https://github.com/timsutton/mcxToProfile) to convert `com.microsoft.Edge.plist` to `com.microsoft.Edge.mobileconfig`. Install the profile.

```
./mcxToProfile.py --plist com.microsoft.Edge.plist --identifier MicrosoftEdgePolicy
```

### Method 2

Place `com.microsoft.Edge.plist` in `/Library/Managed Preferences/<username>/`. However, the file may disappear. I don't know why.

## Linux

Place `msedge-policies.json` in `/etc/opt/edge/policies/managed/`.
