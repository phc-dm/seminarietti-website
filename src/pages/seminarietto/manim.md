---
layout: ../../layouts/Seminarietto.astro
title: "Animazioni Matematiche in Python: Manim"
description: Seminarietto di introduzione a Manim, una libreria Python per
  creare animazioni matematiche
---
# Animazioni Matematiche in Python: Manim

<img class="float-right" src="/manim-logo-sidebar.svg" alt="Logo di Manim">

Vi sarà capitato di vedere una qualche animazione di **3Blue1Brown** o di altri youtuber che trattano di **matematica divulgativa**.

Ma come vengono create? La maggior parte di queste sono realizzate grazie ad una libreria **Python** chiamata **`manim`** che permette di programmare queste animazioni.

In questo seminarietto vedremo brevemente come installare e come funziona questa libreria seguendo gli esempi della documentazione.

Seguirà una parte interattiva in cui raccoglieremo alcune idee e proveremo a creare un’animazione insieme, quindi **portatevi tante idee**!

## Dove e Quando?

Ci vediamo il  **31 Gennaio alle 18:00 in Aula 3**. Probabilmente registreremo il seminarietto, ma consigliamo fortemente di partecipare in presenza visto che sarà molto interattivo

<!-- 
Per ora è a data da destinarsi, fateci sapere se siete interessati attraverso il segue form di disponibilità:

- <https://www.when2meet.com/?23032856-6BFOp>
 -->

## Dettagli

Alcuni link utili relativi a questo seminarietto se volete già iniziare a dare un’occhiata:

* [Documentazione della versione *community* di `manim`](https://docs.manim.community/)

    Questa è la documentazione che useremo durante il seminarietto, contiene molti esempi e spiega come funziona la libreria.
* [Canale di 3Blue1Brown](https://www.youtube.com/3blue1brown)

    Lui è il creatore della versione originale di `manim`, uno youtuber che fa molti video di matematica divulgativa. Poi un gruppo di persone l'ha [forkata](https://en.wikipedia.org/wiki/Fork_(software_development)) e creato la versione *community* che è quella consigliata da usare.

Inoltre sempre 3Blue1Brown ha organizzato due eventi chiamati [Summer of Math Exposition](https://some.3b1b.co/) in cui ha indotto una competizione per creare animazioni matematiche negli scorso anni. Veramente moltissime persone hanno partecipato e la maggior parte ha usando `manim` per animare i propri video

* [Summer of Math Exposition (2021)](https://www.youtube.com/playlist?list=PLnQX-jgAF5pTkwtUuVpqS5tuWmJ-6ZM-Z)
* [Summer of Math Exposition (2022)](https://www.youtube.com/playlist?list=PLnQX-jgAF5pTZXPiD8ciEARRylD9brJXU)
* [Summer of Math Exposition (2023)](https://www.youtube.com/playlist?list=PLnQX-jgAF5pQS2GUFCsatSyZkSH7e8UM8)

Ad esempio questi sono alcuni video interessanti creati utilizzando `manim`

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/AmgkSdhK4K8?si=rsxSlAmWheebbaR5" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Materiale Post Seminarietto

Il seminarietto si è tenuto il 31 Gennaio 2023, ecco la registrazione del seminarietto

<iframe title="Registrazione del Seminarietto" frameborder="0" src="https://drive.google.com/file/d/1vmH2Je-VGIVRfKyXlnS1AEUYTPMHIE8X/preview" width="560" height="315" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

**Nota:** è la prima volta che ne registriamo uno ed il video ogni tanto lagga. L'audio invece sembra essere venuto relativamente bene, giustamente compilare animazioni con Manim e nel frattempo registrare lo schermo non vanno molto d'accordo

Per ora ancora nessuno si è cimentato nella realizzazione di un'animazione ma appena qualcuno ci prova caricheremo qua video e codice.

### Installare Manim in Aula 3 e 4

Tutte le dipendenze `apt` di manim sono già installate, per installare il pacchetto Python per il proprio utente basta eseguire

```bash
pip install manim
```

Se il comando `manim` non funziona allora probabilmente manca `~/.local/bin` nella variabile d'ambiente `PATH`, per aggiungerlo basta aggiungere la seguente riga alla fine del proprio `.bashrc` che si trova in `~/.bashrc`

```bash
export PATH="$HOME/.local/bin:$PATH"
```
