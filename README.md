
# LaTeX Game Of Life
Reimplementation of the classic **[Conway's game of life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life)** using LaTeX/Tex programming.

## Render
Using ``pdflatex``, the program will produce a *draft.pdf* file with all generations (default=100) a page for each.
Gif picture of all slide for the *glider_gun* schema :
![Alt](http://ezodev.tk/static/GameOfLife_latex.gif)


## Installation
* Download the repo thank's to the github page. Or clone the project with the git link :
```shell
git clone git@github.com:Ezotose-1/LaTeX_GameOfLife.git
```
 * Build the project using the ``src/Makefile`` :
```sh
make
```
To build the pdf, you need to have pdflatex install on your device.

## Utilisation
The program will load a board store in ``ref/*.tex`` by including the tex file.
You can create your own board and include it in the ``src/life.tex``.
By default, it will do **100 generations** : one for each page of the pdf file.
You can configure it in the ``src/life.tex`` :
```latex
% Load precise number of generations into the pdf %
\Generation{100}
```


## File architecture
```
LaTeX_GameOfLife
├── ref                // References boards
│   ├── *.tex
│   └── output         // References .pdf 
│   │   └── *.pdf
└── src                // Source code
    ├── life.tex
    └── Makefile
```


   
### License
----
Developped by Pierre B. & CPB  
Languages : LaTeX
Free to use 
*GNU General Public License v2.0*
