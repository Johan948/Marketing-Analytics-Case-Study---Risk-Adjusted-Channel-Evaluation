# Studiu de Caz – Marketing Analytics  
## Evaluarea Canalelor pe Bază de Risc–Randament (fără date de conversie)

### 📌 Prezentare generală
Acest studiu de caz analizează performanța relativă a canalelor de marketing digital într-un context caracterizat de **lipsa datelor privind conversiile și veniturile**.  
Obiectivul principal este **susținerea deciziilor de alocare a bugetului în condiții de incertitudine**, prin compararea canalelor din perspectiva eficienței, stabilității și consistenței performanței.

În absența indicatorilor clasici orientați spre rezultate finale (CPA, ROAS), analiza propune un **cadru ajustat la risc**, bazat pe metrici operaționale și măsuri statistice.

---

### ❓ Problema de business
Compania X derulează campanii de advertising pe mai multe canale digitale (Search, Social, Display, Mobile, Video), însă nu dispune de date fiabile privind conversiile sau veniturile generate.

**Întrebarea-cheie:**
> Cum pot fi evaluate și comparate canalele de marketing din punct de vedere al eficienței și riscului, în absența datelor de conversie?

---

### 🧠 Metodologie
Analiza urmează o abordare structurată, orientată spre decizie:

- **Indicator proxy de eficiență:**  
  - CTR/CPC (rata de click ajustată cu costul per click)
- **Măsurarea riscului:**  
  - Coeficientul de variație (CV) aplicat asupra valorilor log-transformate ale CTR/CPC
- **Măsurarea consistenței:**  
  - Upside Frequency – proporția zilelor în care performanța unui canal depășește media mobilă globală
- **Scor compozit:**  
  - Scor **Risk–Reward normalizat**, obținut prin standardizare (z-score) și funcție sigmoid

Acest cadru permite ierarhizarea canalelor în funcție de **profilul risc–randament**, nu doar pe baza performanței medii.

---

### 📊 Rezultate principale
- **Social** prezintă cel mai favorabil profil risc–randament, datorită stabilității și consistenței ridicate.
- **Display** și **Mobile** înregistrează o eficiență medie mai ridicată, dar sunt caracterizate de volatilitate crescută, fiind potrivite pentru **scalare oportunistică**.
- **Search** are un profil defensiv, stabil, însă cu un potențial limitat de supraperformanță.
- **Video** prezintă cel mai slab raport risc–randament, fiind marcat de volatilitate ridicată și consistență scăzută.

Rezultatele confirmă faptul că **nu există un canal dominant absolut**, subliniind importanța unei abordări orientate spre managementul riscului.

---

### 📈 Output-ul analizei
- Statistici agregate la nivel de canal
- Vizualizări de tip serie de timp pentru CTR/CPC
- Analiză de volatilitate și Upside Frequency
- Clasament final al canalelor pe baza scorului Risk–Reward

---

### ⚠️ Limitări și observații
- Studiul **nu urmărește optimizarea profitabilității**.
- Rezultatele reflectă **eficiența operațională și comportamentul traficului**, nu performanța finală de business.
- Concluziile trebuie completate cu date de conversie (CPA, ROAS) și validate prin experimente (ex. A/B testing).

---

### 🛠️ Tehnologii & competențe
- Python (pandas, numpy, matplotlib, seaborn)
- Analiză statistică
- Metrici de risc și normalizare
- Marketing analytics
- Luarea deciziilor în condiții de incertitudine

---

### 📄 Raport complet
Explicațiile detaliate privind metodologia, vizualizările și concluziile sunt disponibile în raportul PDF:

👉 `Marketing-Analytics-Case-Study---Risk-Adjusted-Channel-Evaluation.pdf`

---

### 👤 Autor
**Tontici Sergiu**  
Marketing Analytics / Performance Analysis

---

### 🎯 De ce este relevant acest proiect
Acest proiect demonstrează cum pot fi obținute **insight-uri decizionale relevante**, chiar și în condiții de date incomplete — o situație frecvent întâlnită în practica reală a marketingului digital.
