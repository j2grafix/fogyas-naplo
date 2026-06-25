# Fogyás Napló feltöltése GitHub-ra — lépésről lépésre

Ez az útmutató teljesen kezdőknek készült. A végén lesz egy saját, ingyenes weboldalad, amit bármilyen eszközről elérsz egy linkkel — pl. `https://[felhasználóneved].github.io/fogyas-naplo/Fogyas_Naplo.html`

Nem kell programoznod, nem kell semmit telepítened a géped szépségéhez — csak egy böngésző és pár kattintás.

---

## 1. lépés — GitHub fiók létrehozása

1. Nyisd meg: **https://github.com/signup**
2. Add meg az email cízmed, válassz jelszót, majd egy felhasználónevet (ez lesz a linkedben is, pl. `sanyavbl`)
3. Igazold a fiókot az emailben kapott kóddal
4. Ha kész, bejelentkezve látod a GitHub főképernyőt

> Ha már van GitHub fiókod, ezt a lépést kihagyhatod.

---

## 2. lépés — Új "repository" (tároló) létrehozása

A "repository" (röviden "repo") egy mappa a GitHub-on, ahova a fájljaid kerülnek.

1. Jobb felül kattints a **+** gombra → **New repository**
2. **Repository name**: írj be valamit, pl. `fogyas-naplo`
3. Állítsd **Public**-ra (ez kell ahhoz, hogy a GitHub Pages ingyenesen működjön)
4. **NE** jelöld be a "Add a README file" opciót (nem kötelező, mindegy is)
5. Kattints a zöld **Create repository** gombra

---

## 3. lépés — A HTML fájl feltöltése

1. Az új, üres repo oldalán keresd meg a **"uploading an existing file"** linket (középen, a gyors útmutató szövegben), vagy felül az **Add file → Upload files** gombot
2. Húzd be (drag & drop) a `Fogyas_Naplo.html` fájlt a böngésző ablakába, amit tőlem letöltöttél
3. Görgess le, és kattints a zöld **Commit changes** gombra
4. Várj néhány másodpercet — a fájl most már fent van a GitHub-on

> Tipp: ha frissített verziót akarsz feltölteni később, ugyanitt töltheted fel újra ugyanazzal a névvel — a régit felülírja.

---

## 4. lépés — GitHub Pages bekapcsolása

Ez a lépés teszi "élővé" a fájlt, hogy egy linken elérhető legyen.

1. A repo tetején kattints a **Settings** fülre (fogaskerék ikon mellett)
2. A bal oldali menüben keresd meg a **Pages** menüpontot
3. A **"Build and deployment"** szekcióban, a **Source** legördülőnél válaszd: **Deploy from a branch**
4. Alatta a **Branch** legördülőnél válaszd: **main** (vagy `master`, ha az jelenik meg), a mappánál hagyd: **/ (root)**
5. Kattints **Save**
6. Várj 1-2 percet, majd frissítsd az oldalt (F5) — megjelenik egy zöld doboz, benne a linkkel:
   `Your site is live at https://[felhasználóneved].github.io/fogyas-naplo/`

---

## 5. lépés — A naplód elérése

A teljes link, amin a naplód megnyílik:

```
https://[felhasználóneved].github.io/fogyas-naplo/Fogyas_Naplo.html
```

(Cseréld ki a `[felhasználóneved]`-et a saját GitHub felhasználónevedre, és ha más néven mentetted a fájlt, azt is.)

**Mentsd el ezt a linket könyvjelzőbe** (Ctrl+D / Cmd+D), vagy küldd el magadnak emailben/Messengerben — ezt fogod megnyitni mindig, bármelyik gépről vagy telefonról.

---

## Fontos: hogyan működik az adatmentés ezen a verzión

A napló adatai (amiket beírsz) a böngésződ saját, helyi tárolójában (`localStorage`) mentődnek el — **böngészőnként és eszközönként külön**. Ez azt jelenti:

- Ha a Chrome-ban töltöd ki a telefonodon, és utána a laptopodon Firefox-szal nyitod meg, **nem fogja látni** a telefonos adatokat — mert azok külön böngészőkben, külön tárolóban vannak.
- A GitHub Pages-es link mindenhonnan **elérhető** lesz, de az **adatok nem szinkronizálódnak automatikusan** a különböző eszközök/böngészők között.

**Megoldás, ha több eszközről akarod ugyanazt a naplót látni:**
Az "Adatok" fülön van **Export (JSON)** és **Import (JSON)** gomb.
1. Az egyik eszközön/böngészőben exportálod a naplót (egy `.json` fájl letöltődik)
2. Átküldöd magadnak ezt a fájlt (emailben, Google Drive-on, stb.)
3. A másik eszközön/böngészőben az **Import (JSON)** gombbal betöltöd

Ezt bármikor megismételheted, ha frissíteni akarod az adatokat a másik helyen.

---

## Hogyan frissítsd később a naplót (ha én küldök egy javított verziót)

1. Nyisd meg a repódat a GitHub-on
2. Kattints rá a `Fogyas_Naplo.html` fájlra a fájllistában
3. Jobb felül kattints a ceruza ikonra, vagy egyszerűbb: menj vissza a repo főoldalára, és **Add file → Upload files**, húzd be az új fájlt — ugyanazzal a névvel felülírja a régit
4. Commit changes
5. Pár másodperc múlva a linken már az új verzió lesz

**Fontos:** ha frissíted a fájlt, a böngésződben korábban elmentett adataid **megmaradnak** (azok külön vannak tárolva a böngésződben, nem a fájlban) — kivéve, ha a böngésződ gyorsítótára (cache) miatt a régi verzió jelenik meg. Ha ez történne, nyomj egy **Ctrl+Shift+R** (kemény frissítés) a böngészőben.

---

## Gyakori kérdések

**Kell érte fizetnem?**
Nem, a GitHub Pages teljesen ingyenes publikus repóknál.

**Más is láthatja a naplómat?**
A repo "Public", de ez csak a fájlt teszi láthatóvá technikailag — gyakorlatilag csak az látja meg, akinek elküldöd a linket, és a Google sem fogja "felindexelni" egyhamar egy ilyen apró, friss oldalt. Ha teljesen biztos akarsz lenni, hogy senki más ne találja meg, a GitHub fizetős (Pro) csomagjával lehet "Private" repóból is Pages-t futtatni — de ehhez nem kell most folyamodnod, hacsak nem szeretnéd.

**Mi van, ha törlöm véletlenül a repót?**
Mindig tartsd meg a `Fogyas_Naplo.html` fájlt a saját gépeden is biztonsági másolatként, és exportáld időnként a JSON adataidat is.
