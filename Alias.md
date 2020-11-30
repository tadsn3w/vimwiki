# Create Aliases

## Use newcommand to create the alias: 
  
    \newcommand{\set}[1]{\setlength\itemsep{#1em}} 
  
 This new command asks for parameter like \set{2}  The {#1em} code ask for the parameter
 
    \newcommand\calculator{\tikz{
		\node (c) [inner sep=0pt, draw, fill=black, anchor=south west]{\phantom{N}};
		\begin{scope}[x=(c.south east),y=(c.north west)]    \fill[white] (.1,.7) rectangle (.9,.9);    
		\foreach \x in {.1, .33, .55, .79}{    
		\foreach \y in {.1, .24, .38, .53}{    
		\fill[white] (\x,\y) rectangle +(.11,.07);}} 
		\end{scope} }}
		\def\calcicon#1{\noindent#1 \calculator\ } 
        
        It creates a little icon calculator.  To execute this new commens \calcualtor\
     
The above command requires package tikz,pgfplots
      
