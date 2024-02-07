# Sito per i Seminarietti

Piccolo sito in [Astro](https://astro.build/) (sono partito dal template `minimal`) per i seminarietti del PHC.

Per aggiungere un seminarietto, basta aggiungere un file in markdown in `src/pages/seminarietto/`. 

## Struttura del progetto

Questa è la struttura del progetto, con i file più importanti:

```
├── public/
│   ├── favicon.png             # Icona del sito
│   └── manim-logo-sidebar.svg  # Altri file degli articoli
├── src/
│   ├── layouts/
│   │   ├── Page.astro          # Layout pagina generica
│   │   ├── Homepage.astro      # Layout della homepage
│   │   └── Seminarietto.astro  # Layout pagina seminarietto
│   ├── pages/
│   │   ├── seminarietto/       # Un markdown per ogni seminarietto
│   │   │   └── manim.md
│   │   └── index.md            # Homepage del sito in markdown
│   ├── content/
│   │   └── contacts.md         # Frammento per i contatti (riutilizzato in più punti)
│   └── styles.scss             # Stili globali, tipografia del sito
├── README.md                   # Questo file
└── _redirects                  # Redirects per Netlify (per short link dei QRCode)
```

## Development

```bash
$ npm install
$ npm run dev
```

## Deployment

Usare il segue comando per generare i file statici in `out/`

```bash
$ npm run build
```

Questo non serve farlo mai perché il sito è hostato su Netlify e si aggiorna automaticamente quando si fa push su `main`.
