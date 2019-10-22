## Ievads Python

---?color=linear-gradient(90deg, white 50%, black 50%)

@snap[west span-30 text-center]

#### Python valoda

#### repl.it vide

@snapend

@snap[north-east span-60 text-12]
@box[bg-green text-white box-padding](**Kas** tas ir?)
@snapend

@snap[east span-60 text-12]
@box[bg-blue text-white box-padding](**Kāpēc** to vajag?)
@snapend

@snap[south-east span-60 text-12]
@box[bg-gold text-white box-padding](**Kā** to lieto?)
@snapend

---

## Kas tas ir?

+++

### Programmēšanas valoda Python

@ul

- Vienkārša sintakse
- Daudz dažādu izmantošanas iespēju
- Populāra kā pirmā programmēšanas valoda

@ulend

+++

### Sintakses atšķirības

- Atkāpēm ir sintaktiska nozīme
- Bloki tiek apzīmēti ar atkāpi
- Piespiež ievērot formatēšanas labo stilu

---

## Kāpēc mācīties Python

+++

### Kāpēc to vajag vispār?

@ul

- Ir svarīgi mācīties un zināt vairākas valodas
- Paver iespējas vienkārši vadīt dažādas ierīces un procesus

@ulend

+++

### Kāpēc to vajag skolā?

@ul

- izvirzījusies kā populārakā pirmā valoda pasaulē
- Vienkārši sākt
- Iespējams veidot ļoti dažādus projektus

@ulend

---

## Kā to lietot

---?color=linear-gradient(90deg, white 50%, grey 50%)

@snap[west span-50 text-center]

#### Python

```python
# Šis ir komentārs
print("Sveika, pasaule")
```

@snapend

@snap[east span-50 text-center]

#### JavaScript

```javascript
// Šis ir komentārs
alert("Sveika, pasaule");
console.log("Sveika, pasaule");
```

@snapend

+++

@snap[text-20 span-60 text-center]

```python
def sveiciens(vards):
    print("Labrīt, " + vards)

sveiciens("Evija")


> 'Labrīt, Evija'
```

@snapend

@snap[south text-18]

@[1](definējam funkciju)
@[4](izsaucam funkciju)
@[7](rezultāts)
@snapend

+++

@snap[north span-100 text-smallcaps]
### Zarošanās

@snapend

@snap[west span-50 text-18]

Python

```python
def pozitivs(skaitlis):
    if skaitlis > 0:
        return True
    else:
        return False
```

@snapend

@snap[east span-50 text-18]

JavaScript

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

@snap[text-20]

```python
def dalisana(skaititajs, saucejs):
    if skaititajs == 0:
        return 0
    elif saucejs == 0:
        return "Ar 0 dalīt nedrīkst!"
    else:
        return skaititajs /  saucejs
```

@snapend

@snap[south span-100 text-10]

@[1](definējam funkciju ar diviem argumentiem)
@[2,4,6](zarošanās nosacījumi)
@[2-3](pārbaudam pirmo nosacījumu)
@[4-5](pārbaudam citu nosacījumu)
@[6-7](izpildam visos citos gadījumos)

@snapend
