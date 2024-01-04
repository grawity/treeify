LDAP
----

    $ ldapsearch -QLLL '(objectClass=*)' dn | ldifls -s $'\t' | treeify -s $'\t' -R

    o=Nullroute
     ├─cn=Kerberos
     ├─l=Alias object
     ├─l=Real object
     ├─ou=Application users
     │  ├─ou=Ampache+uid=grawity
     │  ├─ou=Cacti+uid=grawity
     │  ├─ou=Syncthing+uid=grawity
     │  └─ou=Transmission+uid=grawity
     ├─ou=Configuration
     │  ├─cn=Dovecot anonymous user
     │  ├─ou=Filesystems
     │  │  ├─nisMapName=auto.master
     │  │  │  └─cn=/net
     │  │  └─nisMapName=auto.net
     │  │     ├─cn=*
     │  │     ├─cn=ember
     │  │     ├─cn=land
     │  │     ├─cn=sky
     │  │     ├─cn=star
     │  │     ├─cn=wind
     │  │     └─cn=wolke
     │  ├─ou=NIS services map
     │  │  ├─cn=athinfo+ipServicePort=49155
     │  │  ├─cn=cso+ipServicePort=105
     │  │  ├─cn=eklogin+ipServicePort=2105
     │  │  ├─cn=gale+ipServicePort=11512
     │  │  ├─cn=gemini+ipServicePort=1965
     │  │  ├─cn=ircs+ipServicePort=994
     │  │  ├─cn=kf+ipServicePort=21490
     │  │  ├─cn=kpop+ipServicePort=1109
     │  │  ├─cn=routeros-api+ipServicePort=8728
     │  │  ├─cn=routeros-api-tls+ipServicePort=8729
     │  │  ├─cn=smtps+ipServicePort=465
     │  │  ├─cn=spotify-disc+ipServicePort=57621
     │  │  ├─cn=submissions+ipServicePort=465
     │  │  ├─cn=syncthing-disc+ipServicePort=21027
     │  │  ├─cn=syncthing+ipServicePort=22000
     │  │  ├─cn=systemd-journald+ipServicePort=19531
     │  │  ├─cn=venti+ipServicePort=17034
     │  │  ├─cn=winbox+ipServicePort=8291
     │  │  ├─cn=wireguard+ipServicePort=708
     │  │  ├─cn=x25+ipServicePort=1998
     │  │  └─ou=Unofficial
     │  └─uid=test
     ├─ou=Devices
     │  ├─cn=vol3
     │  ├─cn=vol4
     │  ├─cn=vol5
     │  └─ou=Home
     ├─ou=Hosts
     │  ├─cn=blizzard
     │  │  ├─cn=blizzard.data
     │  │  └─cn=blizzard.games
     │  ├─cn=dune.nullroute.lt
     │  ├─cn=ember.nullroute.lt
     │  ├─cn=frost
     │  ├─cn=fujitsu
     │  ├─cn=land.nullroute.lt
     │  ├─cn=midnight
     │  ├─cn=myth.nullroute.lt
     │  ├─cn=sky.nullroute.lt
     │  ├─cn=star.nullroute.lt
     │  ├─cn=vm-ampere.nullroute.lt
     │  ├─cn=vm-litnet.nullroute.lt
     │  ├─cn=vm-okeanos.nullroute.lt
     │  ├─cn=wind.nullroute.lt
     │  │  └─cn=iLO4
     │  ├─cn=wolke.nullroute.lt
     │  ├─ou=Containers
     │  │  ├─cn=lanman
     │  │  └─cn=vm-vol5.nullroute.lt
     │  ├─ou=Foreign
     │  │  ├─cn=baltix-henet-vno1-gw
     │  │  ├─cn=finmin-vbams
     │  │  ├─cn=freetransit-ch-win
     │  │  ├─cn=freetransit-ch-win-oob
     │  │  ├─cn=freetransit-nl-ams
     │  │  ├─cn=gw-core.utenos-kolegija.lt
     │  │  ├─cn=henet-dus
     │  │  ├─cn=henet-lon
     │  │  ├─cn=kaunas-hp-kttc
     │  │  ├─cn=ktu-baltix-gw
     │  │  ├─cn=ktu-itd-gw
     │  │  ├─cn=ku-gw
     │  │  ├─cn=ntp.cgates.lt
     │  │  ├─cn=panko-gw
     │  │  ├─cn=su-gw
     │  │  ├─cn=vu-as-gw
     │  │  └─cn=vu-mii-gw
     │  └─ou=Personal computers
     │     ├─cn=pixel3a
     │     ├─cn=rain
     │     └─cn=raindows
     ├─ou=Netgroups
     │  ├─cn=arch-ops
     │  └─cn=nfs-servers
     ├─ou=NIS groups
     │  ├─cn=netadmins
     │  ├─cn=netguests
     │  ├─cn=netusers
     │  └─cn=users
     ├─ou=People
     │  └─uid=grawity
     ├─ou=Processes
     │  ├─cn=Apache httpd
     │  ├─cn=Dovecot mail server
     │  ├─cn=FreeRADIUS
     │  ├─cn=Kerberos KDC
     │  ├─cn=Nextcloud
     │  ├─cn=Postfix SMTP server
     │  ├─cn=Roundcube webmail
     │  ├─cn=RWho
     │  │  ├─cn=RWho Client API
     │  │  └─cn=RWho Host API
     │  └─cn=SimpleSAMLphp
     └─ou=Security
        ├─cn=DSA admins
        └─cn=Replica servers

vim: ts=4:sw=4:et
