# Gofore curling

Hagaton 2017

---

## Lähtökohta

<!-- .slide: data-state="primary-theme" -->

- huonoja ideoita

Notes:

- tiimi syntyi oluen ääressä
- tiimi ei ollut työskennellyt aiemmin yhdessä
- Riston curling-idea

---

## Curling-peli

<!-- .slide: data-state="primary-theme" -->

- mikropalveluarkkitehtuuri
- Docker
- tilaton
- curl

Notes:

- mikropalveluarkkitehtuuri, jotta jokainen tiimin jäsen voi työskennellä itsenäisesti
- vain yksi oli käyttänyt dockeria aiemmin
- kaikki tekevät jotain uutta

---

## Teknologiat

<!-- .slide: data-state="primary-theme" -->

- Docker
- Python
- Node.js
- .Net
- Træfɪk
- Redis
- Nginx
- Vue.js

Notes:

- Haluttiin yhdistää kaikkea uutta teknologiaa

---

## Hagathon

<!-- .slide: data-state="primary-theme" -->

- ensimmäiset commitit Tikkurilassa
- määriteltiin rajapinnat
- omat mikropalvelut
- lopputulos demottiin kolmella koneella
- viimeistelyyn viikkoja

Notes:

- Sovittiin, että ennen lähtöä ei koodata

---

## Arkkitehtuuri

<!-- .slide: data-state="primary-theme" -->

![Arkkitehtuuri](../assets/images/png/arkkitehtuuri.png)

- isomofrinen fysiikkaengine
- load balancerit yhteyksissä

Notes:

- traefik api gatewayna, tarjoaa load balancerit
- enginen toiminta
