## Kuvan lisääminen

```latex
 % Tekstin levyinen kuva
\includegraphics[width=\textwidth]{universe.jpg}

% Tekstin keskellä (siinä missä kirjoitettukin)
\begin{figure}[H] % tämä H tarkoittaa tekstin mukana { h | t | b | p | H}
\centering
\includegraphics[width=8cm]{Plot.png}
\caption{Kuvateksti (pakollinen)} % Raportissa tulee olla selite jokaisen kuvan/kuvion/taulukon alla
\label{img:myimg.jpg} % vaihda vastaamaan kuvaa, jolloin voit tekstissä viitata \ref{img:myimg}
\end{figure}
```

## Behind the scenes

Koska .tex tiedostot sijaitsevat `chapters`-kansiossa ja kuvat `images`-kansiossa, pitää kuviin referoida muodossa `../images/image.jpg`

*Tämä on kuitenkin jo hoidettu `main.tex`-tiedostossa* `\graphicspath{ {./images/} }`-komennolla, joten kuvat saa lisättyä kirjoittamalla niiden nimen suoraan.

[Include photos in LaTeX -  Overleaf](https://www.overleaf.com/learn/latex/Inserting_Images)