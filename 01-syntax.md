# JS Syntax

### Variablen definieren

JS hat keine statistischen Typen, das heisst, man muss beim Definieren von Variablen keine Datentypen angeben.

Stattdessen verwenden wir das Stichwort `var`.

Beispiel:
```js {cmd=node}
var name = 'Kabi';

console.log(name);

var x = 1;

console.log('x', x);

x = 'Eins';

console.log('x', x);
```

**ACHTUNG** Wenn man `var` vergisst, wird eine globale Variable definiert.

```js {cmd=node}
x = 5

console.log(5)
```

Zusätzlich gibt es noch `let` und `const` um Variablen bzw. Konstanten zu definieren.


### Kommentare

Kommentare sind exakt gleich wie bei Java.

Beispiel:
```js {cmd=node}
console.log(1)
//console.log(2)
console.log(3); //console.log(4)
/* console.log(5)
console.log(6) */
```


# Zahlen

Es gibt nur eine _einzigen_ Datentyp für Zahlen:
`double`


Beispiel:
```js {cmd=node}
console.log(1 + 1)
console.log(0.1 + 0.1)
console.log(0.1 + 0.2)
console.log(0.1 + 0.2 === 0.3)
```


Die üblichen Operatoren funktionieren wie gewohnt:
`+`, `-`, `*`, `/`, `%`


_Empfehlung_: Auf `++` und `--`verzichten.

```js {cmd=node}
var i = 0
//i++
i += 1
```

# Strings

Strings können mit einfachen und doppelten Anführiungszeichen gekennzeichnet werden.

Beispiel:
```js {cmd=node}
console.log('Guten Tag!')
console.log('Hello world')
console.log('Sie haben "Hello" gesagt')
console.log('Er ass bei "Johnny\'s Burger Bude"!')
console.log('\n')
console.log('Festgemauert in der Erde \nstand...')
console.log('\n')
console.log('Früh mmorgens, Asslé, Nsamè, Oléolé, Jong Jong')
```

**Tipp**: In JS-Code einfache Anführungszeichen verwenden, in HTML doppelte.

### Template-Sting

Template-Strings werden mit einfachen Backticks (\`) gemacht. Sie eignen sich gut für mehrzeiligen Te. Mit `$()` kann man beliebige Variablen einfügen.


Beispiel:
```js {cmd=node}
var text = `Drei
Zwei
Eins
Lift off!!!`

console.log(text)
```

```js {cmd=node}
var anrede = 'His royal highness'
var titel = 'Prince'
var vorname = 'Charles'

console.log(`${anrede}, ${titel}, ${vorname} mag gerne Tiere.`)
```

```js {cmd=node}
var anrede = 'Her majesty'
var titel = 'Queen'
var vorname = 'Elizabeth'

console.log(`${anrede}, ${titel}, ${vorname} ist eine excellente Formel 1 Fahrerin!`)
```

### Strings in Zahlen umwandeln

Mit den Funktionen `parseInt`und `parseFloat`können Strings in Zahlen umgewandelt werden.

```js {cmd=node}
var zahl = parseInt('41')

console.log(zahl + 1)
console.log('41' + 1)
console.log(41 + (+ '1')) // HACK!
```

### Methoden von Strings

Überflüssige Leerzeichen entfernen:

```js {cmd=node}
var x1 = `        Hanna        \n\n         `

console.log(x1)
console.log(x1.trim())
```

### Den Anfang eines Strings überprüfen:

```js {cmd=node}
var url = 'HTTPS://www.redhub.com'
var isSecure = url.trim().toLowerCase().startsWith('https')

console.log('Sichere Verbindung', isSecure)
```

