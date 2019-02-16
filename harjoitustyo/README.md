# Harjoitustyö 1

Ohjeita LaTeXin käyttöön työssä.

## Mikä ihmeen LaTeX?

[LaTeX](https://fi.wikipedia.org/wiki/LaTeX)

Tärkeintä on ymmärtää se, että kirjoittaessa keskittyy nimenomaan sisällön tuottamiseen, eikä dokumentin ulkoasuun. LaTeX huolehtii dokumentin ulkonäöstä ja syntaksista.

*Google auttaa aina!*

## Dokumentin rakenne

Jotta työskentely ja dokumentin jäsentäminen olisi selkeämpää, dokumentti on jaettu osiin kappaleittain. Osiin jako helpottaa myös versionhallintaa.

Dokumentin rakenne simppelisti:

- main.tex
  - styles.tex
  - changelog.tex
  - chapters/
    - johdanto.tex
    - vaatimuksetjajarjestelmankuvaus.tex
    - vaatimustenkeruusuunnitelma

## Yleisiä ohjeita

[LATEX REFERENSSI](https://www.overleaf.com/learn/latex/Main_Page)


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

- The labels consists of sequential numbers.
  - The individual entries are indicated with a black dot, a so-called bullet.
  - The text in the entries may be of any length.
- The numbers starts at 1 with every call to the enumerate environment.

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