# Privoxy Launchctl

## Why?

I use homebrew.  It doesn't create this when you install Privoxy.

## Useage

Copy the .plist file to

```
/Library/LaunchAgents
or
~/Library/LaunchAgents
```

Then, you can bring it up to see if it works with:

```
launchctl load ~/Library/LaunchAgents/com.kfring.privoxy.plist
```

Upon reboot it *should* start.
