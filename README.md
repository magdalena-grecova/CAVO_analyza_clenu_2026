# Analýza členské základny ČAVO (2026)

**Autor:** Magdalena Grecová  
**Datum:** květen 2026  
**Nástroje:** Python (pandas), Power BI

---

## O projektu

Česká asociace pro vzácná onemocnění (ČAVO) sdružuje individuální členy (pacienty se vzácným onemocněním, kteří nemají pro svou diagnózu pacientskou organizaci) a pacientské organizace (zastupující jedno či více vzácných onemocnění).

Cílem projektu bylo zmapovat strukturu a vývoj členské základny a poskytnout organizaci 
přehledný datový výstup, který může sloužit jako podklad pro strategická rozhodnutí.

---

## Obsah analýzy

- Celkový počet členů a zastoupených diagnóz
- Geografické rozložení členů podle krajů
- Vývoj členství v čase (2012–2026)
- Věková struktura individuálních členů
- Nejčastější diagnózy v členské základně

---

## Struktura repozitáře
CAVO_analyza_clenu_2026/
├── data/
│   ├── CAVO_IND_clean.csv       # Anonymizovaná data individuálních členů
│   └── CAVO_ORG_clean.csv       # Anonymizovaná data členských organizací
├── notebooks/
│   └── clenove_analyza.ipynb    # Čištění dat a přiřazení krajů podle PSČ
├── dashboard/
│   └── CAVO_clenove_2026.pdf    # Power BI dashboard
└── README.md

---

## Poznámka k datům

Data byla před analýzou anonymizována – odstraněny veškeré osobní identifikátory 
(jména, kontakty, adresy). Analýza pracuje výhradně s agregovanými údaji (kraj, rok narození, diagnóza, rok vzniku členství).
Pro účely analýzy se počítalo s tím, že každá pacientská organizace zastupuje jednu diagnózu.
