Jens Marten Liivak: Udacity Networking for web developers
```  
Lesson 1: "From Ping to HTTP"  

"Ping" Käsk saadab valitud IP aadressile test sõnumid/paketid, kui need ka tagasi tulevad
siis on sinu ja valitud hosti vahel neti ühendus olemas ning neil on töötav arvuti koos ühendusega.
Juhul kui need ei tule tagasi ja timeouti lähevad siis kas a. Sul pole töötavat interneti ühendust,
b. Valitud hostil pole ühendust või seal aadressil pole arvutit.  
"printf" Käsk võimaldab sõnade sisestamise ja selle abil erinevate asjade kätte saamise või saatmise.   
"nc-l" Avab ühepoolse kuulamis ühenduse.  
"nc" Võimaldab teiste hostidega suhtlemise ja kasutatakse tihti informatsiooni taotlustel.

Erinevad port numbrid, mis voivad vajalikud olla:
22:SSH
80:HTTP
443:HTTPS  
  
```  
```  
Lesson 2: "Dig into DNS Records"

"CTRL + C" Hotkey peatab käiva protsessi, nt ping protsessi loop.
"host" Näitab antud hosti nime taga olevaid IP aadresse ja muud informatsiooni. 
"dig" Töötab peaaegu samamoodi kui host käsk aga näitab ka detailsemat infot (Nt mis server sinu taotlusele vastas)  

Seletati ka IPv4 ja IPv6 erinevust.
IPv4 Väiksema bit suurusega ja vanem.
IPv6 Suurema bit suurusega ja uuem.  
  
```  
```  
Lesson 3: "Addressing and Networks"

Olemas on ka reserveeritud IP aadressid. 
Need on tavaliselt seatud erinevatele avalikele teenustele ja valitsustele.

Püstitatud on ka probleem, milleks on see, et maailmas pole piisavalt IP aadresse olemas.
See on lahendatud süsteemiga (NAT) mis võtab kokku kõik ühe ruuteri ühendused, vähendades kasutust.

```  
```  
Lesson 4: "HTTP on TCP on IP"

"tcpdump" 
Samuti rääkis packetite vajalikkusest ning lähemalt, et kuidas need töötavad.
Pärast x aja möödumist katkeb ühendus juhul, kui üks pool teiselt vastust ei saa.
```  
```  
Lesson 5*

traceroute --> Näitab ette kõik enne läbitud IP-aadressid, milleni jõuti enne soovitud aadressile jõudmist.
Ruuterid ei ole suutelised (või võimelised?) suurtes kogustes packeteid korraga läbi laskma ning räägiti selle lahendusest.
Samuti oli jutt, et seadmetel on firewall, mis filtreerib seadme ja võrgu vahel toimuvat tegevust - vältides süsteemitõrkeid ning pahavara.
```  
```  
# Mida ma huvitavat teada sain:

- Kuidas timeout tekib.

- Juhul kui inimesed on NAT-iga eraldatud, saab neil olla sama IP-aadress.

- Lõpmatute loopide vältimiseks on packetitel limiteeritud eluaeg.

- Et eksisteerivad reserveeritud port-id (port-id 0-1023)
```
