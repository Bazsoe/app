# Autó költségnapló – telepítés iPhone-ra

Ez egy webalkalmazás (PWA): a Főképernyőről appként indul, internet nélkül is működik.

## 1. Feltöltés ingyenes HTTPS tárhelyre
Az iPhone csak **HTTPS**-ről telepít webappot – fájlból vagy localhostról nem. Töltsd fel az `autokoltseg-pwa` mappa tartalmát (az `index.html` legyen a gyökérben) valamelyikre:
- **Netlify Drop** (app.netlify.com/drop): húzd a mappát az oldalra, és kapsz egy https címet.
- **Cloudflare Pages**: Workers & Pages → Create → Pages → Upload assets, majd tölts fel a mappát.
- **GitHub Pages**: tedd a fájlokat egy repóba, Settings → Pages → Deploy from branch; a címed `https://felhasznalo.github.io/repo/` lesz (alkönyvtárból is működik).

## 2. Hozzáadás a Főképernyőhöz
1. Nyisd meg a címet **Safariban** (nem Chrome-ban).
2. Koppints a **Megosztás** gombra (négyzet felfelé nyíllal).
3. Válaszd: **Hozzáadás a Főképernyőhöz**, majd **Hozzáadás**.
4. Az első indítást online végezd el, hogy az app letöltődjön; utána offline is megy.

## 3. Az adataid
Az adatok csak a telefonodon, az app böngészőtárolójában vannak, sehová nem kerülnek fel. A Főképernyőn lévő app és a Safari külön tárolót használ, ezért egymás adatát nem látják. Ha az iOS tárhelyet szabadít fel, vagy hetekig nem használod az appot, a böngészőadat ritkán törlődhet – ezért **mentsd rendszeresen** (Beállítások → Teljes mentés képekkel; a CSV export képeket nem tartalmaz), és őrizd meg a fájlt.

## 4. Őszintén
Ez nem App Store-os natív app: nincs értesítés, nincs automatikus felhőmentés, és az iOS böngészőtárolási szabályai érvényesek rá. Cserébe nincs fiók, nincs követés, ingyenes.

## Frissítés
Új verzió feltöltése után az app a következő indításkor (esetleg a másodikon) frissül.
