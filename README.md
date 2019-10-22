Jens Marten Liivak: Udacity Networking for web developers
```  
Lesson 1: "From Ping to HTTP"  

"Ping" Käsk saadab valitud IP aadressile test sõnumid/paketid, kui need ka tagasi tulevad
siis on sinu ja valitud hosti vahel neti ühendus olemas ning neil on töötav arvuti koos ühendusega.
Juhul kui need ei tule tagasi ja timeouti lähevad siis kas a. Sul pole töötavat interneti ühendust,
b. Valitud hostil pole ühendust või seal aadressil pole arvutit.  
"printf" Käsk võimaldab sõnade sisestamise ja selle abil erinevate asjade kätte saamise või saatmise.   
"nc-l" Avab ühepoolse kuulamis ühenduse.  
"nc" Võimaldab teiste hostidega suhtlemise. Kasutatakse tihti informatsiooni taotlustel ning andmete vahetamisel.

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
Mis võimaldab ühe IP aadressi all, luua terve privaatvõrgu.

```  
```  
Lesson 4: "HTTP on TCP on IP"

"tcpdump" Annab võimaluse detailsemalt jälgida kõike sisse ja välja minevat võrgu liiklust.
Käsklusele peab tavaliselt lisama ka filtri/täpsustuse, et näha endale vajalikku informatsiooni.

Andmete saatmisel võib esineda ka "Timeout". Timeout on saatmise protsessi katkestus koos erroriga.
Timeout tekkib siis kui kumbki pool liiga kaua võrgus ei vasta. Põhjuseid võib selleks olla mitu.
Näiteks a. Teist valitud hosti pole olemas b. Katkestus võrgus kummalgil poolel või interneti teenuse pakkuja poolne viga

```  
```  
Lesson 5: "Big Networks

Ühendades ennast teise hostiga läbi võrgu (nt veebilehega), peab sinu internetiliiklus
liikuma läbi mitme erineva IP aadressi (ruuteri), et jõuda sihtkohta. Mida rohkem peatusi
kust on vaja läbi minna, seda aeglasem on ühendus.
"traceroute" Käsklus annab sulle nimekirja igast peatusest, mis enne sihtkohta läbiti.

"Ping" kui definitsioon on, sinu signaalil kulutatud aeg, et liikuda sihtkohta ja tagasi.
Mida suurem pingi kulutatud aeg, seda aeglasem on ühendus. Suur peatuste arv suurendab pingi.

```  
```  

