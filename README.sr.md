<a href="https://shadowstyleshop.rs/"><img src="media/cover.jpg" alt="Shadow Style Shop, naslovna strana na laptopu i telefonu" width="100%"></a>

# Shadow Style Shop

Web prodavnica majica sa printom i konfiguratorom u kom kupac postavlja svoj dizajn na prednju i zadnju stranu pre porudžbine.

**[shadowstyleshop.rs](https://shadowstyleshop.rs/)** · [Studija slučaja](https://svilenkovic.rs/radovi/shadow-style-shop) · [English](README.md)

> [!NOTE]
> Klijentski projekat. Izvorni kod pripada klijentu i čuva se u privatnom repozitorijumu. Ova stranica opisuje šta sam uradio i kako.

<table>
  <tr><td><b>Klijent</b></td><td>Shadow Style Shop</td></tr>
  <tr><td><b>Delatnost</b></td><td>Majice sa printom i DTF štampa po dizajnu kupca</td></tr>
  <tr><td><b>Lokacija</b></td><td>Srbija</td></tr>
  <tr><td><b>Vrsta</b></td><td>Web prodavnica sa konfiguratorom</td></tr>
  <tr><td><b>Moj deo posla</b></td><td>Dizajn, izrada, SEO, hosting i održavanje</td></tr>
  <tr><td><b>Tehnologije</b></td><td>PHP 8.3, SQLite, Fabric.js, PWA</td></tr>
</table>

## O projektu

Shadow Style Shop prodaje majice sa printom preko sajta, bez fizičke radnje, i štampa dizajne koje kupci sami pošalju. Katalog ima sedam kolekcija i preko sto printova, a nove vlasnik dodaje iz panela. Ono što nijedan gotov šablon nije dobro rešavao bila je porudžbina po meri: kupac ima svoju sliku i hoće da je vidi na majici pre nego što plati.

Konfigurator radi na Fabric.js platnu, a biblioteka se servira sa istog servera. Kupac pomera i skalira sliku preko mockupa majice i bira boju majice i poziciju printa, posebno za prednju i zadnju stranu. Obe strane se izvoze kao slike i šalju u jednom zahtevu, koji dobija referentni broj i upisuje se u bazu. Vlasniku stiže mejl sa oba dizajna u prilogu, pa može da odgovori ponudom i bez otvaranja panela.

## Šta sam uradio

- Popust na količinu od tri majice naviše, vidljiv u korpi dok se bira, a konačnu cenu računa server i ne gleda cenu poslatu iz pregledača
- Otpremljeni fajlovi se proveravaju po stvarnom tipu sadržaja, bez obzira na ekstenziju, i čuvaju se tamo gde ne mogu da se izvrše
- Admin panel koji se instalira kao PWA, za proizvode, kolekcije, porudžbine, zahteve iz konfiguratora i poruke
- Poruke povezane sa sandučetom prodavnice u oba smera: odgovor iz panela odlazi kao pravi mejl, a dolazna pošta se vraća u istu prepisku
- Iz svake otpremljene fotografije proizvoda nastaju JPEG, WebP i AVIF, a server šalje format koji pregledač podržava
- Čiste adrese kroz mali ruter, a preusmerenje sa .php verzija napisano tako da ne upadne u petlju sa internim preusmeravanjem servera

## Merenja

| | Performanse | Pristupačnost | Dobre prakse | SEO |
| :-- | :-: | :-: | :-: | :-: |
| Telefon | 99 | 100 | 100 | 100 |
| Desktop | 100 | 100 | 100 | 100 |

PageSpeed Insights, laboratorijsko merenje živog sajta, septembar 2026. Sigurnosna zaglavlja: 6 od 6. HTML validator: bez grešaka. axe provera pristupačnosti: bez prekršaja. Strukturisani podaci: `ClothingStore`, `Organization`.

## Snimci ekrana

<table>
  <tr>
    <td width="68%" valign="top"><img src="media/desktop.webp" alt="Shadow Style Shop, naslovna strana na ekranu širine 1440 px"></td>
    <td width="32%" valign="top"><img src="media/mobile.webp" alt="Shadow Style Shop, naslovna strana na telefonu"></td>
  </tr>
</table>

<img src="media/inner-1.webp" alt="Istaknuti printovi na naslovnoj strani">
<sub>Istaknuti printovi na naslovnoj strani</sub>

<img src="media/inner-2.webp" alt="Kolekcije sa brojem dizajna u svakoj">
<sub>Kolekcije sa brojem dizajna u svakoj</sub>

---

<sub>Izrada: [D. Svilenković](https://svilenkovic.rs).</sub>
