
- [Mengder og diskrete strukturer](#mengder-og-diskrete-strukturer)
- [Relasjoner og funksjoner](#relasjoner-og-funksjoner)
- [Utsagnslogikk](#utsagnslogikk)
- [Predikatlogikk](#predikatlogikk)
- [Bevis og bevisteknikker](#bevis-og-bevisteknikker)
- [Rekursjon og induksjon](#rekursjon-og-induksjon)
- [Kombinatorikk](#kombinatorikk)
- [Grafteori](#grafteori)
- [Formelle språk](#formelle-sprak)
- [Tilstandsmaskiner](#tilstandsmaskiner)
- [Anvendelser og repetisjon](#anvendelser-og-repetisjon)

#generell
Ord liste: https://matematikkradet.no/ordliste/
Definisjoner:

> [!info]  Atomære formler:
En **atomær formel** (også kalt **atomisk formel**) er den enkleste formen for en logisk formel i **predikatlogikk**. Den kan defineres som en **grunnleggende utsagnsenhet** som ikke inneholder logiske konnektiver (som ∧, ∨, →, ¬) eller kvantorer (∃, ∀).
> ^atomareformler

> [!info] pedikat :
P():
En logisk funksjon kaldt P(), condition er alminelig - som eksempel: P(a>b) eller annen logisk funksjon -> P(4,2) = True
> 
>^predikat

> [!info]  utsagn
> Et utsagn som enten er True eller False. 
> 
> 2+2 = 4 er et utsagn som er et True
>x+2 + 5 er ikke et utsagn fordi det kan være sant eller usant basert på x.
>
>Kan brukes for å filtrere basert på logikk
>^utsagn


> [!info] tautologi (⊤)):
**Tautologi** er et logisk utsagn som **alltid er sant**, uansett hvilke verdier de involverte variablene har. 
>^tautologi

> [!info] kontradiksjon (⊥)):
> **Kontradiksjon** er et logisk utsagn som aldri er sant, uansett hvilke verdier de involverte variablene har.
>^kontradiksjon

> [!info] Aritet
>
> **Aritet** (også kalt *ary*) er et begrep innen **logikk, matematikk og informatikk**  
> som beskriver **antall argumenter (eller operander)** en funksjon, relasjon eller operasjon tar inn.  
>
> | **Eksempel** | **Aritet** | **Beskrivelse** |
> |-------------|-----------|-------------------------------------|
> | P(x) | 1 (unær) | Predikat PPP tar én variabel x |
> | P(x,y) | 2 (binær) | Relasjon RRR tar to variabler (f.eks. "x > y") |
> | P(x,y,z) | 3 (ternær) | Relasjon SSS tar tre variabler |
> ^artitet


> [!info] **Domene**
>
>
>
> - **Domene**: Mulige verdier en funksjon eller relasjon kan ta.
>
> - **Univers (U)**: Største mengde av elementer vi vurderer.
>
> - **U (Universalmengden)**: Hele mengden som inneholder alle relevante elementer.
>
>
>
> **Eksempel**:
>
> Hvis \( U = \{1,2,3,4,5\} \), og funksjonen \( f(x) = x^2 \) har domenet \( \mathbb{R} \), så er \( U \) universalmengden for dette systemet.
>
>^domene

> [!info] Direkte bevis (P⇒Q)
**Definisjon:** I et direkte bevis antar man at **P** er sann, og viser at **Q** også nødvendigvis må være sann.
>
**Eksempel:**
>
>- Påstand: Hvis et tall er partall (**P**), så er det delelig med 2 (**Q**).
>- Bevis: Anta at **P** er sann, dvs. tallet er partall. Da kan vi skrive tallet som 2k, hvor k er et heltall. Siden 2k er delelig med 2, har vi vist at **Q** er sann.
> ^direktebevis


> [!info] Kontrapositivt bevis (P⇒Q⇔¬Q⇒¬P)
>**Definisjon:** Kontrapositivt bevis innebærer å vise at **¬Q** (ikke Q) fører til **¬P** (ikke P), som er ekvivalent med å vise at **P ⇒ Q**.
>
>**Eksempel:**
>
>- Påstand: Hvis et tall er delelig med 2 (**P**), så er det partall (**Q**).
>- **Bevis:** Vi viser kontrapositive: Anta at tallet **ikke er partall** (¬**Q**), det vil si at det er et oddetall. Et oddetall er ikke delelig med 2, så ¬**P** er sann. Derfor er **P** ⇒ **Q** bekreftet.
>^kontrapositivtbevis


> [!info] Motsigelsesbevis (¬P⇒⊥)
**Definisjon:** Anta at **P** er falsk (¬P), og vis at dette fører til en **motsigelse** (⊥). Dermed må **P** være sann.
>
**Eksempel:**
>
>- Påstand: Det finnes ingen minste positive reelle tall (**P**).
>- **Bevis:** Anta at det finnes et minste positivt tall (¬**P**). La dette tallet være x. Da er x/2​ også et positivt tall som er mindre enn x, dette er ikke sant. Dermed kan det ikke finnes et minste positivt tall, og **P** er sann.
> ^motsigelsesbevis

> [!info] Motbevis
**Definisjon:** Motbevis innebærer å finne et **moteksempel** som viser at påstanden er falsk.
>
**Eksempel:**
>
>- Påstand: Alle tall er partall.
>- **Bevis:** Tallet 3 er et moteksempel, da det ikke er partall. Dermed er påstanden feil.
> ^motbevis

> [!info] Inuksjonsbevis (om noen uker)
Bevis ved moteksempel/motbevis
>
**Definisjon:** Bevis ved moteksempel innebærer å finne et eksempel som viser at en påstand ikke er sann.
>
**Eksempel:**
>
>- Påstand: Alle prime tall er oddetall.
>- **Bevis:** Tallet 2 er et moteksempel, da det er et primtall og et partall. Dermed er påstanden feil.
> ^induksjonsbevis
> [!info] Ikke-Konstruktive bevis 
>
**Definisjon:** Ikke-konstruktive bevis viser at et objekt eksisterer uten nødvendigvis å gi en eksplisitt konstruksjon av objektet.
>
**Eksempel:**
>
>- Påstand: Det finnes et uendelig antall primtall.
>- **Bevis:** Anta at det er et endelig antall primtall, la dem være p1, p2, ... pn​. Konstruer tallet P = p1 * p2 * ... * pn + 1. Dette tallet er ikke delelig med noen av de kjente primtallene, så det må enten være et nytt primtall eller ha et annet primtall som faktor. Dermed finnes det et uendelig antall primtall, uten å spesifisere hvilke.

> [!info] Ekvivalensrelasjon
> En mengde som er:
>- Refleksiv
>- Antisymmetrisk
>- Transitivit
>^ekvivalensrelasjon

> [!info] Delt ordning
> En
> - Refleksivitet
> - Antisymmetri 
>Transitivitet
>^deltordning
## Mengder og diskrete strukturer
#mengder-og-diskrete-strukturer 

- 01 - [mengder definisjon og operasjoner](obsidian://open?vault=Hetlesaether&file=School%2FNTNU-V25%2F%20TMA4140%20Discrete%20mathematics%2FLectures%2F01%20-%20menger%20definisjon%20og%20operasjoner.pdf)
- 02 - [set builder NZQRu kartisisk produkt (u)endelige mengder](obsidian://open?vault=Hetlesaether&file=School%2FNTNU-V25%2F%20TMA4140%20Discrete%20mathematics%2FLectures%2F02%20-%20set%20builder%20NZQRu%20kartisisk%20produkt%20(u)endelige%20mengder.pdf)

- [oving1]()

# Relasjoner og funksjoner
#relasjoner-og-funksjoner
- 03 - [Relasjoner og ordninger](obsidian://open?vault=Hetlesaether&file=School%2FNTNU-V25%2F%20TMA4140%20Discrete%20mathematics%2FLectures%2F03%20-%20Relasjoner%20og%20ordninger.pdf)
- 04 - [Ekvivalensrelasjoner og Funksjoner](obsidian://open?vault=Hetlesaether&file=School%2FNTNU-V25%2F%20TMA4140%20Discrete%20mathematics%2FLectures%2F04%20-%20Ekvivalensrelasjoner%20og%20Funksjoner.pdf)

injektiv og surjektiv

[delvis ordning](#^delvisordning
[ekvivalensrelasjon](#^ekvivalensrelasjon)
total ordning (a,b)L(b,a)
[oving2](Assignments/Oving2/Solution.pdf)


# Utsagnslogikk
#Utsagnslogikk
- 05 - [Utsagnslogikk, sannheter og logisk ekvivalens](obsidian://open?vault=Hetlesaether&file=School%2FNTNU-V25%2F%20TMA4140%20Discrete%20mathematics%2FLectures%2F05%20-%20Utsagnslogikk%2C%20sannheter%20og%20logisk%20ekvivalens.pdf)
- 06 - [Utsagnslogikk2](obsidian://open?vault=Hetlesaether&file=School%2FNTNU-V25%2F%20TMA4140%20Discrete%20mathematics%2FLectures%2F06%20-%20utsagnslogikk2.pdf)
### **[Utsagn](#^utsagn)slogistikk(Propositional Logic)**

1. **Sannhetsverdier (Truth Values)**
    
    P∈{Sant,Usant}P \in \{ \text{Sant}, \text{Usant} \}P∈{Sant,Usant}
2. **Logiske operatorer (Logical Operators)**
    
    - Konjunksjon (AND): P∧Q
    - Disjunksjon (OR): P∨Q
    - Implikasjon (Implication): P→Q
    - Ekvivalens (Equivalence): P↔Q
    - Negasjon (Negation): ¬P
3. **Sannhetstabeller (Truth Tables)**
    
| $P$ | $Q$ | $P \lor Q$ | $P \land Q$ | $P \rightarrow Q$ |
| --- | --- | ---------- | ----------- | ----------------- |
| 1   | 1   | 1          | 1           | 1                 |
| 1   | 0   | 1          | 0           | 0                 |
| 0   | 1   | 1          | 0           | 1                 |
| 0   | 0   | 0          | 0           | 1                 |

    
1. **[Tautologi](#^tautologi) (Tautology)**

    P∨¬P(Alltid sann)
2. **[Kontradiksjon](#^kontradiksjon) (Contradiction)**
3. 
    P∧¬P(Alltid usann)
4. **Logisk ekvivalens (Logical Equivalence)**
    (P⇒Q)⇔(¬P∨Q)

# Predikatlogikk
#predikatlogikk
Predikatlogikk lar deg **iterere gjennom variabler**, **sjekke betingelser**, og **filtrere/sortere objekter** basert på logiske regler.

08 - [predikatlogikk](obsidian://open?vault=Hetlesaether&file=School%2FNTNU-V25%2F%20TMA4140%20Discrete%20mathematics%2FLectures%2F08%20-%20predikatlogikk.pdf)

### **Grunnleggende konsepter i predikatlogikk:**

5. **Individvariabler**: Symboler som representerer objekter i en mengde (f.eks. x,y,zx, y, zx,y,z).
6. **[Predikater](#^predikat)**: Funksjoner som uttrykker egenskaper eller relasjoner mellom objekter (f.eks. P(x) kan bety "x er et primtall").
7. **Kvantorer**:
    - **Universell kvantor** (∀x) – betyr "for alle x".
    - **Eksistensiell kvantor** (∃x) – betyr "det finnes minst én x".

	 kode-eksempel med [aritet](#^artitet)] 1:

	func **∀**(int[]. [U](#^domene)) {
		for (i : [U](#^domene)) {
			if (! [predikat](#^predikat)(i)) {
				return false;
			}
		}
		return true;
	}
	
	func **∃**(int[]. [U](#^domene)) {
		for (e : [U](#^domene)) {
			if ([predikat](#^predikat)(i)) {
				return true;
			}
		}
		return false;
	}
8. **[Utsagn](#^utsagn)**: ∀xP()/∃xP() er et [utsagn](#^utsagn)
	

9. **Logiske operatorer**:
    - **∧ (og)**
    - **∨ (eller)**
    - **¬ (ikke)**
    - **⇒ (implikasjon)**
    - **⇔ (ekvivalens)**
10. **Domene (U)**: Mengden av mulige verdier variablene kan anta.

# Bevis og bevisteknikker
#bevis-og-bevisteknikker

09 - [bevisteknikk 1](./Lectures/09%20-%20bevisteknikk1.pdf)
10 - [bevisteknikk 2](./Lectures/10%20-%20bevisteknikk2.pdf)

- [Beivser](#^beviser) er å verifisere at en påstand er riktig matematisk. I faget er det en det en del ulike bevis vi kommer til å bruke: 
- [Direkte bevis](#^direktebevis) (P⇒Q)
- [Kontrapositivt bevis](#^kontrapositivtbevis)P⇒Q⇔¬Q⇒¬P)
- [Motsigelsesbevis](#^motsigelsesbevis) (¬P⇒⊥)
- [Motbevis](#^motbevis) 
- [Inuksjonsbevis](^#induksjonsbevis) (coming soon)
- Bevis ved moteksempel/motbevis (finn 1 x som ikke funker)
- Ikke-Konstruktive bevis (finn 1 passende x)

# Rekursjon og induksjon
#rekursjon-og-induksjon