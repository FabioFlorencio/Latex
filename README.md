# 📋 Latex ⚡

![imagem gif de um gato folheando um livro](https://i.giphy.com/media/v1.Y2lkPTc5MGI3NjExeGUwY281MXptb3h5Y2lnaXVlZmxjdHByYjBlcjZ1Mmlhd3NleXp3cyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/W8OfQ8S1PXWKY/giphy.gif)

Aqui está uma tabela de revisão sobre as principais sintaxes do Latex.


- [📋 Latex ⚡](#-latex-)
  - [🌐 Comandos simples](#-comandos-simples)
    - [Comentário, compilar, caractere de escape](#comentário-compilar-caractere-de-escape)
  - [✍️ Formatação](#️-formatação)
    - [Texto](#texto)
  - [📋 Tabelas](#-tabelas)
    - [Exemplo de tabela](#exemplo-de-tabela)
    
    

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



## 📋 Tabelas

### Exemplo de tabela
