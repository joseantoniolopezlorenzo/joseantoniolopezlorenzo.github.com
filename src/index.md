---
  title: Inicio
  subtitle: Página personal de José Antonio López Lorenzo (Jall Profesor)
  title-prefix: Página personal de José Antonio López Lorenzo
  description: Presentación de distintos proyectos desarrollados por mi
  keywords:
    - proyectos
    - desarrollador
    - web
    - javascript
    - php
  date: 05/11/2020
  author: Jall Profesor
  lang: 'es-ES'
  css:
    - assets/css/modesto.min.css
    - assets/css/jall.min.css
---

# Sitio en construcción {.myclass}

::: teorema

esto es un teorema [This span should appear in small caps.]{.smallcaps}
:::

:::::::::::::: {.columns}
::: {.column}
This is the content of the first column; column width should be forty percent.
:::
::: {.column}
This is the content of the second column; column width should be sixty percent.
:::
::::::::::::::

## Probando

~~~{.gnuplot im_fmt="svg" im_out="img" im_dir="assets/images/pd"}
set terminal svg \
    font "arial,10" fontscale 1.0 size 500, 350
set key inside left top vertical Right \
    noreverse enhanced autotitles box linetype -1 linewidth 1.000
set samples 400, 400
plot [-10:10] real(sin(x)**besj0(x))
~~~

~~~{.gnuplot im_fmt="svg" im_out="img" im_dir="assets/images/pd"}
set terminal svg \
    font "arial,10" fontscale 1.0 size 500, 350
set dummy u,v
set key bmargin center horizontal Right noreverse enhanced autotitles nobox
set parametric
set view 50, 30, 1, 1
set isosamples 50, 20
set hidden3d back offset 1 trianglepattern 3 undefined 1 altdiagonal bentover
set ticslevel 0
set title "Interlocking Tori"
set urange [ -3.14159 : 3.14159 ] noreverse nowriteback
set vrange [ -3.14159 : 3.14159 ] noreverse nowriteback
splot cos(u)+.5*cos(u)*cos(v),sin(u)+.5*sin(u)*cos(v),.5*sin(v) \
      with lines, 1+cos(u)+.5*cos(u)*cos(v),\
      .5*sin(v),sin(u)+.5*sin(u)*cos(v) with lines
~~~

~~~{.gnuplot im_fmt="svg"  im_out="img" im_dir="assets/images/pd"}
set terminal svg \
    font "arial,11" fontscale 1.0 size 500, 350
set border 4095 front linetype -1 linewidth 1.000
set view 130, 10, 1, 1
set samples 50, 50
set isosamples 50, 50
unset surface
set title "set pm3d scansbackward: correctly looking surface"
set pm3d implicit at s
set pm3d scansbackward
splot sin(sqrt(x**2+y**2))/sqrt(x**2+y**2)

~~~

~~~{.mermaid im_opt="-H 300" im_fmt="svg" im_out="img" im_dir="assets/images/pd"}
sequenceDiagram
    Alice ->> Bob: Hello Bob, how are you?
    Bob-->>John: How about you John?
    Bob--x Alice: I am good thanks!
    Bob-x John: I am good thanks!
    Note right of John: Bob thinks a long<br/>time, hola mundo so long<br/>that the text does<br/>not fit on a row.

    Bob-->Alice: Checking with John...
    Alice->John: Yes... John, how are you?
~~~