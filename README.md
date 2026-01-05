# OPIUM ARCHIVE - Static Preorder Site

Sito statico dark/gothic per preorder. Contatto unico: Instagram DM @opiumarchiveofficial.

## ✨ Caratteristiche
- Hero con GIF, sezioni con video/GIF di sfondo
- Galleria prodotto con varianti colore (black, white, brown)
- Form preorder con campi obbligatori: nome, email, colore, taglia (M-XXL)
- Invio via Instagram DM: copia messaggio precompilato + link DM
- Size guide modal (XXL su richiesta) e social proof counter
- FAQ + sezione Terms & Conditions
- CTA “Follow us” al posto della newsletter

## 🧭 Dove modificare
- Contatto IG: `script.js` (const igHandle) e link in footer/CTA
- Immagini prodotto: `assets/product/` e array in `script.js` + thumbs in `index.html`
- Background: `assets/images/hero.gif`, `assets/images/ec1b1dbf-434e-fa24-9f5e-f28f5b8673d6.gif`, `assets/videos/hero-video.mp4`
- Testi principali: `index.html` (hero, features, prezzo)
- FAQ/Terms: `faq.html` (ancora #terms)

## 🚀 Deploy rapido
**Netlify (consigliato)**
1) netlify.com → New site from Git o drag&drop cartella
2) Build command: none, Publish dir: root

**Vercel**: Importa repo/cartella, framework “Other”, build none, output root.

**GitHub Pages**: Settings → Pages → deploy from branch `main` root.

## 🔧 Flusso Instagram DM
- Il form copia negli appunti il messaggio ordine (nome, email, phone, colore, taglia, note, timestamp)
- Mostra il testo copiato e un bottone “APRI INSTAGRAM DM” verso `https://ig.me/m/opiumarchiveofficial?text=...`
- Se clipboard fallisce, mostra il testo da copiare manualmente

## 🎨 Personalizzazione rapida
- Colori tema: `style.css` variabili `:root`
- Prezzo/nome/feature: `index.html` blocco product-info
- Taglie: select e size guide in `index.html`
- IG handle: cambia `igHandle` in `script.js`
- Aggiungi altre foto colore: aggiorna thumbs + array `productImages` in `script.js`

## 📂 Struttura media
- `assets/product/` immagini prodotto e size chart (sizes.png)
- `assets/images/` gif e backgrounds
- `assets/videos/` video per sezioni

## 📜 Note
- Nessuna email: contatto unico via Instagram DM
- XXL misura su richiesta (nota in size guide)
- Terms link: `faq.html#terms`

## 🧪 Test rapido
1) Apri index.html localmente
2) Prova form con colore/taglia → verifica messaggio copiato e link IG
3) Clicca Terms nel footer → scroll a sezione Terms in FAQ
4) Clicca follow CTA → profilo IG

## ⚡ Stack
- HTML + CSS + JS vanilla, nessuna build/deps
