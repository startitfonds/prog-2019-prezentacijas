## Prezentācija tiešsaistē

#### https://ej.uz/python-flask

---

+++

## Turpmākais plāns

@ul
- Serveri
  - Pieprasījumu apstrāde
  - Ietvari
  - Failu sūtīšana
@ulend

+++

### Vairāk darbosimies praktiski!

+++

## Kas ir serveris?

@ul
  - Serveris ir datorsistēma klienta servera arhitektūrā, kas nodrošina klientu pieprasījumu apstrādi un nosūta tiem atbildes.
  - Serveris ir arī datorprogramma vai programmu kopums, kas nodrošina klienta programmu pieprasījumu apstrādi.
  - Šo arī var izlasīt Wikipedia (https://lv.wikipedia.org/wiki/Serveris)
@ulend

+++

## Serveru veidi

@ul
  - HTTP (WEB)
  - DHCP
  - DNS
  - EMAIL
  - FTP
  - Šo arī var izlasīt Wikipedia (https://lv.wikipedia.org/wiki/Serveris)
@ulend

+++

### Darbosimies vairāk praktiski

Abstrahēsimies no visiem serveru veidiem un paliksim pie WEB servera

@ul
- Kam tie vajadzīgi?
- Kur tos izmanto?
- Kādi reāli dzīves pielietojumi?
- Kad var iztikt bez servera?
- Ko nozīmē darboties ar WEB serveriem
  - Datubāzes
  - Tiesības
  - Rezerves kopijas
  - Strāvas bojājumi
  - Tīkla bojājumi
@ulend

+++

## Mūsdienu serveru puses izstrāde

@ul
- Back-end
- Front-end
- Serveri var rakstīt (konfigurēt/uzstādīt) pats, bet vai tas ir efektīvi
- Viss ir individuāli un atkarīgs no vajadzības
- Dažādas valodas, dažādi tīmekļizstrādes ietvari:
  - PHP (Slim, Laravel)
  - Ruby (Rails)
  - Python (Django, Flask)
@ulend

+++

## Nedaudz par manu pieredzi

### Kā es saskāros ar serveriem?

@ul
  - Word-press
  - Self-service sistēma (PHP)
  - Vienkāršas vizītkāršu tipa lapas (PHP)
  - Jau kaut kas nopietnāks ar RoR (Ruby)
@ulend

+++

## Kādu ietvaru izmantosim mēs?

@ul
  - Tā kā mēs darbojamies ar Python, tad izmantosim kādu no dotās valodas ietvariem
  - Sāksim no pamatiem, tāpēc ērts būs mikro ietvars Flask
  - Analoģiski PHP Slim ietvars
@ulend

+++

## Pietiks pļāpāt, tagad sāksim darboties praktiski

@ul
  - Pieslēdzamies repl.it
  - Piestartējam FLASK serveri
  - Izveidojam vienkāršu index skatu, kas atgriež 'Sveika pasaule!'
  - Veicam pieprasījumu caur
    - fetch
    - postman
    - pārlūku
@ulend

+++

## Fetch piemērs

### Ja mūs interesē lapas saturs (body)

```javascript
fetch(new Request('https://flask-tutorials.akmakit.repl.co/'))
        .then((resp) => resp.text())
        .then((data) => console.log(data))

```

+++

## Fetch piemērs

### Ja mūs interesē json

```javascript
fetch(new Request('https://flask-tutorials.akmakit.repl.co/'))
  .then((resp) => resp.json())
  .then((data) => console.log(data))
```

+++

## Ja mūs interesē HEADERS

```javascript
fetch(new Request('https://flask-tutorials.akmakit.repl.co/))
  .then((resp) => resp.headers.forEach(header => console.log(header)))
  .then((data) => console.log(data))
```

+++

## Tālāk turpināsim darboties praktiski

### Turpināsim ar citu vienkāršu pieprasījumu

@ul
  - Apstrādāsim pieprasījumus:
    - about
    - contact
@ulend

+++

## Tālāk turpināsim darboties praktiski

### Tagad mēs gribētu atgriezt HTML dokumentu ar padotu parametru

@ul
  - Apstrādāsim pieprasījumus:
    - about
    - contact
@ulend

+++

## Tālāk turpināsim darboties praktiski

### Tagad mēs gribētu padod parametrus un padarboties ar tiem

@ul
  - Apstrādāsim pieprasījumus:
    - Padosim parametrus paši un tos atgriezīsim
    - Atgriezīsim objektu kā simbolu virkni
    - Atgriezīsim objektu kā JSON
    - No padotajiem parametriem uzzīmēsim tabulu iekš HTML
@ulend

+++

## Tālāk turpināsim darboties praktiski

### GET apskatījām, tālāk laiks POST, DELETE

@ul
  - Apstrādāsim pieprasījumus:
    - Izveidosim POST pieprasījumu
    - Ierakstīsim datus failā
    - Nolasīsim no faila
    - Uzzīmēsim faila saturu tabulas veidā
    - Nolasīsim rindu no faila
    - Izdzēsīsim rindu no faila
@ulend

+++

## Tālāk turpināsim darboties praktiski

### Paskatīsimies, kā varam atgriezt faila saturu balstoties uz pieprasījuma tipu

@ul
  - Apstrādāsim pieprasījumus:
    - application/json
    - text/plain
    - text/html
    - kā ar neapstrādātiem pieprasījumiem?
@ulend

+++

## Tālāk turpināsim darboties praktiski

### Saglabāsim attēlu uz servera

@ul
  - Apstrādāsim pieprasījumus:
    - multipart/form-data
    - izveidosim vietu, kur glabāt failus
    - saglabājam failu
@ulend
