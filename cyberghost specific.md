To work with cyberGhost, you need to connect to get from cyberghost the list of file needed to connect (client.cert client.key default.ovpn et ca.crt ).
To get that crteate a manual instalaltion (Routeurs or other devices on the website from cyberghost).

Download those files within The repository referenced by "${CUSTOM_VOLUME}". 

Then cyberghost .ovpn files must be manually updated to work. 

Add the same path to cert and key than for ca. It should come from :
```
ca /etc/openvpn/custom/ca.crt
cert client.crt
key client.key
```

To : 
```
ca /etc/openvpn/custom/ca.crt
cert /etc/openvpn/custom/client.crt
key /etc/openvpn/custom/client.key
```

## Tools to ensure it is working 

Utiliser ipleak.net pour les torrents
Ce site offre un test spécifique pour vérifier l'IP utilisée lors des téléchargements torrent :

Go to ipleak.net

Find  section "Torrent Address detection"

click on "Activate" then "this Magnet Link"

Add torrent magnet to transmission 

Look on  ipleak.net : your ip should be displayed 

Other websyites : 
- checkmyip.torrentprivacy.com 
- whatismyip.com : Only manual 

