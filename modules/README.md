# Gofore curling

Hagaton 2017

---

## Lähtökohta

<!-- .slide: data-state="primary-theme" -->

- Hagaton-kiima
- tiimi ei ollut työskennellyt aiemmin yhdessä
- jotain turhaa uusilla teknologioilla
- huonoja ideoita

Notes:

- tiimi syntyi oluen ääressä
- Devaajat ei ole tehneet pelejä
- Tanssimattoideoita (DDR & autopeli)
- Riston curling-idea

---

## Curling-peli

<!-- .slide: data-state="primary-theme" -->

- mikropalveluarkkitehtuuri
- Docker
- tilaton
- ohjaus komentoriviltä
- hieno käyttöliittymä

Notes:

- mikropalveluarkkitehtuuri kaikki voivat työskennellä itsenäisesti
- vain yksi oli käyttänyt dockeria aiemmin
- kaikki tekevät jotain uutta

---

## Teknologiat

<!-- .slide: data-state="primary-theme" -->

- Docker
- Python
- Node.js
- .Net Core
- Træfɪk
- Redis
- Nginx
- Vue.js
- Matter.js

Notes:

- Haluttiin yhdistää kaikkea uutta teknologiaa
- GO:takin kokeiltiin

---

## Hagathon

<!-- .slide: data-state="primary-theme" -->

- määriteltiin rajapinnat
- omat mikropalvelut
- ensimmäiset commitit ennen Tikkurilaa
- lopputulos demottiin kolmella koneella

Notes:

- Sovittiin, että ennen lähtöä ei koodata
- Koodaus intensiivistä
- Opintomatka saunan pukuhuoneeseen Gambinan kanssa

---

## Post-hagaton

<!-- .slide: data-state="primary-theme" -->

- viikossa palvelut toiminnassa
- viimeistelyyn kuukausi
- tuotantoympäristöksi AWS EC2
- tuotantoasennukset Ansiblella

Notes:

- Jo sunnuntaina jatkettiin
- AWS-tunkkaajat usein ensikertalaisia

---

## Arkkitehtuuri

<!-- .slide: data-state="primary-theme" -->

![Arkkitehtuuri](../assets/images/png/arkkitehtuuri.png)

Notes:

- arkkitehtuuri tehty hiukan perse edellä puuhun mentaliteetilla
- isomorfinen fysiikkaengine
- load balancerit yhteyksissä
- traefik api gatewayna, tarjoaa load balancerit
- enginen toiminta ja väärinkäyttö
- pienin mikropalvelu noin 16 riviä
