# Ataskaita ir Išvados

## Duomenų Paruošimas

Duomenys buvo išvalyti naudojant specialiai sukurtą funkciją, kuri pašalina HTML tagus, skaičius, specialiuosius simbolius ir konvertuoja tekstą į mažąsias raides.

## Modelių Kūrimas ir Vertinimas

Buvo sukurti trys klasifikavimo modeliai: logistinė regresija, atsitiktinių miškų klasifikatorius ir dirbtinis neuroninis tinklas. Modeliai buvo vertinami pagal tikslumą, atpažinimo tikslumą ir F1 balą.

### Modelių Rezultatai

- **Logistinė regresija:** Tikslumas - 0.8693, Atpažinimo tikslumas - 0.8768, F1 balas - 0.8711
- **Atsitiktinių miškų klasifikatorius:** Tikslumas - 0.8396, Atpažinimo tikslumas - 0.8373, F1 balas - 0.8403
- **Dirbtinis neuroninis tinklas:** Tikslumas - 0.8635, Atpažinimo tikslumas - 0.8710, F1 balas - 0.8654

### Geriausio Modelio Optimizavimas

Buvo atliktas atsitiktinių miškų klasifikatoriaus hiperparametrų optimizavimas. Geriausiai parinkti hiperparametrai: `{'max_depth': None, 'n_estimators': 100}`. Po optimizacijos modelio tikslumas šiek tiek pagerėjo.

## Reagavimo Būtinybės Nustatymas

Buvo identifikuoti atsiliepimai, į kuriuos reikia sureaguoti, naudojant kritinius sentimentų įvertinimus, raktinius žodžius ir ilgio kriterijus.

## Išvados

- Logistinė regresija pasirodė geriausiai pagal visus vertinimo kriterijus.
- Atsitiktinių miškų modelis po hiperparametrų optimizacijos pasiekė geresnius rezultatus.
- Modeliai gali būti naudingi identifikuojant svarbius vartotojų atsiliepimus, kuriems reikalingas greitas reagavimas.

