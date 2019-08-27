## JAVASCRIPT

+++

### Palīgvārdnīca

- Resursu saraksts
- GIT
- Javascript
- Trello

+++

#### Resursu sakraskts

- [W3Schools HTML [ENG]](https://www.w3schools.com/html/default.asp)
- [W3Schools CSS [ENG]](https://www.w3schools.com/css/default.asp)
- [W3Schools Bootstrap4 [ENG]](https://www.w3schools.com/bootstrap4/default.asp)
- [W3Schools JS [ENG]](https://www.w3schools.com/js/default.asp)
- [W3Schools How To [ENG]](https://www.w3schools.com/howto/howto_css_menu_icon.asp)
- [MDN HTML pamati [ENG]](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started)
- [MDN CSS pamati [ENG]](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/How_CSS_works)
- [MDN Javascript pamati [ENG]](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript)

+++

#### GIT Špikeris, Soļi

- Veicam izmaiņas pirmkodā
- Saglabājam veiktās izmaiņas
- Pievienojam izmaiņas, jeb git add
- Veicam GIT apņemšanās, jeb git commmit
- Aizsūtam izmaiņas uz GitHub repozitoriju, jeb git push

+++

#### GIT Vizuālais Špikeris

@img[](assets/img/git-workflow-simple.png)

+++

#### Es kā izstrādātājs gribētu izvietot savu html kodu globālajā tīmeklī izmantojot GitHub Pages

- Atveram savu github repozitoriju
- Atveram repozitorija iestatījumus
- Atrodam iestatījumos GitHub Pages
- Uzspiežam uz pogas ar tekstu None
- Izvēlamies no saraksta master branch

---

### Uzdevums 1 - Funkcijas un to izsaukumi

- Izveidot funkciju kura palielina i mainīgā vērtību
- Izveidot funkciju kura samazina i mainīgā vērtību, bet i var būt tikai naturāls skaitlis
- Piesaistīt šīs funkcijas pie pogām
- Izveidot ievada logu, kura vērtība tiktu mainīta uz i mainīgā vērtību pie pogas nospiešanas

+++

#### Es kā **izstrādātājs** gribētu zināt kā **atkļūdot savu kodu**, lai kļūdu meklējumi aizņemtu mazāk laika

- Atveram savu mīļāko pārlūku
- Atveram Developer Tools jeb iztrādātāja rīkus
  - Nospiežam F12 VAI
  - Nospiežam kreiso peles taustiņu uz brīvās vietas un izvēlamies atkarībā no pārlūka
    - Chrome - "Inspect"
    - Edge - "Inspect element"
    - IE11 - "Inspect element"
    - Mozzilla Firefox - "Inspect element"

+++

#### Es kā izstrādātājs gribētu zināt vairāk par JS pamata sintaksi, lai es varētu sākt programmēt JS valodā

```html
<script type="text/javascript">
const a = 5;
let b = 3;

if (a !== b) {
    const pazinojums = `${a} nav vienāds ar ${b}`;
} else {
    const pazinojums = a + " ir vienads ar " + b;
}
console.log(pazinojums)
</script>
```

+++

#### Es kā izstrādātājs gribētu zināt vairāk par JS pamata sintaksi, lai es varētu sākt programmēt JS valodā (2)

```html
<script type="text/javascript">
const a = 5;
let b = 3;
var pazinojums;

if (a !== b) {
    pazinojums = `${a} nav vienāds ar ${b}`;
} else {
    pazinojums = a + " ir vienads ar " + b;
}
console.log(pazinojums);
</script>
```

+++

#### Es kā izstrādātājs gribētu zināt vairāk par JS funkcijām, lai es varētu mazāk atkārtot savu pirmkodu

```javascript
function summa(a, b) {
    return a + b;
}

summa(2,2);
```

```javascript
function hipotenuza(a, b) {
    return Math.sqrt(a * a + b * b);
}

hipotenuza(4,5);
```

---

### Uzdevums 2 - Manipulācijas ar masīvu

- Izveidot funkciju, kura pievienos vērtību masīva beigās
- Izveidot funkciju, kura izņems vērtību no masīva beigām
- Izveidot funkciju, kura izdrukās visu masīvu kā HTML DOM elementu
- Izveidot funkciju, kura iestarpinās jaunu elementu masīvā pēc norādītā indeksa
- Izveidot funkciju, kura izņems elementu no masīva pēc norādītā indeksa

+++

### Es kā izstrādātājs gribētu labāk strukturēt savu programmatūras kodu, lai tas būtu vienkāršāk pārvaldāms un saprotams

+++

#### Es kā izstrādātājs gribētu zināt vairāk par JS masīviem

```javascript
const masivs = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9];
let i = 0;
do {
    masivs[i++];
} while (i < masivs.length);
```

```javascript
const masivs = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9];
let i = 0;
while (i < masivs.length) {
    masivs[i++];
};
```

```javascript
const masivs = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9];
for (let i = 0; i < masivs.length; i++) {
    masivs[i++];
};
```

---

### Uzdevums 3 - Manipulācijas ar objektiem

- Izveidot funkciju, kura pievienos jaunu atslēgu ar vērtību objektam
- Izveidot funkciju, kura dzēsīs atslēgu (un tās vērtību) no objekta
- Izveidot funkciju, kura izdrukās visas objekta atslēgas un to vērtības

+++

#### Es kā izstrādātājs gribētu zināt vairāk par JS objektiem

```javascript
const obj = {
    atslega: "vertiba",
    key: "value"
};

console.log(Object.keys(obj));
console.log(Object.values(obj));
console.log(obj);

delete obj.atslega;
console.log(obj);

obj.key = undefined;
console.log(obj);

```

---

### Uzdevums 4 - Darbības ar DOM elementiem

- Izveidot funkciju, kura izveidos jaunu HTML "form" DOM elementu
- Izveidot funkciju, kura pievienos HTML DOM "form" elementam jaunu rindu ar diviem ievadlaukiem un pogu
- Izveidot funkciju, kura 2 punktā pievneotās pogas nospiešanas gadījumā dzēstu no HTML DOM formas to rindu kurā atrodas šī nospiestā poga
- Pievienot formai pogu "Pievienot rindu" ar kuras nospiešanu tiks izpildīta funkcijas no otrā punkta
- Izveidot funkciju kura parādītu visu ievad lauku saturu kā javascript objektu, pirmais lauks - atslēga, otrais lauks - vērtība

+++

#### Es kā izstrādātājs gribētu zināt vairāk par HTML DOM

![HTML DOM](https://www.w3schools.com/whatis/img_htmltree.gif)

---

### Uzdevums 5 - Klašu izmantošana

- Pārveidot 4 uzdevuma risinājumu tā, lai tas izmantotu klasi ar metodēm nevis vienkārši funkcijas

+++

#### Es kā izstrādātājs gribētu zināt vairāk par JS klasēm

```javascript
  class Kava {
    kartis = [];
    constructor() {
      for (let suit = 0; suit < 4; suit++) {
        kartis.push([]);
        for (let type = 0; type < 13; type++) {
          kartis[suit].push(type);
        }
      }
    }

    dealCard() {
      // ...implementation
    }

    drawCard(suit, type) {
      // ...implementation
    }
  }
```

---

### Uzdevums 6 - Darbības ar DOM elementiem (padziļināti)

- Pārveidot 5. uzdevuma klasi lai tā nestrādātu pa tiešu ar DOM elementiem, bet gan mainītu javascript objektu un pēc izmaiņām izsauktu speciālu metodi, kura pārveidotu šo objektu par HTML DOM

+++

#### Es kā izstrādātājs gribētu zināt vairāk par JS HTML bibliotēkām

- jquery
- React
- Angular
- node modules
