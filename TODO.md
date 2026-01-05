# OPIUM ARCHIVE - TODO & NEXT STEPS

## ✅ IMPLEMENTATO

### SEO & Meta Tags
- Meta description, keywords
- Open Graph tags (Facebook/LinkedIn)
- Twitter Card tags
- Favicon placeholder

### UI/UX Features
- ⏰ **Countdown Timer** (14 giorni) - automatico con animazione
- 📊 **Social Proof Badge** - "47 PREORDERS PLACED" (incrementa ogni 30-60 sec)
- 📐 **Size Guide Modal** - tabella misure cliccabile
- 📧 **Newsletter Form** - footer con subscribe
- 🎨 **Loading Screen** - logo animato all'avvio
- 🎯 **Cursor Crosshair** - aesthetic gothic
- ✨ **Hover Effects** - animazioni sweep su bottoni
- 📱 **Responsive** - mobile-friendly tutto

### Form Enhancements
- ✓ Validazione email migliorata
- ✓ Check campi required
- ✓ Messaggi success/error chiari
- ✓ Timestamp nelle email
- ✓ Gestione errori robusta

### Pagine Aggiuntive
- **faq.html** - FAQ completa su ordini, spedizioni, resi, brand

---

## 🔴 DA FARE (TUO)

### 1. CONTENUTI MEDIA
```
/images/
  - product-front.jpg    (1200x1200px)
  - product-back.jpg
  - product-detail.jpg
  - product-lifestyle.jpg
  - og-image.jpg         (1200x630px per social)
  - favicon.ico          (32x32px logo)
```

### 2. EMAIL CONFIGURAZIONE
Scegli un metodo:

**Opzione A: Formspree** (CONSIGLIATO - gratis 50 form/mese)
1. Vai su https://formspree.io
2. Crea account, crea form
3. Copia Form ID
4. In `script.js` linea ~150, decomment sezione Formspree
5. Sostituisci `YOUR_FORM_ID` con il tuo

**Opzione B: EmailJS** (gratis 200 email/mese)
1. https://emailjs.com → registrati
2. Aggiungi email service (Gmail/Outlook)
3. Crea email template
4. In `index.html` aggiungi script EmailJS
5. In `script.js` linea ~175, decomment sezione EmailJS

**Opzione C: Mailchimp Newsletter**
1. https://mailchimp.com → registrati
2. Crea audience list
3. Ottieni embedded form code
4. Sostituisci newsletter form in `index.html`

### 3. GOOGLE ANALYTICS
1. Vai su https://analytics.google.com
2. Crea proprietà per sito
3. Copia ID (tipo `G-XXXXXXXXXX`)
4. In `index.html` linea ~186, decomment sezione Analytics
5. Sostituisci con il tuo ID

### 4. DEPLOY NETLIFY
- File `netlify.toml` già configurato
- Collega repo GitHub a Netlify
- Auto-deploy al push su main

### 5. OTTIMIZZAZIONI (opzionali)
- Comprimi immagini (TinyPNG)
- Aggiungi video hero (formato .mp4, 10-20MB max)
- Crea Instagram @opiumarchive
- Pixel Facebook/TikTok per retargeting

---

## 📝 MODIFICHE VELOCI

### Cambia countdown durata
`script.js` linea 11:
```javascript
countdownDate.setDate(countdownDate.getDate() + 14); // 14 giorni
```

### Cambia email contatto
Cerca e sostituisci:
- `contact@opiumarchive.com` → tua email
- In `index.html` e `faq.html`

### Cambia prezzo/nome prodotto
`index.html` linea ~50:
```html
<h3 class="product-title">OPIUM HOODIE 001</h3>
<p class="product-price">€89.00</p>
```

### Aggiungi/modifica taglie
`index.html` linea ~58 (features) e ~92 (form select)

---

## 🎨 ASSETS CONSIGLIATI

### Foto Prodotto
- Shot 1: Fronte su mannequin/modello (sfondo nero)
- Shot 2: Retro
- Shot 3: Close-up logo/dettagli
- Shot 4: Lifestyle (modello indossa)
- Formato: JPG, 1200x1200px, <500KB

### Video Hero (opzionale)
- 10-30 secondi loop
- Aesthetic Y2K/gothic
- Muto, autoplay
- MP4, <20MB
- Aggiungi in hero section:
```html
<video autoplay loop muted playsinline>
  <source src="hero-video.mp4" type="video/mp4">
</video>
```

### Social Graphics
- Instagram posts: 1080x1080px
- Stories: 1080x1920px
- Style: minimal, nero/bianco, font Space Grotesk

---

## 🚀 LAUNCH CHECKLIST

- [ ] Carica foto prodotto
- [ ] Sostituisci placeholder image
- [ ] Configura email form (Formspree/EmailJS)
- [ ] Aggiungi Google Analytics
- [ ] Testa form su mobile e desktop
- [ ] Verifica link FAQ
- [ ] Crea account social (Instagram/TikTok)
- [ ] Deploy su Netlify
- [ ] Test finale su dominio live
- [ ] Annuncio lancio su social

---

**Note**: Tutti i file sono pronti. Devi solo aggiungere contenuti visivi e configurare servizi esterni (analytics). Contatto principale: Instagram @opiumarchiveofficial.
