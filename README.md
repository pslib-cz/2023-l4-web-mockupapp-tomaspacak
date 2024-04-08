# My workout - fitness aplikace
Obsahem tohoto repozitáře jsou podklady pro vytvoření fitness aplikace, která se soustředí možnost sestavení svých vlastních tréninkových plánů. Jednotlivé podklady jsou rozebrány v tomto souboru.

## Tabulka - katalog cviků
Tato kapitola slouží jako průvodce katalogem cviků, který ma sloužit jako podklad pro vytvoření databáze cviků pro fitness aplikaci. Tabulka je rozdělena do několika sloupců, které obsahují potřebné informace o jednotlivých cvicích. Sloupce Kategorie I a Kategorie II by měly být implementovány jako atribut v databázovém modelu, aby uživatelé mohly snadno filtrovat cviky podle jejich preferencí. Níže je popsán účel a obsah každého sloupce:
### Jméno Cviku
- **Popis:** Oficiální název cviku
- **Typ:** Text
- **Příklad:** Dřepy, Bench press

### ID
- **Popis:** Jedinečný identifikátor cviku v databázi
- **Typ:** Číslo
- **Příklad:** 1, 2

### Kategorie I
- **Popis:** Rozdělení cviků na cviky s vlastní vahou nebo cviky s vybavením
- **Typ:** Text
- **Příklady:** S, P

### Kategorie II
- **Popis:** Specifikuje, na jakou svalovou skupinu je cvik zaměřen
- **Typ:** Text
- **Příklady:** Nohy, Hrudník, Záda, Ramena, Břicho

### Popis
- **Popis:** Stručný popis cviku
- **Typ:** Text
- **Příklad:** Dřepy jsou základní cvik na posílení dolní části těla, kde z pozice stojícího postavení  jdete do dřepu a zpět.

### Náročnost
- **Popis:** Obtížnost cviku pro orientační účely.
- **Typ:** Text
- **Příklady:** Začátečník, Střední, Pokročilý

### Primární svaly
- **Popis:** Hlavní svalové skupiny aktivované během cviku.
- **Typ:** Text
- **Příklady:** Quadriceps, Hamstrings, Glutes

### Sekundární svaly
- **Popis:** Sekundární svalové skupiny, které cvik také zapojuje, ale nejsou hlavním cílem.
- **Typ:** Text
- **Příklady:** Core, Lower back

### Jak na to
- **Popis:** Podrobnější popis správného provedení cviku.
- **Typ:** Text
- **Příklad:** 1. Postavte se rovně s nohama ve šíři ramen. 2. Pomalu se ohněte v kolenou...

## Design a uživatelské rozhraní

### Barevná paleta
Primární barva:
Sekundární barva: rovnoměrný linearní gradient
### Ikony
Ve složce ikony jsou uloženy veškeré potřebné ikony ve formátu SVG.
### Homepage
V dolní části se nachází menu, přes které se lze dostat do tří základních částí aplikace - přehled vytvořených plánů (homepage), sestavení nového tréninkového plánu a moje data.
Na homepage je zobrazen přehled všech vytvořených plánů uživatelem (v případě, že se nevejdou na obrazovku, tak je potřeba vertikálně skrolovat). Pro spuštění plánu je potřeba na něj kliknout.
![homepage] (./img/homepage.png)

#### Spuštěný plán
Nahoře se nacházejí stopky, které měří uplynulý čas při cvičení. Lze je pozastavit pomocí tlačítka pauza dole, stejným tlačítkem se opět spustí. Pod názvem plánu a stopkami se nachází seznam cviků. Vedle každého cviku se nachází ikona, na kterou uživatel klikne, když je s cvikem hotov. Ve chvíli kdy jsou zakliknuta veškerá cvičení, tak je plán ukončen pomocí jediného tlačítka dole, poté je uživatel přesměrován na homepage. Plán lze i předčasně ukončit pomocí tlačítka vedle tlačítka pauza, po té je uživatel automaticky přesměrován na homepage.
![spuštěný plán]()
![dokončený plán]()

### Nový plán
V této části je možné vytvořit nový plán, který se po uložení zobrazí na homepage.

### Moje data
Zde si uživatel zapisuje svoji váhu, obvod pasu, procentuální míru tuku a svalů. Zároveň je zde vidět celkový čas strávený cvičením.
![moje data]()



