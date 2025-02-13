
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
En logisk funksjon kaldt P(), P kan være P(A>B) eller annen logisk funksjon
>^predikat

> [!info]  utsagn
> Et utsagn som enten er True eller False. 
> 
> 2+2 = 4 er et utsagn som er et True
>x+2 + 5 er ikke et utsagn fordi det kan være sant eller usant basert på x.
>
>Kan brukes for å filtrere basert på logikk
>^utsagn


> [!info] tautologi:
**Tautologi** er et logisk utsagn som **alltid er sant**, uansett hvilke verdier de involverte variablene har. 
>^tautologi


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
## Mengder og diskrete strukturer
#mengder-og-diskrete-strukturer 

- 01 - [mengder definisjon og operasjoner](obsidian://open?vault=Hetlesaether&file=School%2FNTNU-V25%2F%20TMA4140%20Discrete%20mathematics%2FLectures%2F01%20-%20menger%20definisjon%20og%20operasjoner.pdf)
- 02 - [set builder NZQRu kartisisk produkt (u)endelige mengder](obsidian://open?vault=Hetlesaether&file=School%2FNTNU-V25%2F%20TMA4140%20Discrete%20mathematics%2FLectures%2F02%20-%20set%20builder%20NZQRu%20kartisisk%20produkt%20(u)endelige%20mengder.pdf)

- [oving1](obsidian://open?vault=Hetlesaether&file=School%2FNTNU-V25%2F%20TMA4140%20Discrete%20mathematics%2FAssignments%2FOving1%2Foving1.pdf)

# Relasjoner og funksjoner
#relasjoner-og-funksjoner
- 03 - [Relasjoner og ordninger](obsidian://open?vault=Hetlesaether&file=School%2FNTNU-V25%2F%20TMA4140%20Discrete%20mathematics%2FLectures%2F03%20-%20Relasjoner%20og%20ordninger.pdf)
- 04 - [Ekvivalensrelasjoner og Funksjoner](obsidian://open?vault=Hetlesaether&file=School%2FNTNU-V25%2F%20TMA4140%20Discrete%20mathematics%2FLectures%2F04%20-%20Ekvivalensrelasjoner%20og%20Funksjoner.pdf)

injektiv og surjektiv


# Utsagnslogikk
#Utsagnslogikk
- 05 - [Utsagnslogikk, sannheter og logisk ekvivalens](obsidian://open?vault=Hetlesaether&file=School%2FNTNU-V25%2F%20TMA4140%20Discrete%20mathematics%2FLectures%2F05%20-%20Utsagnslogikk%2C%20sannheter%20og%20logisk%20ekvivalens.pdf)
- 06 - [Utsagnslogikk2](obsidian://open?vault=Hetlesaether&file=School%2FNTNU-V25%2F%20TMA4140%20Discrete%20mathematics%2FLectures%2F06%20-%20utsagnslogikk2.pdf)
### **Utsagnslogikk (Propositional Logic)**

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
2. **Kontradiksjon (Contradiction)**
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
6. **[Predikater](#^predikat)**: Funksjoner som uttrykker egenskaper eller relasjoner mellom objekter (f.eks. P(x)P(x)P(x) kan bety "x er et primtall").
7. **Kvantorer**:
    - **Universell kvantor** (∀x) – betyr "for alle x".
    - **Eksistensiell kvantor** (∃x) – betyr "det finnes minst én x".

	 kode-eksempel med [[#aritet]] 1:

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
8. **[Utsagn](#^utsagn)**: ∀xP()/ExP() er et utsagn
	

9. **Logiske operatorer**:
    - **∧ (og)**
    - **∨ (eller)**
    - **¬ (ikke)**
    - **⇒ (implikasjon)**
    - **⇔ (ekvivalens)**
10. **Domene (U)**: Mengden av mulige verdier variablene kan anta.

# Bevis og bevisteknikker
#bevis-og-bevisteknikker

# Rekursjon og induksjon
#rekursjon-og-induksjon