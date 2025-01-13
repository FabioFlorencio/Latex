# 📚 Latex ⚡

![imagem gif de um gato folheando um livro](https://i.giphy.com/media/v1.Y2lkPTc5MGI3NjExeGUwY281MXptb3h5Y2lnaXVlZmxjdHByYjBlcjZ1Mmlhd3NleXp3cyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/W8OfQ8S1PXWKY/giphy.gif)

Aqui está uma tabela de revisão sobre as principais sintaxes do Latex.


- [📚 Latex ⚡](#-latex-)
  - [🌐 Comandos simples](#-comandos-simples)
    - [Comentário, compilar, caractere de escape](#comentário-compilar-caractere-de-escape)
  - [📦 Pacotes comuns](#-pacotes-comuns)
    - [Exemplo](#exemplo)
  - [✍️ Formatação](#️-formatação)
    - [Texto](#texto)
    - [Exemplo parágrafo](#exemplo-parágrafo)
    - [Página](#página)
  - [🎨 Imagem](#-imagem)
    - [Exemplo de imagem](#exemplo-de-imagem)
  - [📋 Tabelas](#-tabelas)
    - [Exemplo de tabela](#exemplo-de-tabela)
      - [Tabela simples com grade](#tabela-simples-com-grade)
      - [Tabela simples sem grade](#tabela-simples-sem-grade)
      - [Tabela com tamanho de célula fixa](#tabela-com-tamanho-de-célula-fixa)
      - [Tabela com cor na célula](#tabela-com-cor-na-célula)
      - [Tabela elaborada](#tabela-elaborada)
      - [Tabela usando resizebox](#tabela-usando-resizebox)
      - [Atividade avaliativa](#atividade-avaliativa)
  - [📝 Cabeçalho](#-cabeçalho)
    - [Exemplo de cabeçalho](#exemplo-de-cabeçalho)
      - [Exemplo](#exemplo-1)
  - [👨‍💻 Formatação de Código de programação](#-formatação-de-código-de-programação)
    - [Exemplo de código 1](#exemplo-de-código-1)
    - [Exemplo de código 2](#exemplo-de-código-2)
    - [Exemplo de código 3](#exemplo-de-código-3)
  - [📕 Capas](#-capas)
    - [Exemplo de Capas](#exemplo-de-capas)
  - [🌐 Sites úteis](#-sites-úteis)
    
    

## 🌐 Comandos simples

### Comentário, compilar, caractere de escape

| **Descrição**         |  **Sintaxe**                                   |
|:----------------------|:-----------------------------------------------|
|`Comentário`           | `% Comentário em uma única linha`              |
|`Compilar`             | `ctrl + enter`                                 |
|`Compilar`             | `ctrl + s`                                     |
|`caractere de escape`  | `\% `                                          |

``` Latex

% Comentário em uma única linha.

\begin{comment}
    Sou um comentário.
    Sou um comentário.
    Sou um comentário.
\end{comment}
```

## 📦 Pacotes comuns

### Exemplo

## ✍️ Formatação

### Texto

| **Descrição**                                        | **Sintaxe**                                                 |
|:-----------------------------------------------------|:------------------------------------------------------------|
| `Alinhamento a esquerda`                             | `\begin{flushleft} Conteúdo a esquerda \end{flushleft}`     |
| `Alinhamento a direita`                              | `\begin{flushright} Conteúdo a direita \end{flushright}`    |
| `Alinhamento a centro`                               | `\begin{center} Conteúdo ao centro \end{center}`            |
| `Quebrar Linha sem parágrafo`                        | `\newline`                                                  |
| `Quebrar Linha sem parágrafo`                        | `\\`                                                        |
| `Determina a tabulação vertical`                     | `\vspace{1cm}`                                              |
| `Determina a tabulação horizontal`                   | `\hspace{2cm}`                                              |
| `Quebrar linha com parágrafo`                        | `\par`                                                      |
| `linha horizontal`                                   | `\hrulefill\par`                                            |


### Exemplo parágrafo

```Latex

% Usando pacote setspace

% \onehalfspacing -> espaço entre linhas
% \doublespacing -> espaço entre linhas
% \singlespacing -> espaço entre parágrafos


\usepackage{setspace}

\begin{document}

\section{Estudo de parágrafos}

\section{Estudo de parágrafos}
\singlespacing
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras vel mattis sapien. Curabitur sem magna, lacinia eu magna venenatis, ornare ultricies augue. Quisque lobortis ante ut risus faucibus ultrices. Suspendisse quis dui 
\singlespacing

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras vel mattis sapien. Curabitur sem magna, lacinia eu magna venenatis, ornare ultricies augue. Quisque lobortis ante ut risus faucibus ultrices. Suspendisse quis dui 
\section*{Título sem númeração}

% Defini o espaço entre linhas de um parágrafo especifico
% \singlespace
% \doublespace
% \onehalfspace 
\begin{doublespace}    
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras vel mattis sapien. Curabitur sem magna, lacinia eu magna venenatis, ornare ultricies augue. Quisque lobortis ante ut risus faucibus ultrices. Suspendisse quis dui 
\end{doublespace}
\section*{Título sem númeração}

\begin{spacing}{1.2}    
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras vel mattis sapien. Curabitur sem magna, lacinia eu magna venenatis, ornare ultricies augue. Quisque lobortis ante ut risus faucibus ultrices. Suspendisse quis dui nisi. Pellentesque sollicitudin diam vitae turpis lacinia, id vulputate metus cursus. Donec sagittis fermentum enim, id cursus massa porttitor vel. Etiam vitae odio sit amet magna varius tincidunt a eget dolor.
\end{spacing}

\end{document}

```

### Página

| **Descrição**                                        | **Sintaxe**                                                 |
|:-----------------------------------------------------|:------------------------------------------------------------|
| `Determina cor da página`                            | `\pagecolor{argumento}`                                     |


```Latex

% Exemplo para alterar cor da pagina

\definecolor{CorA}{rgb}{0.6,1,0.3}


\begin{document}

\colorbox{red}{Lorem ipsum}\textbf{ dolor sit amet, consectetur adipiscing elit. Cras vel mattis sapien. Curabitur sem magna, lacinia eu magna venenatis, ornare ultricies augue. Quisque lobortis ante ut risus faucibus ultrices. Suspendisse quis dui nisi. Pellentesque sollicitudin diam vitae turpis lacinia, id vulputate metus cursus. Donec sagittis fermentum enim, id cursus massa porttitor vel. Etiam vitae odio sit amet magna varius tincidunt a eget dolor.}

\pagecolor{CorA}

\end{document}
```


## 🎨 Imagem

### Exemplo de imagem


```Latex

\begin{figure}[!htb]
    \centering
    \includegraphics[width=1\linewidth]{inserir-img.png}
    \caption{Caption}
    \label{fig:enter-label}
\end{figure} 

```

## 📋 Tabelas

### Exemplo de tabela

#### Tabela simples com grade


```Latex

\begin{table}[!h]
   \centering
    \begin{tabular}{|c|c|}\hline    
         Operador & Significado\\ \hline
         + & adição\\ \hline
         - & subtração\\ \hline
         * & multiplicação\\ \hline
         / & divisão\\ \hline
         \% & resto da divisão ("mod")\\ \hline                
    \end{tabular}       
    \caption{Operadores aritméticos}    
\end{table}
```
#### Tabela simples sem grade


```Latex

\begin{table}[!h]
    \large
    \begin{flushleft}    
      \begin{tabular}{l l}      
        \hspace{1cm} 2 * 6 / 3 & \hspace{3cm} Resultado = 4\\
        \hspace{1cm} 3 + 2 * 4 & \hspace{3cm} Resultado = 11\\
        \hspace{1cm} (3 + 2) * 4 & \hspace{3cm} Resultado = 20\\
        \hspace{1cm} 60 / (3 + 2) * 4 & \hspace{3cm} Resultado = 48\\
        \hspace{1cm} 60 / ((3 + 2) * 4) & \hspace{3cm} Resultado = 3\\
      \end{tabular}
    \end{flushleft}
\end{table}
```
#### Tabela com tamanho de célula fixa


```Latex

\begin{table}[h]
    \centering
    \begin{tabular}{|p{4cm}|c|}\hline    
         Tamanho fixo contéudo &  Tamanho variável \\ \hline
         Tamanho fixo &  Tamanho variável \\ \hline         
    \end{tabular}    
\end{table}
```

#### Tabela com cor na célula


```Latex

\usepackage[table]{xcolor}

\arrayrulecolor{orange}
\setlength{\arrayrulewidth}{0.5mm}
\renewcommand\arraystretch{1.5}

\begin{table}[h]
    \centering
    \begin{tabular}{|p{4cm}|c|}\hline    
         \rowcolor{yellow}Tamanho fixo contéudo & Tamanho variável \\ \hline
         Tamanho fixo &  \cellcolor{green}Tamanho variável com cor na célula\\ \hline         
    \end{tabular}    
\end{table}
```
#### Tabela elaborada


```Latex

\usepackage{adjustbox} % ajusta tabela
\usepackage{multirow} % junta celulas

\section*{Tipos primitivos em Java}

\begin{table}[!ht]
\resizebox{0.99\linewidth}{!}{
  \begin{tabular}{|c|c|c|c|c|}\hline
    \textbf{Descrição} & \textbf{Tipo} & \textbf{Tamanho} & \textbf{Valores} & \textbf{Valor Padrão}\\ \hline
    \multirow{4}{*}{Tipos numéricos inteiros} & \textbf{byte} & 8 bits & -128 a 127 & 0\\ \cline{2-5} 
     & \textbf{short} & 16 bits & -2147483648 a 2147483647 & 0\\ \cline{2-5} 
     & \textbf{int} & 32 bits & -2147483648 a 2147483647 & 0\\ \cline{2-5} 
     & \textbf{long} & 64 bits & \begin{tabular}[c]{@{}c@{}}-9223372036854770000 a\\ 9223372036854770000\end{tabular} & 0L\\ \hline
    \multirow{2}{*}{\begin{tabular}[c]{@{}c@{}}Tipos numéricos com\\ ponto flutuante\end{tabular}} & \textbf{float} & 32 bits & -1,4024E-37 a 3,402E+38 & 00.f\\ \cline{2-5} 
     & \textbf{double} & 64 bits & -4,94E-307 a 1,79E+308 & 0.0\\ \hline
    um caractere Unicode & \textbf{char} & 16 bits & '\textbackslash{}u0000' a '\textbackslash{}uFFFF' & '\textbackslash{}u0000'\\ \hline
    valor verdade & \textbf{boolean} & 1 bit & \{false,true\} & false\\ \hline
    \end{tabular}}
\end{table}
```

#### Tabela usando resizebox
  
  
```Latex
\usepackage{adjustbox} % ajusta tabela
\usepackage{colortbl}
\newcommand{\colorir}{\cellcolor{blue}}

\begin{table}[!h]
    \centering
    \resizebox{0.98\linewidth}{!}{
    \begin{tabular}{c|c|c|c|c|c|c} \hline
         Atividade &  1$^\circ$ Semestre & 2$^\circ$ Semestre &  3$^\circ$ Semestre &  4$^\circ$ Semestre &  5$^\circ$ Semestre & 6$^\circ$ Semestre \\ \hline
         A &\colorir  &\colorir  &\colorir  &\colorir  &\colorir  &\colorir  \\ \hline
         B &\colorir  &\colorir  &\colorir  &          &          & \\ \hline
         C &          &          &\colorir  &\colorir  &\colorir  &\colorir  \\ \hline
         D &          &          &\colorir  &\colorir  &\colorir  &\colorir  \\ \hline
         E &          &          &          &\colorir  &\colorir  &\colorir  \\ \hline
         F &          &          &          &          &\colorir  &\colorir  \\ \hline
         G &          &          &          &\colorir  &\colorir  &\colorir  \\ \hline
         H &          &          &          &          &          &\colorir  \\ \hline
          
    \end{tabular}}
    \caption{Cronograma de atividades}
    \label{tab:cronograma}
\end{table}
```

#### Atividade avaliativa


```Latex

% juntas as linhas
\usepackage{multirow}

\begin{table}[h!]    
\hrulefill\par
    \Large
    \begin{tabular}{r  c  l}
        \multirow{5}*{\includegraphics[scale= 0.5]{arquivo.png}}
        \hspace{3cm} & \textbf{Atividade Avaliativa}\\
        \hspace{3cm} & Curso: Desenv. de software multiplataforma\\
        \hspace{3cm} & Disciplina: Mobile I\\
        \hspace{3cm} & Professor: X\\
        \hspace{3cm} & Data: 24/12/2024\\
    \end{tabular}\par  
\hrulefill\\
\vspace{0.3cm}Aluno: \hspace{10cm} Nota:
\hline

\end{table}

```
## 📝 Cabeçalho

### Exemplo de cabeçalho

#### Exemplo


```Latex

\documentclass[a4paper ,12pt]{article}
\usepackage[utf8]{inputenc}
\usepackage[brazil]{babel}
\usepackage{fancyhdr}
\usepackage{graphicx,color} % Required for inserting images
\usepackage[headsep=0.9cm, top= 3cm, bottom= 3cm, right= 2cm, left= 3cm]{geometry}

\pagestyle{fancy}
\fancyhf{Técnicas de Programação II}
\lhead{\includegraphics[scale=0.2]{fatec_ra_metropolitana_sp_capital_zona_leste_cor.png}}
\rhead{Padrões de projeto}
\rfoot{Página\thepage}
\lfoot{Dia \today}

\begin{document}
\section{Introdução}
    \subsection{Apresentação}
    \subsection{Quem sou?}
    \subsection{O que faço}
\section{Desenvolvimento}    
    \subsection{Coleta de dados}
        \subsubsection{Métodos}
\section{Conclusão}    

\newpage
\section{Teste}

\end{document}

```


## 👨‍💻 Formatação de Código de programação 

### Exemplo de código 1

```Latex

% pacote para formatar código
\usepackage{listings}

\begin{document}

\begin{lstlisting}

def soma(*args):
    total = 0 
    for i,numero in enumerate(args):
        print(i,numero)            

soma(2,4,6,7,8,3)        
\end{lstlisting}

\end{document}
```

### Exemplo de código 2

```Latex

\usepackage{listings}
\usepackage{xcolor}

%cria novas cores
\definecolor{codegreen}{rgb}{0, 0.6, 0}
\definecolor{codegray}{rgb}{0.5, 0.5, 0.5}
\definecolor{codepurple}{rgb}{0.8, 0, 0.2}
\definecolor{backcolour}{rgb}{.95, .95, 1}

\lstdefinestyle{mystyle}{
  backgroundcolor=\color{backcolour},
    commentstyle=\color{codegreen},
    keywordstyle=\color{blue},
    stringstyle=\color{codepurple},
    basicstyle=\ttfamily\footnotesize,
    breakatwhitespace=false,
    breaklines=true,
    captionpos=b,
    keepspaces=true,
    numbers=left,
    numbersep=5pt,
    showspaces=false,
    showstringspaces=false,
    showtabs=false,
    tabsize=2,
    literate = {á}{{\'a}}1  {é}{{\'e}}1  {í}{{\'i}}1 {ó}{{\'o}}1  {ú}{{\'u}}1
		{Á}{{\'A}}1  {É}{{\'E}}1  {Í}{{\'I}}1 {Ó}{{\'O}}1  {Ú}{{\'U}}1
		{à}{{\`a}}1  {è}{{\`e}}1  {ì}{{\`i}}1 {ò}{{\`o}}1  {ù}{{\`u}}1
		{À}{{\`A}}1  {È}{{\'E}}1  {Ì}{{\`I}}1 {Ò}{{\`O}}1  {Ù}{{\`U}}1
		{ä}{{\"a}}1  {ë}{{\"e}}1  {ï}{{\"i}}1 {ö}{{\"o}}1  {ü}{{\"u}}1
		{Ä}{{\"A}}1  {Ë}{{\"E}}1  {Ï}{{\"I}}1 {Ö}{{\"O}}1  {Ü}{{\"U}}1
		{â}{{\^a}}1  {ê}{{\^e}}1  {î}{{\^i}}1 {ô}{{\^o}}1  {û}{{\^u}}1
		{Â}{{\^A}}1  {Ê}{{\^E}}1  {Î}{{\^I}}1 {Ô}{{\^O}}1  {Û}{{\^U}}1
		{œ}{{\oe}}1  {Œ}{{\OE}}1  {æ}{{\ae}}1 {Æ}{{\AE}}1  {ß}{{\ss}}1
		{ç}{{\c c}}1 {Ç}{{\c C}}1 {ø}{{\o}}1  {Ø}{{\O}}1   {å}{{\r a}}1
		{Å}{{\r A}}1 {ã}{{\~a}}1  {õ}{{\~o}}1 {Ã}{{\~A}}1  {Õ}{{\~O}}1
		{ñ}{{\~n}}1  {Ñ}{{\~N}}1  {¿}{{?`}}1  {¡}{{!`}}1
		{°}{{\textdegree}}1 {º}{{\textordmasculine}}1 {ª}{{\textordfeminine}}1  
}


\lstset{style=mystyle}

\begin{document}

\begin{lstlisting}[language=Python, caption=Exemplo de Listing]

def reajustar_salario(sal_ant):
    
    PERC_20 = 20
    PERC_15 = 15
    PERC_10 = 10
    PERC_5 = 5
    
    if sal_ant <= 280:
        perc_aumento = PERC_20
    elif sal_ant <= 700:
        perc_aumento = PERC_15
    elif sal_ant <= 1500:
        perc_aumento = PERC_10
    else:
        perc_aumento = PERC_5

    valor_aumento = (sal_ant / 100) * perc_aumento
    sal_atual = sal_ant + valor_aumento

    return sal_ant, sal_atual, perc_aumento, valor_aumento

# A função retorna uma tupla com os valores
result = reajustar_salario(2800)
msg = 'Salário antigo: R${:.2f} | Salário atual: R${:.2f} | percentual: {}% | valor do aumento:R${:.2f}'

print(msg.format(*result))


\end{lstlisting}

\end{document}
```

### Exemplo de código 3

  
```Latex
\usepackage{tcolorbox}
\usepackage{listings}

\begin{document}

\begin{tcolorbox}[colback=green!5!white, colframe=green!75!black, title=Código Exemplo]
\begin{lstlisting}[language=Python]
def hello():
    print("Hello, world!")
\end{lstlisting}
\end{tcolorbox}

\end{document}

```

## 📕 Capas

### Exemplo de Capas

```Latex

\begin{titlepage}
    
    \begin{center}
        {\LARGE \textbf{Fatec Zona Leste}}
        
        \vspace{5cm}
    
        Relatório Final\\
        Trabalho de conclusão de curso\\
    
        \vspace{5cm}
        {\Large \textbf{Como criar um trabalho no Latex}}
        
        \vspace{6cm}
        \hspace{5cm}Autor: \textbf{Fábio}\\
        
        \hspace{5cm}Orientador: \textbf{Prof. X}\\
        \vspace{2cm}
    
        São Paulo, Dezembro de 2024
    \end{center}
\end{titlepage}

\newpage

\renewcommand{\contentsname}{Índice}
\tableofcontents 

\newpage

\section{Introdução}
\section{Desenvolvimento}
\section{Conclusão}

%add conteúdo em tableofcontents
\addcontentsline{toc}{section}{Anexo}

\section*{Anexo}

```


## 🌐 Sites úteis


| **Descrição**                                      | **Links**                                                             |
|:---------------------------------------------------|:----------------------------------------------------------------------|
| `Ferramenta para encontrar símbolos específicos`   | [detexify](https://detexify.kirelabs.org/classify.html)               |
| `Ferramenta para gerar tabela`                     | [tables generator](https://www.tablesgenerator.com/)                  |