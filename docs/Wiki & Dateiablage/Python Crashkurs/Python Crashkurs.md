---
Owner: FFlorian Hoos
tags:
  - Programmierung
Last edited time: 2024-02-26T13:15
---
### **1. Variablen und Datentypen:**

```Python
pythonCopy code
# Variablenzuweisung
x = 5
name = "Max"
ist_wahr = True

# Datentypen: int, float, str, bool
y = 3.14
text = "Hallo"
ist_falsch = False
```

Man beachte, dass es bei Python keine festen Variablen gibt. D.h. der Datentyp wird automatisch festgelegt. Man kann jedoch Variablen zwingen ein Datentyp anzunehmen durch [casting](https://www.w3schools.com/python/python_casting.asp).

### **2. Bedingungen und Schleifen:**

```Python
pythonCopy code
# Bedingungen (if-elif-else)
if x > 0:
    print("x ist positiv")
elif x == 0:
    print("x ist Null")
else:
    print("x ist negativ")

# Schleifen (for und while)
for i in range(5):
    print(i)

counter = 0
while counter < 5:
    print(counter)
    counter += 1

```

### **3. Listen und Dictionaries:**

```Python
pythonCopy code
# Listen (Arrays)
zahlen = [1, 2, 3, 4, 5]
namen = ["Max", "Anna", "Eva"]

# Zugriff auf Elemente einer Liste
print(zahlen[0])  # Ausgabe: 1
print(namen[1])   # Ausgabe: Anna

# Dictionaries (Schlüssel-Wert-Paare)
person = {"name": "Max", "alter": 30, "stadt": "Berlin"}

# Zugriff auf Werte in einem Dictionary
print(person["name"])  # Ausgabe: Max
print(person["alter"]) # Ausgabe: 30

```

### **4. Funktionen:**

```Python
pythonCopy code
# Funktionen definieren
def quadrat(x):
    return x * x

# Funktion aufrufen
ergebnis = quadrat(3)
print(ergebnis)  # Ausgabe: 9

```

### **5. Dateiverarbeitung:**

```Python
pythonCopy code
# Datei öffnen und lesen
with open("datei.txt", "r") as f:
    for line in f:
        print(line.strip())

# Datei schreiben
with open("neue_datei.txt", "w") as f:
    f.write("Hallo, Welt!")
```