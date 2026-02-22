# CLAUDE.md - Magneticode GitHub Pages

## Azienda

- **Nome**: Magneticode
- **Sito ufficiale**: https://www.magneticode.com
- **LinkedIn**: https://www.linkedin.com/company/magneticode
- **Sede**: Roma, Italia
- **Email**: info@magneticode.com
- **Fondatore/CEO**: Emanuele Garofalo (Cloud Architect, Enterprise Architect)
- **Tagline**: "Your digital compass, navigating the technological maze with magnetic precision"

## Servizi principali

- Cloud Adoption & Governance
- DevOps & Automazione (CI/CD, IaC)
- Data Management & Analytics
- Digital Transformation (end-to-end)
- Consulenza Strategica IT
- Training & Formazione tecnologica

## Mission

Supportare i clienti lavorando in modo collaborativo per superare con efficienza e innovazione le sfide tecnologiche. Condividere la visione del cliente e trasformarla in realtà con soluzioni su misura e supporto continuo.

## Struttura del sito

Sito single-page su GitHub Pages con Jekyll. Tema scuro personalizzato (blu/cyan).

### File principali

| File | Descrizione |
|------|-------------|
| `_config.yml` | Configurazione Jekyll (title, description, URL) |
| `_layouts/default.html` | Layout base HTML con font Inter da Google Fonts |
| `index.html` | Homepage: hero, servizi, chi siamo, approccio, contatti, footer |
| `assets/css/style.css` | CSS completo, responsive, variabili custom in `:root` |
| `assets/js/main.js` | Navbar scroll, mobile menu, IntersectionObserver animations |
| `404.html` | Pagina errore 404 personalizzata |
| `Gemfile` | Dipendenze Ruby (github-pages, minima) |

### Sezioni della homepage (index.html)

1. **Navbar** (`#navbar`) - Logo + menu, fixed, trasparente → opaca on scroll
2. **Hero** (`#hero`) - Headline, sottotitolo, 2 CTA buttons
3. **Servizi** (`#servizi`) - Griglia 3 colonne di 6 service cards
4. **Chi siamo** (`#chi-siamo`) - Stats box + testo + valori
5. **Approccio** (`#approccio`) - 4 step cards (Analisi → Strategia → Implementazione → Supporto)
6. **Contatti** (`#contatti`) - Info contatto + form
7. **Footer** - Brand + link + copyright

### Design system (variabili CSS)

- Background: `#0a1628` (dark), `#060f1d` (darker), `#111d33` (cards)
- Primary: `#2563eb` → `#3b82f6`
- Accent: `#06b6d4` → `#22d3ee`
- Testo: `#e2e8f0` (body), `#94a3b8` (muted), `#f1f5f9` (heading)
- Font: Inter (Google Fonts)
- Border radius: 8px / 12px / 20px

## Note tecniche

- Il form di contatto usa un action **placeholder** Formspree (`formspree.io/f/placeholder`) — va configurato con un ID reale
- Il sito è in italiano
- Layout responsive con breakpoint a 968px, 768px, 480px
- Le animazioni usano IntersectionObserver (fade-in dal basso)
- La navbar diventa opaca con backdrop-filter on scroll (>50px)
