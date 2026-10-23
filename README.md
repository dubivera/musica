# musica

Brani audio per [dubivera.blogspot.com](https://dubivera.blogspot.com/), pubblicati con GitHub Pages.

## Struttura

- `musica/` — i file audio (mp3, m4a, ogg, wav). Nomi senza accenti, es. `notturno-01.mp3`
- `player/` — lettore da incorporare su Blogger: playlist casuale in loop. L'elenco dei brani è in `player/tracks.js`
- `crediti.html` — autori e licenze dei brani

## Playlist nel blog (gadget HTML o vista HTML del post)

```html
<iframe src="https://dubivera.github.io/musica/player/" width="100%" height="70" style="border:0" title="Musica per leggere"></iframe>
```

Per aggiungere un brano: caricare il file in `musica/`, aggiungere una riga in `player/tracks.js` e una in `crediti.html`.

## Inserire un singolo brano su Blogger (vista HTML del post)

```html
<iframe src="https://dubivera.github.io/musica/player/?b=notturno-01.mp3&t=Notturno"
        width="100%" height="90" frameborder="0"></iframe>
```

Oppure senza player, link diretto:

```html
<audio controls src="https://dubivera.github.io/musica/musica/notturno-01.mp3"></audio>
```

Limite: 25 MB per file caricato dal browser.
