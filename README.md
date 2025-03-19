### **1. Praktilise töö sooritamise käik**
**Eesmärk:**
Luua Pygame'i abil lihtne graafiline rakendus, mis kuvab ekraanil tausta, ristküliku ja pildi.

**Lühikirjeldus:**
Rakendus avab 640x480 suuruse akna, täidab selle hele-sinise taustaga ning kuvab punase ristküliku, mille peale laaditakse ja skaleeritakse pildifail "Knight.png".

**Töötasin:** Üksi

**Kas sain või andsin abi?**
- Otsisin abi veateadete lahendamiseks.
- Sain juhiseid failitee parandamiseks ja Pygame'i sündmuste käsitlemiseks.
- Jagasin oma lahendust, et aidata teistel sarnase probleemiga.

---

### **2. Esinenud probleemid ja nende lahenduskäik**

**Probleem 1: Faili "img/Knight.png" ei leitud**
- **Viga:** `FileNotFoundError: No file 'img/Knight.png' found in working directory`
- **Lahendus:** Kontrollisin, kas pildifail on õigel kohal ning kasutasin `os.path.exists()` meetodit failitee kontrollimiseks enne laadimist.

**Kasutatud promptid ja allikad:**
- `pygame image not found error` (Google otsing)
- https://www.pygame.org/docs/
- OpenAI ChatGPT

**Probleem 2: Ekraan ei uuendanud õigesti pilti**
- **Viga:** `pygame.display.flip()` ei olnud paigutatud õigesse kohta.
- **Lahendus:** Lisatud pärast `screen.blit(playerImage, player)`, et tagada pildi kuvamine ekraanil.

---

### **3. Testimine ja tulemus**

**Testimismeetodid:**
- Manuaalne testimine (programmi käivitamine ja kontrollimine, kas kõik elemendid on õigesti kuvatud).

**Kas kood töötas ootuspäraselt?**
- Jah, pärast failitee parandamist töötas kood korrektselt.

**Parandused, mida tegin:**
1. Lisa failitee kontrollimine enne pildi laadimist.
2. Liigutasin `pygame.display.flip()` õigesse kohta.

**Tulemus:**
- Programm kuvab tausta, ristküliku ja mängija pildi.
- Aken suletakse korrektselt `pygame.QUIT` sündmuse abil.

---

### **4. Eneseanalüüs**

#### **4.1. Kuidas sul läks?**

Ülesanne oli huvitav ja õpetlik. Esines mõningaid probleeme failitee ja ekraani värskendamisega, kuid need said lahendatud. Õppisin rohkem Pygame'i sündmuste käsitlemise ja failide laadimise kohta.

#### **4.2. Kas avastasid uusi Python'i tehnikaid või lähenemisi?**

- `os.path.exists()` meetodi kasutamine failide olemasolu kontrollimiseks enne nende laadimist.
- `pygame.display.flip()` tähtsus ekraani värskendamisel.
- `pygame.Rect()` abil lihtsa objekti loomine ilma eraldi klassita.

#### **4.3. Enesehinnang**
Hindan oma tööd **4**.
- [ ] 2 – Lävend on saavutamata (olulised puudused, töö jäi lõpetamata või ei vasta nõuetele)
- [ ] 3 – Lävend on nõrgalt saavutatud (töö on tehtud, kuid mitmed aspektid vajaksid parandamist)
- [x] 4 – Lävend on saavutatud (ülesanne on korrektselt täidetud ja vastab ootustele)
- [ ] 5 – Lävend on saavutatud ja ületatud (ülesanne on lahendatud suurepäraselt, lisatud lisaväärtust või ületatud ootused)

#### **4.4. Mida teeksid järgmisel korral teisiti?**
- Lisaksin rohkem kontrolli failitee käsitlemiseks, et vältida vigu, kui faili pole olemas.
- Testiksin koodi erinevate ekraanisuurustega, et veenduda selle paindlikkuses.
- Võiksin lisada ka tegeliku mänguloogika, et muuta programm interaktiivseks.

---

**Kokkuvõte:**
Ülesanne täideti edukalt. Programmi põhifunktsioonid töötavad ning sain rohkem teadmisi Pygame'i kasutamisest. Edaspidi keskenduksin rohkem veakindlusele ja paindlikumale failihaldamisele.

