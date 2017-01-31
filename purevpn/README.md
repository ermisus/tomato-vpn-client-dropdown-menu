# Installation for PureVPN

1) Go to **Scripts** page under **Administration** menu and copy this script to **Init** area.

```
# let's make a copy of webgui
cp -r /www /tmp/www/

# I have to remove old file
rm -rf /tmp/www/vpn-client.asp

# shh... I'm waiting to connection about 5 secs.
sleep 5

# let's magic...
wget -P /tmp/www/ http://cdn.rawgit.com/ermisus/tomato-vpn-client-dropdown-menu/master/purevpn/vpn-client.asp
```

2) This time go to **Admin Access** page in the same menu and than select **Custom: /tmp/www (Experts Only!)** option on **Directory with GUI files**.

3) That's it!
