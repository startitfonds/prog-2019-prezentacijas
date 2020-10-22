## Prezentācija tiešsaistē

#### https://ej.uz/startit-python

---

## Ievads Python

---?color=linear-gradient(90deg, white 50%, black 50%)

@snap[west span-30 text-center]

#### Kāpēc Python?

#### Ievads Python

@snapend

@snap[north-east span-60 text-12]
@box[bg-gold text-white box-padding](Pielietojums)
@snapend

@snap[east span-60 text-12]
@box[bg-green text-white box-padding](Ievads sintaksē)
@snapend

@snap[south-east span-60 text-12]
@box[bg-blue text-white box-padding](Salīdzinājums ar JS)
@snapend

---

### Kāpēc Python?

@ul

- Vienkārša sintakse
  - (ja zina angļu valodu @fa[solid-smile-wink] )
- Dažādas izmantošanas iespējas
- Populāra kā pirmā programmēšanas valoda
  - Vadošajās ASV universitātēs
  - ne-programmētājiem
  - profesionālās izglītības kursos
- Daudz tiešsaistē materiālu

@ulend

+++

### Izmantošana

@ul
- datu apstrāde (NumPy, SciPy, Pandas)
- tīmekļa lapas (Flask, Bottle, Django)
- mašīnmācīšanās (OpenCV, PyTorch, TensorFlow)
- robotika (pyFirmata)
@ulend

---

### Sintakses īpatnības

- Atkāpēm (atstarpēm) ir nozīme ...
- ... jo bloki tiek apzīmēti ar atkāpi
- Piespiež ievērot formatēšanas labo stilu
- Palīdz ar koda lasāmību

+++

### Bloki

- Lieto 4 vai 2 atstarpes
- moderni redaktori automātiski palīdz

+++

#### Bloku piemērs

```python
def piemers():
    diena = 22
    if diena == 22:
        print("Kursu diena!")
    return diena

piemers()
```

@snap[south span-100 text-10]

@[1](funkcijas deklarācija)
@[2-5](funkcijas definīcijas bloks ar atkāpi)
@[4](zarošanās bloks ar atkāpi)
@[7](funkcijas izsaukšana)

@snapend

---

## Kā to lietot

+++

#### Pamata datu tipi

```python
virkne = "Labrīt, skolotāji!"
virkne2 = 'Var arī šādi'
vesels_skaitlis = 10
decimalskaitlis = 2.5
pareizi = True
nepareizi = False
nav = None
```

@snap[south span-100 text-10]

@[1,2](string)
@[3](int)
@[4](float)
@[5,6](boolean)
@[7](empty value)
@snapend

+++

#### Datu tipu pārveidošana

```python
virkne = "10"
skaitlis = 12
skaitlis2 = int(virkne)     # 10
skaitlis3 = float(virkne)   # 10.0
skaitlis4 = float(skaitlis) # 12.0
virkne2 = str(skaitlis)     # "10"
```

@snap[south span-100 text-10]

@[1,6](string)
@[2,3](int)
@[4,5](float)
@snapend

+++

#### Datu struktūras

```python
masivs = ["viens", 2, "trīs", 4.0]
vardnica = { "diena": 22, "menesis": 10 }
divdimensiju = [[0, 0],
                [0, 0]]
salikts =   [
                {"id": 1, "vards": "Anna"},
                {"id": 2, "vards": "Bruno"}
            ]
```

@snap[south span-100 text-10]

@[1,3-4](list)
@[2](dictionary)
@[5-8](list of dictionaries)
@snapend

+++

#### Operatori

```python
a = 1
b = 2 + 3 -7
c = (2 ** 5) - (2 * 2)
dalijums = 12 / 10      # == 1.2
vesela_dala = 12 // 10  # == 1
atlikums = 12 % 10      # == 2
```

@snap[south span-100 text-10]

@[1](piešķir vērtību)
@[2](saskaita, atņem)
@[3](kāpina, reizina)
@[4](iegūst dalījuma rezultātu kā float)
@[5](iegūst dalījuma veselo daļu kā integer)
@[6](iegūst dalījuma atlikumu kā integer)

@snapend

+++

#### Ievade un izvade

```python
teksts = input()
teksts2 = input("Ievadiet vārdu: ")
skaitlis = int(input())
skaitlis2 = int(input("Ievadiet skaitli: "))
print(teksts)
print(skaitlis)
```

@snap[south span-100 text-10]
@[1,2](Tekstu ievieto mainīgajā)
@[3,4](Tekstu pārveido par skaitli un ievieto mainīgajā)
@[5-6](Lieto mainīgos, lai izvadītu datus)
@snapend

+++

#### Izvade

```python
vards = "Maris"
skaitlis = 22
sveiciens = "Labrīt, " + vards
sveiciens2 = "Labrīt, {}".format(vards)
diena = "Šodien ir " + str(22) + " oktobris"
diena2 = "Šodien ir {}. oktobris".format(skaitlis)
print(sveiciens)
print(diena2)
```

@snap[south span-100 text-10]
@[1,2](Definē mainīgos)
@[3,4](Tekstu kombinē ar citu tekstu un ievieto mainīgajā)
@[5-6](Tekstu kombinē ar skaitli un ievieto mainīgajā)
@[3,5](Līdzīgi kā Javascript)
@[4,6](Ertāka Python sintakse)
@snapend

+++

#### Zarošanās

```python
diena = 22
if diena == 21:
    print("Pirmā kursu diena!")
elif diena == 22:
    print("Otrā kursu diena!")
else:
    print("Parasta diena")
```

@snap[south span-100 text-10]
@[1](Definē mainīgos)
@[2,4](veic salīdzinājumu)
@[6](izpilda, ja neatbilst nevienam nosacījumam)
@[3,5,7](izpildāmais bloks ar atkāpi!)
@snapend

+++

#### Salīdzinājuma operatori

```python
2 == 2              # = =
2 != 3              # ! =
2 < 3               # <
2 <=3               # < =
2 in [1, 2, 3]
```

@snap[south span-100 text-10]
@[1](vienāds)
@[2](nav vienāds)
@[3](mazāks)
@[4](mazāks vai vienāds)
@[5](ir atrodams sarakstā)
@snapend

---

@snap[north-east]
#### Sintakses salīdzinājums
@snapend

@snap[west span-50]
#### Python

```python
# Šis ir komentārs
print("Čau!")
```
@snapend

@snap[east span-50]

#### JavaScript

```javascript
// Šis ir komentārs
console.log("Čau!");
```

@snapend

+++

@snap[north span-100 text-smallcaps]
### Funkciju definēšana

@snapend

@snap[west span-50]

#### Python

```python
# definējam funkciju
def sveiciens(vards):
    print("Labrīt, " + vards)

# izsaucam funkciju
sveiciens("Evija")
```
@snapend

@snap[east span-50]

#### JavaScript

```javascript
// definējam funkciju
function sveiciens(vards) {
    console.log("Labrīt, " + vards);
}
//izsaucam funkciju
sveiciens("Evija");
```
@snapend

---

### Laiks praktizēties!

- https://snakify.org/en/
- https://codingbat.com/python
- https://www.learnpython.org/en/Welcome

---

@snap[north span-100 text-smallcaps]
#### Zarošanās
@snapend

@snap[west span-50]

#### Python

```python
def pozitivs(skaitlis):
    if skaitlis > 0:
        return True
    else:
        return False


```
@snapend

@snap[east span-50]

#### JavaScript

```javascript
function pozitivs(skaitlis) {
    if (skaitlis > 0) {
        return true;
    } else {
        return false;
    }
}
```
@snapend

+++

@snap[north span-100 text-smallcaps]
#### if-elif-else piemērs
@snapend

```python
def dalisana(skaititajs, saucejs):
    if skaititajs == 0:
        return 0
    elif saucejs == 0:
        return "Ar 0 dalīt nedrīkst!"
    else:
        return skaititajs /  saucejs
```

@snap[south span-100 text-10]

@[1](definējam funkciju ar diviem parametriem)
@[2,4,6](zarošanās nosacījumi)
@[2-3](pārbaudam pirmo nosacījumu)
@[4-5](pārbaudam citu nosacījumu)
@[6-7](izpildam visos citos gadījumos)

@snapend

+++

@snap[north span-100 text-smallcaps]
#### Cikli (for .. in range ...)
@snapend

```python
for i in range(5):
    print(i)

for i in range(5, 11):
    print(i)

for i in range(2, 11, 2):
    print(i)
```

@snap[south span-100 text-10]
@[1](Cikls izpildās no 0 (pēc noklusējuma) līdz 4 (5 neieskaitot) ar soli 1)
@[2](Izdrukā 5 skaitļus - 0, 1, 2, 3, 4)
@[4](Cikls izpildās no 5 līdz 10 ar soli 1)
@[7](Cikls izpildās no 2 līdz 10 ar soli 2)
@snapend

+++

@snap[west span-50 text-center]
#### Python

```python
for i in range(5):
  print(i)

```
@snapend

@snap[east span-50 text-center]

#### JavaScript

```js
for (let i = 0; i < 5; i += 1) {
  console.log(i);  
}
```

@snapend

+++

@snap[north span-100 text-smallcaps]
#### Cikli (for .. in ...) ar iterable
@snapend

```python
vards = "zebra"
for burts in vards:
    print(burts)

masivs = ["viena", "maza", "turku", "pupa"]
for elements in masivs:
    print(elements)

for i in range(len(masivs)):
    print(i, masivs[i])
```

@snap[south span-100 text-10]
@[1,2](Cikls ņems pēc kārtas simbolus no string mainīgā)
@[3](Izdrukā simbolus (burtus) atsevišķi)
@[5,6](Cikls ņems masīva elementus pēc kārtas)
@[7](Izdrukā masīva elementus atsevišķi)
@[9](Var izmantot range un masīva vai string garumu)
@[10](Tādā gadijumā vērtībai jāpiekļūst izmantojot indeksu)
@snapend

+++

@snap[north span-100 text-smallcaps]
#### Cikli (for .. in ...) ar vārdnīcu
@snapend

```python
vardnica = {"viens": "one", "divi": "two", "trīs": "three"}

for atslega in vardnica:
    print(atslega, vardnica[atslega])

for atslega, vertiba in vardnica.items():
    print(atslega, vertiba)

vardnica["cetri"] = "four"

```

---

## Darbības ar failiem

+++

@snap[north span-100 text-smallcaps]
#### Failu darbību vispārīgs apskats:
@snapend

@ul
- atver failu
  - kur atrodas?
  - kāda veida (teksta vai binārs)
  - ko vēlas darīt (lasīt, rakstīt, pievienot)
- veic datu operāciju
  - nolasa
  - ieraksta
- aizver failu
@ulend

+++

### Failu darbības ar Python

```python
with open("dati.txt", "r") as f:
    dati = f.readlines()

for rinda in dati:
    print(rinda)
```

@snap[south span-100 text-10]
@[1](atver failu, norādot faila vārdu un atvēršanas veidu)
@[2](ielasa teksta faila saturu masīvā)
@[3](with bloks beidzies, fails tiek automātiski aizvērts)
@[4,5](dati ir pieejami, izdrukā teksta faila saturu)
@snapend

+++

```python
with open("jauns.txt", "w") as jauns:
    jauns.write("Izveidoju jaunu failu!")
```

```python
with open("jauns.txt", "a") as klaat:
    klaat.write("\nPievienoju jaunu rindiņu!\n)
```

```python
with open("bilde.png", "rb") as bilde:
    # kaut ko ar bināru failu ...
```

+++

### Darbības ar teksta failiem

@ul
- vienkārši teksta faili *.txt
- tabulāri dati, atdalīti ar simbolu *.csv
- formatēti dokumenti *.doc
- web lapas *.html
- json dokumenti *.json
@ulend

+++

### *.txt

@ul
- var vienkārši lasīt izmantojot iebūvēto funkcionalitāti
- rindas ir atdalītas ar "\n"
- rakstot "\n" ir jāpievieno, ja grib jaunu rindu
@ulend
