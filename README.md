# Turner România

Resursă independentă în limba română despre sindromul Turner, pentru familii, paciente și profesioniști.

A pornit dintr-un motiv simplu: când am căutat informații în românește despre sindromul Turner, nu am găsit aproape nimic. Site-ul adună, într-un singur loc și pe înțeles, ce spune literatura medicală actuală.

## Ce conține site-ul

- Ce este sindromul Turner și care sunt variantele lui genetice, toate tratate egal
- Diagnostic, cariotip, tratament cu hormon de creștere, pubertate și estrogen
- Ce presupune monitorizarea pe termen lung, pe fiecare sistem, cu un calendar de urmărire
- Ce contează la școală și în relația cu profesorii
- Viața de adult și tranziția de la medicina pediatrică
- Fertilitate
- Centre de referință din România și din rețeaua europeană Endo-ERN
- Dicționar de termeni medicali

## Sursa informațiilor

Conținutul medical se bazează pe ghidul internațional de consens:

> Gravholt CH, Andersen NH, Christin-Maitre S și colab., pentru The International Turner Syndrome Consensus Group. *Clinical practice guidelines for the care of girls and women with Turner syndrome. Proceedings from the 2023 Aarhus International Turner Syndrome Meeting.* European Journal of Endocrinology, 2024;190(6):G53–G151. doi:10.1093/ejendo/lvae050

Cifrele citate sunt intervale raportate pe populații întregi. Nu prezic evoluția unei persoane anume.

**Conținutul are scop informativ și educațional. Nu înlocuiește sfatul, diagnosticul sau tratamentul unui medic.**

## Structura tehnică

Un singur fișier, `index.html`, complet autonom: markup, CSS și JavaScript inline, fără dependențe și fără pas de build. Singura resursă externă sunt fonturile de la Google Fonts.

- Rutare pe hash, fără server: `#/sindrom`, `#/variante`, `#/diagnostic` și așa mai departe
- CSS scris de mână, cu variabile; fără framework
- Temă deschisă și întunecată, cu respectarea preferinței sistemului și comutator manual
- Responsive, mobile-first

### Cum îl rulezi local

Nu e nevoie de nimic instalat. Deschizi `index.html` direct în browser, sau, dacă preferi un server local:

```
python -m http.server 8000
```

apoi `http://localhost:8000/index.html`

### Cum se modifică

Se editează `index.html` direct. Nu se rescrie de la zero: site-ul are deja multe pagini și un ton stabilit. Reguli de bază pentru orice contribuție:

- Orice afirmație medicală are o sursă verificabilă
- Toate variantele genetice primesc același spațiu și aceeași profunzime
- Orice element interactiv are stare de hover, focus vizibil și stare activă
- Se animă doar `transform` și `opacity`
- Conținutul lat, adică tabelele, stă într-un container cu `overflow-x: auto`

## Licență

Codul: licența MIT, vezi fișierul `LICENSE`.

Conținutul editorial, adică textele despre sindromul Turner: [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.ro). Poți să-l reiei și să-l adaptezi, necomercial, cu atribuire și păstrând aceeași licență. Dacă vrei să-l folosești altfel, întreabă.

## Contribuții

Dacă găsești o greșeală medicală sau o formulare care induce în eroare, deschide un issue. E cel mai util lucru pe care îl poți face aici.
