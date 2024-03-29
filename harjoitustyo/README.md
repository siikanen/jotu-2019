# LaTeX Ohjeita

Ohjeita LaTeXin käyttöön työssä.

## Tärkeää ❗

> **Muista lisätä merkintä tekemistäsi muutoksista changelog.tex, aina kun saat jonkin homman loppuun.**
> **Päivitä myös versionumero sivun yläreunaan!**

Committeja ei ole tässä työssä koskaan liikaa. Committaa aina kun mahdollista niin muut pystyvät seuraamaan mitä tapahtuu.

❗❗ Jos jokin kohta jää kesken tai kaipaa muokkausta, **merkitse se `% TODO ` kommentilla!** ❗❗

## Mikä ihmeen LaTeX?

<details> <summary>LATEX!</summary>
<a href="https://fi.wikipedia.org/wiki/LaTeX">LaTeX</a>

<a href="https://fi.wikipedia.org/wiki/LaTeX">
<img src="https://i.pinimg.com/originals/44/24/b0/4424b015b5d60de8081f4a06abe8bcf9.jpg"
     alt="No vittu latex"
     style="margin-right: 10px; width: 100px" />
</a>

</details>

Tärkeintä on ymmärtää se, että kirjoittaessa keskittyy nimenomaan sisällön tuottamiseen, eikä dokumentin ulkoasuun. LaTeX huolehtii dokumentin ulkonäöstä ja syntaksista.

## Dokumentin rakenne

Jotta työskentely ja dokumentin jäsentäminen olisi selkeämpää, dokumentti on jaettu osiin kappaleittain. Osiin jako helpottaa myös versionhallintaa.

**Lisää sisältö aina kappaleen nimen .tex tiedoston alle. Älä lisää otsikoihin numerointi, latex hoitaa numeroinnitt.**

Dokumentin rakenne simppelisti:

- main.tex
  - styles.tex
  - changelog.tex
  - chapters/
    - johdanto.tex
    - vaatimuksetjajarjestelmankuvaus.tex
    - vaatimustenkeruusuunnitelma.tex

## Yleisiä ohjeita

[LATEX REFERENSSI](https://www.overleaf.com/learn/latex/Main_Page)

*Google auttaa aina!*

### Perus kappalejako ja otsikot

```latex
\chapter{Luvun otskko} % Kommentti

Jokaisen luvun alussa tulee olla vähintään 2 lausetta tekstiä, jossa esitellään lyhyesti, mitä luvussa käsitellään.
Koskaan tule kahta otsikkoka peräjälkeen.

\section{Alaotsikkotaso 1}

Tekstiä alaotsikon alla

\subsection{Alaotsikkotaso 2}

Tekstiä ala-alaotsikon alla

```

### Kuvan lisääminen

[Kuvan lisääminen](images/README.md)

### Taulukon lisääminen

Generoi osoitteessa [https://www.tablesgenerator.com/](https://www.tablesgenerator.com/)

*Muista lisätä `\label{}` ja `\caption{}`*

### Listat

- One entry in the list
- Another entry in the list

```latex
\begin{itemize}
  \item One entry in the list
  \item Another entry in the list
\end{itemize}
```

1. The labels consists of sequential numbers.
2. The numbers starts at 1 with every call to the enumerate environment.

```latex
\begin{enumerate}
  \item The labels consists of sequential numbers.
  \item The numbers starts at 1 with every call to the enumerate environment.
\end{enumerate}
```

1. The labels consists of sequential numbers.
    - The individual entries are indicated with a black dot, a so-called bullet.
    - The text in the entries may be of any length. 
2. The numbers starts at 1 with every call to the enumerate environment.

```latex
\begin{enumerate}
   \item The labels consists of sequential numbers.
   \begin{itemize}
     \item The individual entries are indicated with a black dot, a so-called bullet.
     \item The text in the entries may be of any length.
   \end{itemize}
   \item The numbers starts at 1 with every call to the enumerate environment.
\end{enumerate}
```
