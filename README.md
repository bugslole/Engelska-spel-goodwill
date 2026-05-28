# Good Will Hunting — The Game

> *"You wasted all that time trying to be someone you're not."*

Ett interaktivt 3D-spel baserat på filmen **Good Will Hunting** (1997). Spelas direkt i webbläsaren — ingen installation krävs.

---

## Spela spelet

Öppna `good_will_hunting (1).html` i en modern webbläsare (Chrome, Firefox, Edge).

---

## Kapitel

### Kapitel I — MIT Night Shift
Will Hunting arbetar som städare på MIT. Professor Lambeau har skrivit tre omöjliga matematikproblem på en tavla i korridoren. Lös dem alla och möt Lambeau.

- Rör dig mot tavlan och tryck **E** för att öppna ett problem
- Välj rätt svar bland fyra alternativ
- Lös alla tre — följ de gula pilarna till Lambeau

### Kapitel II — South Boston
En gatufight bryter ut. Överlev två vågor av fiender: gängmedlemmar och sedan polisen.

- Slå med **J** (jab), sparka med **K**, blockera med **L**
- Stamina återhämtar sig automatiskt
- Om du förlorar all hälsa visas en WASTED-skärm med val att försöka igen

### Kapitel III — Sean's Office
Will träffar terapeuten Dr. Sean Maguire. En terapisession i flera steg med dialogval som påverkar poängen.

- Gå fram till skrivbordet och tryck **E** för att prata med Sean
- Välj dina svar med omsorg

---

## Kontroller

| Knapp | Aktion |
|---|---|
| `WASD` | Rörelse |
| Mus (håll + dra) | Kameravridning |
| `J` | Punch |
| `K` | Kick |
| `L` | Block |
| `E` | Interagera / prata |
| `ESC` | Stäng dialog / Gå till huvudmeny |

---

## Teknisk översikt

| Del | Teknologi |
|---|---|
| 3D-rendering | Three.js r128 (WebGL) |
| Ljud | Web Audio API (ingen extern lib) |
| Titelanimation | Canvas 2D |
| Spel-logik | Vanilla JavaScript |
| UI/HUD | HTML + CSS |

Hela spelet är en enda HTML-fil (~1 400 rader) utan byggsteg eller beroenden utöver Three.js från CDN.

### Ljud
Klicka på **♪ SOUND OFF** på startskärmen för att aktivera ljud. Webbläsare kräver användarinteraktion innan ljud kan spelas upp.

Ljudmotorn innehåller:
- Meloditema (triangelvågsoscillatorer med delay-eko)
- Regnambians (filtrerat vitt brus)
- Spelljud: punch, kick, träff, framgång, misslyckande

---

## Skärmdumpar av spelflödet

```
Startmeny (regnanimation + stadssilhuett)
    ↓  Välj kapitel → BEGIN
Kapitelnummer-animation (2,4 sek)
    ↓
Gameplay  ←→  Dialog / Math-quiz
    ↓  Klart
Epilog / Nästa kapitel / WASTED-skärm
```

---

## Licens

Skolprojekt. Filmen *Good Will Hunting* ägs av Miramax Films / Disney. Spelet är ett icke-kommersiellt fan-projekt.
