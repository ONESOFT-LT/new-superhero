## Super herojų ataskaitos ir Tavo herojaus sukūrimo sistema.

Pasinaudojant: [SUPERHERO API](https://akabab.github.io/superhero-api/api/#base-url) Reikia sukurti sistemą, kuri pasakytų kuris super herojus yra **geriausias** pagal Tavo pasirinktą herojaus charakteristiką ir pagal komiksų leidėją (**Marvel Comics** arba **DC Comics**)
Rikiavimas turi veikti ir pagal didėjimą ir pagal mažėjimą.

### Galimos herojaus charakteristikos (visi skačiai - integers):
- intelligence
- strength
- speed
- durability
- power
- combat

#### Sistema turi turėti 3 routes:
1. Sąrašas su visais herojais
2. Konkretaus herojaus peržiūra
3. Naujo herojaus sukūrimo forma

### Peržiūrint visą sąrašą turi matytis ši jo informacija:
- Nuotrauka (sm dydžio)
- Vardas
- Pasirinkta charakteristika
- Ar herojus yra geras ar blogas (alignment)

### Peržiūrint konkretų herojų, sistema turi jį atidaryti kitame route su informacija:
- Jo nuotrauka (LG dydžio)
- Ar geras ar blogas (alignment)
- Ūgis (konvertuojant į metrus ir centrimetrus) -> pvz.: 203cm yra 2m ir 3cm
- Svoris (kilogramais)
- Kiti jo vardai (aliases) (biogaphy -> aliases API endpoint'e dalis).

### Superherojaus sukūrimas:
- **Slapyvardis**

- **Chartakteristikos**:
-- intelligence
-- strength
-- speed
-- durability
-- power
-- combat

- **Nuotrauka** (Idealu, jeigu Tavo sistema priimtų vieną foto, kurią po to galėtų resizint į 2 variantus: SM ir LG) - tik PNG formatas ir keliama foto **1000x1000** dydžio

- **Ar herojus yra geras ar blogas**
- **Ūgis** (įvedu informaciją centimetrais)
- **Svoris** (kilogramai)
- **Nurodau kitus vardus** (aliases)

### Ranka sukrutą herojų - turi būti galimybė ištrinti iš sistemos

## Tavo herojus turi būti matomas irgi bendrų herojų sąraše

### Techniniai reikalavimai:
1. Naudojame migracijas duomenų bazės struktūros tvarkymui
2. Komanda (artisan command) - kuri importuoja informaciją iš API
3. Formos validacijos - naudojant Laravel Request klases
4. Puslapiavimas - per 1 psl max 10 herojų
5. Minimum 2 ryšiai

### OPTIONAL (pagal save, papildomi taškai)
1. Livewire komponentų panaudojimas
2. Blade komponentų panaudojimas
3. Tailwind css instaliavimas per NPM ir panaudojimas dėliojant interface.
4. Serviso sukūrimas (koks servisas - fantazijos reikalas)

Dizainas ir išdėstymas - pagal save. Kad būtų paprasčiau - pateikiam wireframe nuorodą, kad suprast ką reikia atvaizduoti: [WIREFRAME LINK](https://app.moqups.com/gZDL8Wt1lUzKBFQW0mnk3MHfwqgDGBYJ/view?ui=0&fit_width=1)
