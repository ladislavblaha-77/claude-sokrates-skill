# /sokrates — Claude Code skill

Claude Code slash příkaz, který obrací výchozí chování asistenta: na
nahozené téma nedává přímou odpověď, ale reaguje otázkou a cíleně hledá
slabiny, nejasné pojmy a neověřené předpoklady v tom, co řekneš. Jakmile je
spuštěn, zůstává v roli po celou konverzaci, dokud sám neřekneš "shrň to".

Vychází ze tří prvků Sokratovy metody:

- **elenchus** (vyvracení) — netestuje tvrzení přijetím, ale hledáním
  konkrétního případu, kde neplatí
- **maieutika** ("porodnická metoda") — neposkytuje závěr, pomáhá ho
  vytěžit z toho, co už víš
- **eironeia** (předstíraná nevědomost) — ptá se zdánlivě naivně ("co
  přesně tím myslíš?"), protože tam se nejčastěji skrývá nejasnost

Druhá vrstva skillu je meta: nejen vede myšlení v jedné konverzaci, ale na
konci (v souhrnu) pojmenuje, jaké typy otázek byly nejúčinnější, aby ses je
mohl naučit používat sám i bez skillu.

## Instalace

1. Stáhni [`commands/sokrates.md`](commands/sokrates.md)
2. Vlož ho do `.claude/commands/` v projektu, kde ho chceš používat
   (platí jen tam), nebo do `~/.claude/commands/` (platí ve všech
   projektech)

## Použití

```
/sokrates Co je pro náš tým teď nejdůležitější?
```

Skill zůstává v roli celou konverzaci. Pro ukončení a shrnutí napiš
cokoliv ve smyslu "shrň to" / "udělej souhrn" — dostaneš dvě věci:

1. obsahový závěr (co se vyjasnilo, co zůstalo otevřené)
2. meta-vrstvu (jaké typy otázek byly nejúčinnější, abys je příště použil
   sám)

## Kdy to použít

Produktová/strategická rozhodnutí, konflikty priorit, předpoklady před
velkým rozhodnutím, osobní reflexe — kdykoli má smysl nejdřív vyjasnit
vlastní myšlení, než dostat hotovou odpověď.

## Kdy to nepoužívat

Když potřebuješ rychlou faktickou odpověď — skill ji záměrně nedává, dokud
ho neukončíš souhrnem.

## Licence

MIT — viz [LICENSE](LICENSE).
