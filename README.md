# 📚 Latex ⚡

![imagem gif de um gato folheando um livro](https://i.giphy.com/media/v1.Y2lkPTc5MGI3NjExeGUwY281MXptb3h5Y2lnaXVlZmxjdHByYjBlcjZ1Mmlhd3NleXp3cyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/W8OfQ8S1PXWKY/giphy.gif)

Aqui está uma tabela de revisão sobre as principais sintaxes do Latex.


- [📚 Latex ⚡](#-latex-)
  - [🌐 Comandos simples](#-comandos-simples)
    - [Comentário, compilar, caractere de escape](#comentário-compilar-caractere-de-escape)
  - [✍️ Formatação](#️-formatação)
    - [Texto](#texto)
    - [Exemplo parágrafo](#exemplo-parágrafo)
    - [Página](#página)
  - [📋 Tabelas](#-tabelas)
    - [Exemplo de tabela](#exemplo-de-tabela)
      - [Atividade avaliativa](#atividade-avaliativa)
  - [📦 Pacotes comuns](#-pacotes-comuns)
    - [Exemplo de tabela](#exemplo-de-tabela-1)
  - [📦 Capas](#-capas)
    - [Exemplo de Capas](#exemplo-de-capas)
    
    

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
| `Quebrar linha com paragrafo`                        | `\par`                                                      |
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

``` Latex

% Exemplo para alterar cor da pagina

\definecolor{CorA}{rgb}{0.6,1,0.3}


\begin{document}

\colorbox{red}{Lorem ipsum}\textbf{ dolor sit amet, consectetur adipiscing elit. Cras vel mattis sapien. Curabitur sem magna, lacinia eu magna venenatis, ornare ultricies augue. Quisque lobortis ante ut risus faucibus ultrices. Suspendisse quis dui nisi. Pellentesque sollicitudin diam vitae turpis lacinia, id vulputate metus cursus. Donec sagittis fermentum enim, id cursus massa porttitor vel. Etiam vitae odio sit amet magna varius tincidunt a eget dolor.}

\pagecolor{CorA}

\end{document}
```


## 📋 Tabelas

### Exemplo de tabela

#### Atividade avaliativa


```Latex

% juntas as linhas
\usepackage{multirow}

% 
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

## 📦 Pacotes comuns

### Exemplo de tabela

## 📦 Capas

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
