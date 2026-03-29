# 🚀 SCLF Onboarding Gida

Tknika — Smart Collaborative Learning Factory

---

## 🌍 Hautatu hizkuntza / Selecciona idioma / Select language

- 🇪🇺 [Euskara](onboarding.eu.md)  
- 🇪🇸 [Español](onboarding.es.md)  
- 🇬🇧 [English](onboarding.en.md)  

---

## 🎯 Helburua

Dokumentu honek SCLF ekosisteman lanean nola hasi azaltzen du. Arkitektura oinarrizko hiru printzipiotan oinarritzen da:

- 👉 Ez dago monoreporik
- 👉 Ez dago azpimodulurik
- 👉 Dena modularra da

## 🧩 Sistemaren egitura

SCLF hainbat biltegi (repository) independentez osatuta dago. Bakoitzak proiektu autonomo gisa funtzionatzen du:

- `sclf-drone`
- `sclf-gripper`
- `sclf-computer-vision`
- `sclf-ikasmes`
- `sclf-xplanar`
- etab.

**Oharra:** Zure ingurunea arin mantentzeko, erabiliko dituzun moduluak soilik klonatu.

## 🖥️ Hasierako konfigurazioa (Setup)

### 1. Lan-karpeta sortu

```bash
mkdir SCLF
cd SCLF
```

### 2. Beharrezko biltegiak klonatu

```bash
git clone git@github.com:Tknika-SCLF/sclf-drone.git
git clone git@github.com:Tknika-SCLF/sclf-gripper.git
git clone git@github.com:Tknika-SCLF/sclf-computer-vision.git
```

## 🔐 Autentifikazioa (gomendatua)

Kredentzialak etengabe eskatzea saihesteko, SSH erabiltzea gomendatzen da.

Gakoa sortu:

```bash
ssh-keygen -t ed25519 -C "zure_helbide_elektronikoa"
```

Ondoren, gehitu gako publikoa zure GitHub konfigurazioan.

## 🧠 Lan-metodologia

### Git-en fluxu estandarra

Edozein ekarpen egiteko, jarraitu urrats hauek dagokion biltegiaren barruan:

1. **Biltegian sartu (repo)**
   ```bash
   cd sclf-drone
   ```
2. **Adar nagusia eguneratu eta adar berri bat sortu**
   ```bash
   git checkout main
   git pull
   git checkout -b feature/hobekuntzaren-izena
   ```
3. **Lan egin eta commit egin**
   ```bash
   git add .
   git commit -m "feat: aldaketen deskribapen argia"
   ```
4. **Aldaketak igo**
   ```bash
   git push origin feature/hobekuntzaren-izena
   ```
5. **Pull Request**
   Sortu PRa zuzenean GitHub-eko interfazean.

## ⚠️ Arau garrantzitsuak

### ✅ Egin beharrekoak (Do's)
- Erabili adarrak aldaketa bakoitzeko
- Berrikusi aldaketak script-ak exekutatu aurretik
- Mantendu biltegiak txiki eta argi

### ❌ Ez egin (Don'ts)
- Ez egin lan zuzenean `main` adarrean
- Ez erabili azpimodulurik
- Ez exekutatu koderik hura ulertu gabe

## 🧪 Segurtasuna (oso garrantzitsua)

AA (Adimen Artifiziala) laguntzarekin lan egiten baduzu:

👉 **Inoiz ez exekutatu automatikoki sortutako script-ak gainbegiratu gabe.**

**Beti:**
- Irakurri kodea
- Ulertu bere logika
- Exekutatu eskuz

## 🧰 Gomendatutako ingurunea

- **WSL:** Linux Windows barruan, bateragarritasun hobea izateko
- **VSCode / Antigravity:** lanerako ingurune nagusi gisa
- **Docker:** aukerakoa, baina gomendagarria prozesuak isolatzeko

## 📂 Meta-Workspace

Biltegi nagusi honi buruz:

- ❌ Ez da garapen-ingurune bat
- ✅ Ekosistemaren aurkibidea eta sarrera-puntua da

## 🧭 Laburpena

- Klonatu soilik beharrezkoa dena
- Lan egin modu modularrean biltegien bidez
- Erabili beti adarrak
- Berrikusi goitik behera exekutatu aurretik
