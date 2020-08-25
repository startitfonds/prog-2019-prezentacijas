## repl.it skolotājiem

+++

@snap[north-east span-100 text-smallcaps]
#### repl.it skolotāja skats
@snapend

@img[](assets/img/replit-teacher.png)

+++

@snap[north span-100 text-smallcaps]
### Terminoloģija
@snapend

@ul

- Classroom - uzdevumu grupa
- Assignment - uzdevums
- Assignment instructions - uzdevuma apraksts (instrukcijas)
- Assignment code - uzdevuma sākuma kods
- Test case - automātiskas pārbaudes vienība konkrētam uzdevumam
- Assignment state - uzdevuma statuss (publicēts vai melnraksts)
@ulend

---

@snap[north span-100 text-smallcaps]
### Veidojam jaunu uzdevumu grupu
@snapend

@ul

- Nosauc uzdevumu grupu
  - Specifisku un īsu nosaukumu
    - pēc tēmas (Cikli)
    - pēc mērķa (Pārbaudes darbs, novembris)
- Izvēlās programmēšanas valodu
- Var pievienot aprakstu
- Var pievienot attēlu (vieglāk atpazīt)

@ulend

+++

@snap[north span-100 text-smallcaps]
### Veidojam jaunu uzdevumu
@snapend

@img[](assets/img/replit-teacher-new-assignment.png)

+++

@snap[north span-100 text-smallcaps]
### Izveidots jauns uzdevums
@snapend

@img[](assets/img/replit-teacher-new-assignment-filled.png)

+++

@snap[north span-100 text-smallcaps]
### Izveidojam jaunu I/O testu
@snapend

@img[](assets/img/replit-teacher-create-io-test.png)

+++?image=assets/img/replit-teacher-create-io-testcase.png&size=auto 90%

@snap[north span-100 text-smallcaps]
#### Izveidojam jaunu I/O testa vienību
@snapend

+++

@snap[north span-100 text-smallcaps]
### Publicēšanas iespējas
@snapend

@img[](assets/img/replit-teacher-publish-options.png)

---

@snap[north span-100 text-smallcaps]
### Uzdevums
@snapend

@ul

- izveidojiet savu "classroom"
- izveidojiet vienu uzdevumu
  - ievades / izvades uzdevuma tipu
  - ar instrukciju skolēnam
  - ar sākumkodu
  - ar i/o testu

@ulend

---

@snap[north span-100 text-smallcaps]
### Citu uzdevumu grupu pievienošana
@snapend

@ul

- caur "Import Classroom"
  - [https://repl.it/community](repl.it piedāvātās uzdevumu grupas)
  - pēc atvēršanas jāizvēlas "Import and Teach"
- izmantojot URL uz uzdevumu grupu
  - jebkurš var dalīties ar saviem uzdevumiem
  - automātiski tiek izveidota kopija
  - tiek kopēti uzdevumi un testi, bet ne skolēni
  @ulend

+++

@snap[north span-100 text-smallcaps]
### Nokopējiet Start(IT) izstrādātos uzdevumus
@snapend

@ul

- Javascript
  - [https://repl.it/data/classrooms/share/b1c1caedefb594ceaa2b76343d95cc5d](piemēri)
  - [https://repl.it/data/classrooms/share/342b43a672b896272b701217147054d2](pārbaudes darbu piemēri)
- Python 
  - [https://repl.it/data/classrooms/share/8de26716beb51898aa4d536d97949473](ievaduzdevumi)
  - [https://repl.it/data/classrooms/share/27f00d70db48825f28012c5d98e519b7](failu uzdevumi)
  - [https://repl.it/data/classrooms/share/4735fd68b298152540579f33e27d88a2](pārbaudes darbu piemēri)
  
@ulend

+++

@snap[north span-100 text-smallcaps]
### Uzdevumu grupas iespējas
@snapend

@ul

- redz pievienotos skolēnus
- redz skolēnu progresu
- pieprasa progresu kā *.csv failu
- ielūdz jaunus skolēnus

@ulend

+++

@snap[north span-100 text-smallcaps]
### Uzdevumu grupas skats
@snapend

@img[](assets/img/replit-teacher-student-progress.png)

---

@snap[north span-100 text-smallcaps]
### Uzdevumi ar funkcijām
@snapend

```python
def kvadrats(skaitlis):
  # Aprēķināt skaitļa kvadrātu
  return
```

```python
def pozitivs(skaitlis):
  # Ja skaitlis ir lielāks par 0
  # Atgriezt True
  # Pretējā gadījumā atgriezt False
  return
```

+++

@snap[north span-100 text-smallcaps]
### Vienību testu veidošana
@snapend

@ul

- Jāizdomā testa parametri
- Jāzina, kādām jābūt pareizām atbildēm katram parametram
- Jāizvēlas "Automatic Unit tests (recommended)"

@ulend

+++

@snap[north span-100 text-smallcaps]
### Vienību testa piemērs 1
@snapend

@snap[west span-40]

#### Uzdevums

```python
def kvadrats(skaitlis):
  # Aprēķināt skaitļa
  # kvadrātu
  #
  return
```

@snapend

@snap[east span-60]

#### Vienību testi

```python
self.assertEquals(kvadrats(2), 4)

self.assertEquals(kvadrats(2.1), 4.41)

self.assertEquals(kvadrats(-1), 1)
```

@snapend

+++

@snap[north span-100 text-smallcaps]
### Vienību testa piemērs 2
@snapend

@snap[west span-40]

#### Uzdevums

```python
def pozitivs(skaitlis):
  # Ja lielāks par 0
  # atgriezt True
  # vai atgriezt False
  return
```

@snapend

@snap[east span-60]

#### Vienību testi

```python
self.assertEquals(pozitivs(2), True)

self.assertEquals(pozitivs(0), False)

self.assertEquals(pozitivs(-1), False)
```

@snapend

+++

@snap[north span-100 text-smallcaps]
### Vienību testu veidošanas lapa
@snapend

@snap[west span-50]
@img[](assets/img/replit-teacher-unittest1.png)
@snapend

@snap[east span-50]
@img[](assets/img/replit-teacher-unittest2.png)
@snapend

