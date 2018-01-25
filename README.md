# swift-ssh-askpass
Basic ssh-askpass in Swift

This is a very simple project which gets you a `swift-ssh-askpass` that is compatible with `ssh-add` in OS X.

Once built and installed somewhere you can get a GUI prompt for adding your keys by running:

```shell
SSH_ASKPASS=/Path/To/swift-ssh-askpass ssh-add < /dev/null
```

I implemented this in my system by creating a small Applescript that runs at login with the following command:

```
do shell script "SSH_ASKPASS=/Path/To/swift-ssh-askpass ssh-add < /dev/null"
```
