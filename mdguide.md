<!---
	Markdown guide
	Use it with pandoc to render to beautiful documents
	Author @ Ronald Mangang
--->

---
title: Title
author:
	- First Author
	- Second Author
date: \today{}
header-includes:
	- \usepackage[a4paper, portrait, margin=4cm]{geometry}
	- \usepackage{amsmath, amssymb, amsthm, amsfonts}
	- \usepackage{blindtext}

	- \hypersetup{
		colorlinks=true,
		linkcolor=blue,
		filecolor=magenta,
		urlcolor=cyan		
		}
	
	- \linespread{1.1}
	- \newtheorem{theorem}{Theorem}
	
---

\begin{abstract}
Well markdown is just plaintext. It just needs a simple editor like notepad to write a text in markdown. This document is entirely written in markdown and just rendered to PDF as you see now. This is the simplicity and profoundness of markdown! LaTeX, MS Word, HTML --- reduced to plaintext!
\end{abstract}

\tableofcontents

# Heading h1

## Heading h2

### Heading h3

\textcolor{blue}{Colorful}.

Suppose $f:\mathbb{C}\to\mathbb{C}$ is a function. Its derivate at $z_0$ is defined as:
$$ f^{\prime}(z) = \lim_{z\to z_0} \frac{f(z_0+h)-f(z_0)}{h} $$

## Lists

It's so simple to make lists. This is an ordered list.

1. Humans
2. Are
3. Crazy

This is an unordered list.

- Computers
- Are
- Sane

## Tables

This is how a table looks.



## Math

\begin{theorem}
This is a theorem.
\end{theorem}

Here is an inline math: $E=mc^2$. The following is a display math.
$$ \nabla \times \mathbf{B} = \mu_0 \mathbf{j} + \frac{1}{c^2} \frac{\partial \mathbf{E}}{\partial t} $$

If you want to number the equation, then resort to LaTeX environments. :)

\begin{equation}
(i\gamma _{\mu} \partial ^{\mu} - m)\Psi = 0
\end{equation}

Just use the usual TeX for math.


Insert image like this:
![Put some description here.](LINK)

This is a [link](https://ronaldmangang.github.io/temp).

### Code

Code is formatted like this:

```python
	import os, exit
	os.chdir(r'~/Documents/')
	if not os.listdir():
	   print('Directory is empty.')
	   sys.exit()
	print(listdir())
```



\blindtext

\begin{thebibliography}{1}
\bibitem{tmp}
This.
\end{thebibliography}

