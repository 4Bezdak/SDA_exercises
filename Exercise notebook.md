## Easy

#### Vyčistit telefonní číslo
# napište funkci která ze stringu telefonního čísla vrátí pouze číslice
# funkce bude univerzální na různé inputy
# output v int

např:
    ""+1 (613)-995-0253" --> 16139950253
    "613-995-0253" --> 6139950253
    "1 613 995 0253" --> 16139950253
    


```python
def normalize_numbers(number_str):
    pass
```

#### Převrátit číslo
# Převrátit zadané číslo:
Např 123 --> 321 
# funkce musí převracit i negativní čísla
-123 --> -321

```python
def reverse_number(int_number):
    pass
```

#### Úspěšní/Neúspěšní studenti
# Napište funkce na následující operace s danám listem výsledků zkoušek
student_scores = [90.33, 40.5, 55.44, 70.05, 30.55, 25.45, 80.45, 95.3, 38.7, 40.3]

# 1) zaokrouhlit na celé čísla --> output [90, 41, 55...]
# 2) vyfiltrujte úspěšné studenty. Úspěšní jsou ti, kteří mají skóre nad 50  --> output [90, 55 ...]
# 3) spočítejte kolik studentů nesplnilo zkoušku --> output 5
#### Scrabble 
tabulka hodnot písmen:
    Letter                           Value
A, E, I, O, U, L, N, R, S, T       1
D, G                               2
B, C, M, P                         3
F, H, V, W, Y                      4
K                                  5
J, X                               8
Q, Z                               10

Napište funkci která spočítá hodnotu slova ve Scrabblu:
např: 
"Python" -> 14

```python
def scrabble_value(word):
    pass
```

## Not so  easy

#### Závorky
 # napiště fuknci která ověří jestli v textu jsou všechny závorky uzavřené a i ve správném pořadí
# typy závorek [] {}, ()

Příklad text = "Kocka neni pes(leda ze by byl[ale to by byl na indexu {i}])" -> True 
               "Kocka neni pes(((leda ze by byl[]ale to by byl na indexu {i}])" -> False

```python
def matching_brackets
```

#### Is ascending
#Určete jestli čísla v listu jsou v vzestupném pořadí
example_list_1 = [1,4,8,23,39] --> True
example_list_2 = [1,5,2,36,21] --> False


```python
def is_ascending(list_int_number):
    pass
```

#### Ceasarova šifra
# Napiště funcki která enkryptuje zadaný string pomocí Ceasarovi šifry

*Princip Caesarovy šifry je založen na tom, že všechna písmena zprávy jsou během šifrování zaměněna za písmeno, které se abecedně nachází o pevně určený počet míst dále (tj. posun je pevně zvolen).* 
-> v našem případě je posun určený o 3

a --> d, b --> e, x-->a, y--–>b


```python
def encrypt_text(text):
    pass
```

#### Add time easy


```python
Napište funkci která bere dva vstupní argumenty (datový typ každého -> string). 
První je zadaný čas ve 24h formátu (HH:MM)
Druhý je počet hodin a minut které se mají příčíst (ve formátu HH:MM)
Funkce přidá počet hodin a minut k počátečnímu času. Pokud čas je další den, funkce vypíše že to je o XX dní později

output–> add_time("23:20", "3:20") -> "02:40 1 day later"
add_time("13:20", "3:20") -> "14:40"
```


```python
def add_time(start, add):
    pass
```

## Getting Intense here

#### Den narozeni (s datetime modulem)
Napiště funkci která při zadání data narození napíše den v týdnu v kterém se člověk narodil

format_inputu = DD-MM-YYYY

print(day_of_birth("27-04-2022")) # Wednesday

```python
def day_of_birth(date):
    pass
```

#### Text analyzer
text = """Rachel and Joey have their first date. Joey, a specialist in the stuff after the date, tries to lay the groundwork with Rachel, but she keeps slapping his hand away and Joey cannot seem to undo her bra. After talking about it with Monica, Rachel and Joey "power through". Completely taken by the excitement of their first time, Rachel, while climbing onto Joey, accidentally sinks her knee into his groin, preventing him from performing. The two stop to reflect on their sexless experience and how this affects their relationship, and when they talk to Chandler about it, they realize that their friendship is too strong for them to take it beyond. The two break up amicably."""

# napište analyzátor textu který vrátí kolikrát je které slovo v textu + set interpunkčních znamének (.,;")

output --> {"Rachel": 3, "Joey":5, "a":3, "special_char":{",", ".", ":"}}

```python
def text_analyzer(text):
    pass
    
```

#### Integer na Římské čísla


```python
# Napište funkci která převede int číslo na Římské číslice
2022 --> MMXXII
```


```python
def int_to_roman(number):
    pass
```

## I will rather stop with Python...

#### Add_time hardcore
Vytvořte funkci add_time která vyžaduje dva povinné parametry a (jeden volitelný = BONUS)

"11:59 PM" start time in the 12-hour clock format (ending in AM or PM) = Start čas
- "49:05" = hodiny a minuty které se mají přidat k počátečnímu času
# add_time("11:59 PM", "24:05")

- BONUS: (optional) a starting day of the week, case insensitive = den v týdnu
# add_time("11:30 AM", "2:32", "Monday")

Funkce přidá zadaný čas (druhý argument) k počátečnímu času a vrátí ho jako výsledek.

- Pokud výsledek je další den, vytiskne čas a "další den" 
- Pokud je výsledek o x dní později, vytiskne čas a "o x dní pozdějí"

- BONUS:
- Pokud je zadán parametr den v týdnu, ukáže ve výsledku také den v týdnu


```python
def add_time(start, add):
    pass
```
