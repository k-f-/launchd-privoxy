
don't need this anymore now that homebrew's privoxy ships
with a launchctl
---------------------------------------------------------
# Privoxy Launchctl

## Why?

I use homebrew.  It doesn't create this when you install Privoxy.

## How?

Copy the contents of the .plist file to

```
sudo vim /Library/LaunchDaemons/org.privoxy.plist
```

then:

```
sudo chown root:wheel org.privoxy.plist
launchctl load /Library/LaunchDaemons/org.privoxy.plist
launchctl start org.privoxy.launchd.privoxy
```
