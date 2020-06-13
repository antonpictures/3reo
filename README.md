# 3reo
Put 3reo TV on your device. 3reotertain the planet, the best content creators in the world  across all viewing devices out there.

- 1. HOME PAGE 3reo.com to look like this: https://i.imgur.com/q8cQy7g.jpg
- Shorten the Width of Column title #Connected rename it to #C.
- To the right of NOW PLAYNG column, add column (AC) containing the text of next item in the channel's playlist.
- Order the Channel List by the channel# ascending.
- Add Channel Logo Column to the left of #Channel column.
- When scrolling the channels the screen (youtube embed) stays with the viewer. Either add a big SCROLL BAR, as pictured, to the left of the channel list TV grid or simply the TV embed plays picture-in-picture, floating video.
- Above "Now Playing" Column title add the CURRENT TIME (CT) and to it's left current time minus 30 and to the right above the new AC column current time plus 30 minutes as pictured.
- top left corner change the name of the website SYNC with 3REO. 
- Change the title "Public Channels" with "Free Live Cable TV Channels & Movies"
- One global chat like toonreboot
- add working hotkeys UP-DOWN (volume) LEFT-RIGHT (change channel) so people can work the website from the remote in the couch.
-->
- 2. ADMIN PAGE /account/channels to look like this: https://i.imgur.com/hbQFtn7.jpg
- Add "Edit Playlist" button/s for every channel to be able to modify the selected playlist.
--/
- iOS, Android, all TV OS Apps --> app list to be coded: https://i.imgur.com/88jdpHe.png

-->
- Marketing TRAILERS: on 3reo your family and friends can find a channel, a movie and a show for everyone. 
-->
- SOLVED Provide YouTube V3 AP key.
- SOLVED Base instal w/out mods: EC2 vps provisioned and running. Creating EC2 instance with Ubuntu Server 18.04 LTS (HVM), SSD Volume Type. Public IP is 13.56.18.151 - personal ssh keys set
system updated
pulling in required system packages now. nginx, mariadb-server, nodejs, npm
- SOLVED 3reo.com "not secure" in browser bar. Godaddy: I can provide SSL however as hosting is not on domain the Url will need to be setup with SSL by hosting provider also. Buy SSL for website secured connection $79.99/year @godaddy = cloudflare
--/
- static: the c y t u b e installation lives in /opt
- $ modifying the index to embed and track the playlist of a loaded channel is complex, and will take several hours.
- $ when index feature is complete, Then we can move on to playlist editor in ACP.
- end game: Human Channel Moderators using AI bots to select video content from all publicly available sources within the colective interest, filter, categorize, edit and distribute it through the channels of interest. Story by George Anton coded by xaekai based on CyTube.

 - other like UI examples:
      Pluto.tv  https://i.imgur.com/BBbNweM.png
      Xfinity grid https://i.imgur.com/mvdTYpI.jpg
      Comcast https://i.imgur.com/qOkiu4e.jpg
- Logos:
 3reo Orange https://i.imgur.com/KToebw4.jpg
 3reo Glass Door https://imgur.com/gallery/FcrxWu1 
 --/
 --/
# curl -I  http://antube
HTTP/1.1 200 OK
Server: nginx/1.14.0 (Ubuntu)
Date: Thu, 09 Apr 2020 23:42:10 GMT
Content-Type: text/html
Content-Length: 612
Last-Modified: Thu, 09 Apr 2020 22:34:03 GMT
Connection: keep-alive
ETag: "5e8fa2db-264"
Accept-Ranges: bytes
--/
╰┴─$─┶► dig 3reo.com

; <<>> DiG 9.16.1 <<>> 3reo.com
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 11505
;; flags: qr rd ra; QUERY: 1, ANSWER: 2, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 512
;; QUESTION SECTION:
;3reo.com.        IN A

;; ANSWER SECTION:
3reo.com.       299  IN A       104.24.117.247
3reo.com.       299  IN A       104.24.116.247

;; Query time: 66 msec
;; SERVER: 192.168.1.1#53(192.168.1.1)
;; WHEN: Fri Apr 10 16:49:57 PDT 2020
;; MSG SIZE  rcvd: 69
--/
[root@luna xaekai]# dig 3reo.com

; <<>> DiG 9.9.4-RedHat-9.9.4-51.vl7.2 <<>> 3reo.com
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 27388
;; flags: qr rd ra; QUERY: 1, ANSWER: 2, AUTHORITY: 2, ADDITIONAL: 5

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 4096
;; QUESTION SECTION:
;3reo.com.                      IN      A

;; ANSWER SECTION:
3reo.com.               287     IN      A       104.24.117.247
3reo.com.               287     IN      A       104.24.116.247

;; AUTHORITY SECTION:
3reo.com.               172787  IN      NS      hadlee.ns.cloudflare.com.
3reo.com.               172787  IN      NS      louis.ns.cloudflare.com.

;; ADDITIONAL SECTION:
hadlee.ns.cloudflare.com. 172787 IN     A       162.159.38.67
hadlee.ns.cloudflare.com. 172787 IN     AAAA    2606:4700:50::a29f:2643
louis.ns.cloudflare.com. 172787 IN      A       162.159.44.89
louis.ns.cloudflare.com. 172787 IN      AAAA    2606:4700:58::a29f:2c59

;; Query time: 2 msec
;; SERVER: 207.115.64.2#53(207.115.64.2)
;; WHEN: Fri Apr 10 16:54:05 PDT 2020
;; MSG SIZE  rcvd: 212

--/
curl -I 3reo.com
HTTP/1.1 200 OK
Date: Fri, 10 Apr 2020 23:57:06 GMT
Content-Type: text/html; charset=utf-8
Connection: keep-alive
Set-Cookie: __cfduid=dbe21ff69b831bf65a19b80248abf6dbc1586563025; expires=Sun, 10-May-20 23:57:05 GMT; path=/; domain=.3reo.com; HttpOnly; SameSite=Lax
X-Powered-By: Express
Set-Cookie: _csrf=s%3ATKkC3zNnRjRbnZHmQ-n6ot_R.JfwF6%2Fs%2BAHYyBi%2FBj0r4qqgRb1DO75%2BNo29XYuNIbPY; Domain=localhost; Path=/; HttpOnly
Vary: Accept-Encoding
CF-Cache-Status: DYNAMIC
Server: cloudflare
CF-RAY: 582068807c68fdb5-PDX
--/
User HTTPS --->     <-- HTTPS:: Cloud flare :: HTTP -->     <--  HTTP::Your server
--/
 solved - web ssl chain fixed in no time, but the websocket is being a problem.
--/
Node.JS Server and JavaScript/HTML Client for synchronizing online media

