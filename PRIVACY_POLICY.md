# Integritetspolicy för Game4You

**Senast uppdaterad:** 2025-11-28

## 1. Introduktion

Välkommen till Game4You! Denna integritetspolicy förklarar hur vi samlar in, använder, delar och skyddar din information när du använder vår mobilapplikation Game4You.

Genom att använda Appen godkänner du de metoder som beskrivs i denna integritetspolicy. Om du inte godkänner denna policy, vänligen använd inte Appen.

## 2. Ansvarig för personuppgiftsbehandling

**App Utvecklare:** Emil Hakanzon  
**E-post:** hakanzon.dev@gmail.com  
**App:** Game4You

## 3. Vilken information samlar vi in?

### 3.1 Information som lagras lokalt på din enhet

Appen lagrar följande information lokalt på din enhet med hjälp av AsyncStorage:

#### 3.1.1 Personlig spelbibliotek

- Spel du har lagt till i ditt bibliotek
- Dina spelbetyg (0-10)
- Dina recensioner och kommentarer om spel
- Antal timmar spelade per spel
- Spelstatus (spelar nu, slutfört, backlog, önskelista)
- Spel du har gillat
- Anpassade listor med spel (publika eller privata)
- Datum när spel lades till och uppdaterades

#### 3.1.2 Användarinställningar

- Valda genrer för personalisering
- Valt land/region för prissökning
- Tema-inställningar (mörkt/ljust läge)
- Onboarding-status (om du har slutfört introduktionen)

#### 3.1.3 Användarstatistik

- Erfarenhetspoäng (XP)
- Användarnivå
- Spelstatistik (totalt antal spel, genomsnittligt betyg, etc.)

#### 3.1.4 Sökhistorik

- Senaste sökningar
- Sökresultat och filterinställningar

#### 3.1.5 Cachead speldata

- Trendande spel
- Nya utgåvor
- Förbeställningar
- Fan-favoriter
- Spelinformation från IGDB API

### 3.2 Automatiskt insamlad information

#### 3.2.1 Enhetsinformation

- Land/region (identifieras automatiskt från enhetens språk- och regioninställningar via `expo-localization`)
- Plattform (iOS, Android, Web)
- Enhetstyp och skärmstorlek

#### 3.2.2 Teknisk information

- App-version
- Operativsystem-version
- Fel och varningar (endast för appförbättring, lagras lokalt)

### 3.3 Information som INTE samlas in

Appen samlar **INTE** in:

- Personlig identifierbar information (namn, e-post, telefonnummer)
- Inloggningsuppgifter (autentisering är för närvarande inte implementerad)
- Platsdata (GPS)
- Kontaktinformation
- Betalningsinformation
- Biometrisk data
- Kamera- eller mikrofonåtkomst

## 4. Hur använder vi din information?

### 4.1 Lokal datalagring

All din personliga data lagras **endast lokalt** på din enhet. Vi samlar inte in eller överför din data till våra servrar. Data lagras med hjälp av:

- **AsyncStorage** - för persistent lokal lagring
- **Zustand Store** - för applikationsstate med lokal persistence

### 4.2 Användningssyften

Vi använder den insamlade informationen för att:

1. **Leverera appfunktionalitet**
   - Visa ditt personliga spelbibliotek
   - Spara dina betyg, recensioner och spelstatistik
   - Personalisera ditt innehåll baserat på dina preferenser
   - Cacha speldata för snabbare laddning och offline-användning

2. **Förbättra användarupplevelsen**
   - Kom ihåg dina inställningar och preferenser
   - Visa relevanta spelrekommendationer
   - Spara din sökhistorik för snabbare åtkomst

3. **Appförbättring**
   - Identifiera och åtgärda tekniska problem (fel loggas endast lokalt)
   - Förbättra appens prestanda och funktionalitet

## 5. Tredjepartstjänster och API:er

Appen använder följande tredjepartstjänster för att leverera funktionalitet:

### 5.1 IGDB (Internet Game Database) API

**Tjänst:** Twitch/IGDB API  
**Syfte:** Hämta spelinformation, bilder, trailers, metadata  
**Data som delas:** Endast spelnamn och söktermer (ingen personlig data)  
**Länk till integritetspolicy:** [Twitch Privacy Policy](https://www.twitch.tv/p/legal/privacy-policy/)  
**Länk till IGDB Terms:** [IGDB Terms of Service](https://www.igdb.com/terms)

**Vad som händer:**

- Appen gör API-anrop till IGDB för att hämta speldata
- Vi använder OAuth 2.0 client credentials flow (ingen användarautentisering)
- Endast spelnamn och söktermer skickas till IGDB
- Ingen personlig identifierbar information delas

### 5.2 CheapShark API

**Tjänst:** CheapShark Game Deals API  
**Syfte:** Visa spelpriser och erbjudanden från olika butiker  
**Data som delas:** Endast spelnamn för prissökning  
**Länk till integritetspolicy:** [CheapShark Privacy Policy](https://www.cheapshark.com/api/1.0)

**Vad som händer:**

- Appen söker efter spelpriser baserat på spelnamn
- Endast spelnamn skickas till CheapShark
- Ingen personlig data delas

### 5.3 Twitch Integration

**Tjänst:** Twitch  
**Syfte:** Öppna spelstreams och trailers i Twitch-appen eller webbläsaren  
**Data som delas:** Endast spelnamn för att hitta relevanta streams  
**Länk till integritetspolicy:** [Twitch Privacy Policy](https://www.twitch.tv/p/legal/privacy-policy/)

**Vad som händer:**

- Appen kan öppna Twitch-länkar för att visa spelstreams
- Detta sker via extern webbläsare eller Twitch-app
- Ingen data delas direkt från vår app

### 5.4 Expo Framework

**Tjänst:** Expo (Expo SDK)  
**Syfte:** Apputvecklingsplattform och runtime  
**Data som delas:** Teknisk appinformation (version, plattform)  
**Länk till integritetspolicy:** [Expo Privacy Policy](https://expo.dev/privacy)

**Vad som händer:**

- Expo används som utvecklingsplattform
- Vissa Expo-moduler kan samla in teknisk information för funktionalitet
- Ingen personlig data delas med Expo

### 5.5 Expo Application Services (EAS)

**Tjänst:** EAS Build  
**Syfte:** Bygga och distribuera appen  
**Data som delas:** Endast under byggprocessen  
**Länk till integritetspolicy:** [Expo Privacy Policy](https://expo.dev/privacy)

## 6. Datasäkerhet

### 6.1 Lokal säkerhet

Vi implementerar följande säkerhetsåtgärder för att skydda din data:

- **Lokal lagring:** All data lagras endast på din enhet
- **Ingen serveröverföring:** Ingen personlig data överförs till våra servrar
- **Kryptering:** Data lagras med AsyncStorage som använder plattformens säkra lagringsmekanismer
- **Ingen extern databas:** Vi använder ingen molndatabas eller extern server

### 6.2 API-säkerhet

- **OAuth 2.0:** Vi använder säkra OAuth 2.0-flöden för API-autentisering
- **HTTPS:** Alla API-anrop görs över säkra HTTPS-anslutningar
- **Rate Limiting:** Vi implementerar rate limiting för att skydda mot överanvändning
- **Token-hantering:** Access tokens hanteras säkert och förnyas automatiskt

### 6.3 Säkerhetsbegränsningar

Observera att:

- Data lagras lokalt och kan förloras om appen avinstalleras
- Vi rekommenderar regelbundna säkerhetskopior av din enhet
- Om din enhet komprometteras kan lokal data vara tillgänglig

## 7. Datadelning och överföring

### 7.1 Ingen datadelning

Vi delar **INTE** din personliga data med tredje part för marknadsföring eller annat kommersiellt syfte.

### 7.2 API-anrop

När Appen gör API-anrop till tredjepartstjänster:

- Endast nödvändig information (spelnamn) skickas
- Ingen personlig identifierbar information delas
- API-anrop görs direkt från din enhet till tredjepartstjänsten

### 7.3 Internationell dataöverföring

Eftersom vi använder tredjepartstjänster (IGDB, CheapShark) kan data överföras internationellt. Dessa tjänster kan ha servrar utanför EU/EES. Se respektive tjänsts integritetspolicy för mer information.

## 8. Dina rättigheter

Eftersom all data lagras lokalt på din enhet har du full kontroll över din data:

### 8.1 Åtkomst till din data

- All din data är tillgänglig direkt i Appen
- Du kan se all lagrad data i dina inställningar och bibliotek

### 8.2 Rätt att radera

Du kan när som helst:

- Rensa all data genom att avinstallera Appen
- Rensa specifik data via Appens inställningar (t.ex. sökhistorik)
- Radera individuella spel från ditt bibliotek

### 8.3 Rätt att korrigera

- Du kan när som helst uppdatera din data direkt i Appen
- Ändra betyg, recensioner, inställningar etc.

### 8.4 Dataportabilitet

- Data lagras lokalt på din enhet
- Du kan säkerhetskopiera din enhet för att behålla data
- För närvarande finns ingen exportfunktion, men detta kan läggas till i framtida versioner

## 9. Dataförvaring

### 9.1 Lokal lagring

- Data lagras på din enhet tills du raderar den eller avinstallerar Appen
- Cachead speldata uppdateras automatiskt och gamla data rensas
- Cache-varaktighet: 1 timme för speldata

### 9.2 Dataförlust

Observera att:

- Om du avinstallerar Appen raderas all lokal data
- Vi rekommenderar att du säkerhetskopierar din enhet regelbundet
- Vi ansvarar inte för dataförlust vid avinstallation

## 10. Barns integritet

Appen är inte specifikt riktad till barn under 13 år. Vi samlar inte medvetet in information från barn. Om du är förälder eller vårdnadshavare och upptäcker att ditt barn har lämnat personuppgifter till oss, vänligen kontakta oss.

## 11. Cookies och spårning

Appen använder **INTE** cookies eller spårningstekniker. Vi samlar inte in data för marknadsföring eller annonsering.

## 12. Ändringar i denna integritetspolicy

Vi kan uppdatera denna integritetspolicy då och då. Vi kommer att:

- Uppdatera "Senast uppdaterad"-datumet
- Meddela om betydande ändringar via Appen
- Be om ditt godkännande om ändringarna kräver det

Vi rekommenderar att du granskar denna policy regelbundet för att hålla dig informerad om hur vi skyddar din information.

## 13. GDPR och dataskyddsförordningen

### 13.1 Rättslig grund

Eftersom all data lagras lokalt på din enhet och vi inte samlar in personuppgifter på våra servrar, tillämpas GDPR begränsat. Vi behandlar endast data som du aktivt skapar i Appen.

### 13.2 Dina GDPR-rättigheter

Du har rätt till:

- **Åtkomst:** Se all din data i Appen
- **Rättelse:** Uppdatera din data när som helst
- **Radering:** Radera data genom att avinstallera Appen
- **Begränsning:** Begränsa databehandling (använd inte specifika funktioner)
- **Dataportabilitet:** Säkerhetskopiera din enhet för att behålla data
- **Invända:** Sluta använda Appen

## 14. Kaliforniens Consumer Privacy Act (CCPA)

Om du är bosatt i Kalifornien har du rätt till:

- Veta vilken personlig information som samlas in
- Veta om din personliga information säljs eller delas
- Säg nej till försäljning av personlig information (vi säljer inte data)
- Åtkomst till din personliga information
- Radering av din personliga information

## 15. Kontaktinformation

Om du har frågor eller funderingar om denna integritetspolicy eller vår behandling av din information, vänligen kontakta oss:

**App Utvecklare:** Emil Hakanzon  
**E-post:** hakanzon.dev@gmail.com  
**App:** Game4You

## 16. Tredjepartsintegritetspolicys

För mer information om hur tredjepartstjänster behandlar din information, se:

- **Twitch/IGDB:** [Twitch Privacy Policy](https://www.twitch.tv/p/legal/privacy-policy/)
- **CheapShark:** [CheapShark Privacy Policy](https://www.cheapshark.com/api/1.0)
- **Expo:** [Expo Privacy Policy](https://expo.dev/privacy)

## 17. Sammanfattning

**Viktiga punkter:**

- ✅ All data lagras lokalt på din enhet
- ✅ Ingen personlig data delas med tredje part
- ✅ Ingen server eller molndatabas används
- ✅ Du har full kontroll över din data
- ✅ Du kan radera all data genom att avinstallera Appen
- ✅ API-anrop görs endast för att hämta spelinformation (ingen personlig data)

## 18. Godkännande

Genom att använda Game4You-appen bekräftar du att du har läst, förstått och godkänt denna integritetspolicy. Om du inte godkänner denna policy, vänligen avinstallera Appen och använd den inte.

---

**Game4You** - Din personliga gaming-kompanjon, driven av världens mest omfattande speldatabas.

_Denna integritetspolicy är skriven på svenska. Vid eventuella översättningar till andra språk gäller den svenska versionen i händelse av konflikter._
