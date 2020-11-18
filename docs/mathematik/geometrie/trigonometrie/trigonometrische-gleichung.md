<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<script type="text/javascript" src="https://jsxgraph.uni-bayreuth.de/distrib/jsxgraphcore.js"></script>
<link rel="stylesheet" type="text/css" href="https://jsxgraph.uni-bayreuth.de/distrib/jsxgraph.css" />
<link rel="stylesheet" type="text/css" href="../../../main.css" /><!-- ← relative path to custom css -->

# Trigonometrische Gleichung

## Definition
<span class="math">Eine **trigonometrische** alias **goniometrische Gleichung** ist eine Gleichung, bei der die Variable $$x$$ in Form von $$\sin(x)$$ oder $$\cos(x)$$ vorkommt.</span>

## Formeln
> **Allgemeine Sinus- und Kosinusfunktion**
> <div class="math">$$f(x)=a\cdot\sin(bx+c)+d$$</div>
> <div class="math">$$f(x)=a\cdot\cos(bx+c)+d$$</div>
> <span class="math">$$a$$ streckt oder staucht entlang der y-Achse. (Amplitude)
> <br>$$b$$ streckt oder staucht entlang der x-Achse.
> <br>$$c$$ verschiebt nach links oder rechts.
> <br>$$d$$ verschiebt nach oben oder unten.</span>

> **Periodenlänge**
> <br>Die Strecke entlang der x-Achse, bis sich die Kurve wiederholt.
> <div class="math">$$p=\frac{2\pi}{b}$$</div>

> **Wertemenge**
> <br><span class="math">Wenn $$a$$ positiv ist:</span>
> <div class="math">$$W_f=[-a+d;a+d]$$</div>
> <span class="math">Wenn $$a$$ negativ ist:</span>
> <div class="math">$$W_f=[a+d;-a+d]$$</div>

> **Nullstellen**
> <br>Sinusfunktion:
> <div class="math">$$x_k=k\cdot\pi$$</div>
> Kosinusfunktion:
> <div class="math">$$x_k=\frac{\pi}{2}+k\cdot\pi$$</div>

## Graphen
### Einfache Sinuskurve
<div id="jxgbox1" class="jxgbox" style="max-width:100%; max-height:50%; height:400px; width:400px"></div>
<span class="math">$$\overline{\rm AB}$$ ist die Periodenlänge.&nbsp;&nbsp;&nbsp;&nbsp;Funktion: $$y=\sin(x)$$</span>

### Einfache Kosinuskurve
<div id="jxgbox2" class="jxgbox" style="max-width:100%; max-height:50%; height:400px; width:400px"></div>
<span class="math">$$\overline{\rm AB}$$ ist die Periodenlänge.&nbsp;&nbsp;&nbsp;&nbsp;Funktion: $$y=\cos(x)$$</span>

## Rechnungen
### Gleichung einer Sinus- oder Kosinusfunktion ablesen
Beispielgraph:
<div id="jxgbox3" class="jxgbox" style="max-width:100%; max-height:50%; height:400px; width:400px"></div>

#### Schritte
1. <span class="math">Die **Ruhelage** (Mittellinie zwischen höchstem und tiefstem y-Wert) einzeichnen und $$d$$ ablesen.
    <br><br><div id="jxgbox4" class="jxgbox" style="max-width:100%; max-height:50%; height:400px; width:400px"></div>
    <br>$$d=\frac{\text{Max}+\text{Min}}{2}=\frac{1+(-3)}{2}=-1$$</span>
2. Den **x-Wert** des ersten **positiven Durchgangs** (nach oben) entlang der **Ruhelage** ablesen und das **Vorzeichen ändern**.
    <br><div id="jxgbox5" class="jxgbox" style="max-width:100%; max-height:50%; height:400px; width:400px"></div>
    ### Ich habe keine Ahnung, warum der Punkt hier nicht passt. Die Gleichung ist <span class="math">$$f(x)=2\sin(2x-2)-1$$</span>
    <br>$$c=-2$$</span>
3. <span class="math">Die **Parabelschablone** am ersten **positiven Durchgang** bei $$0$$ anlegen und die **Periodenlänge** $$p$$ ablesen.
    <br>$$p=\pi$$</span>
4. <span class="math">Die Formel für die Periodenlänge **nach $$b$$ umstellen** und ausrechnen.
    <br>$$p=\frac{2\pi}{b}$$
    <br>$$b=\frac{2\pi}{p}=\frac{2\pi}{\pi}=2$$</span>
5. <span class="math">Die **Amplitude** ablesen (höchster Ausschlag nach dem ersten positiven Durchgang).
    <br>Graph
    <br>$$a=\frac{\text{Max}-\text{Min}}{2}=\frac{1-(-3)}{2}=2$$</span>
### Nullstellen berechnen
1. <span class="math">Gleich $$0$$ setzen.</span>
2. <span class="math">Am Schluss z. B. folgendes machen:
    <br>$$x_0=\frac{\pi}{2}$$
    <br>$$x_k=\frac{\pi}{2}+k\cdot3\pi,k\in \mathbb{Z}$$
    <br>außerdem: $$\sin(2x)=0$$ → $$2x=k\cdot\pi,k\in \mathbb{Z}$$ → $$x=\frac{k}{2}\pi$$</span>
### Alle reellen Lösungen ermitteln
### Lösungen innerhalb eines Intervalls ermitteln
- <span class="math">Bei $$[0;\pi]$$: 0, 1, 2 einsetzen ins Ergebnis (z. B. $$\frac{k}{2}\pi=\frac{1}{2}\cdot\pi=\frac{1}{2}\pi$$), bis das Intervall zu Ende ist.</span>

<script type="text/javascript">
JXG.Options.text.useMathJax = true;

var board1 = JXG.JSXGraph.initBoard('jxgbox1', {boundingbox: [-3, 1.5, 9, -1.5], keepAspectRatio:false, registerEvents:false, axis:true, grid:false, showCopyright:false, showNavigation:false, defaultAxes: {x: {withLabel:true, label: {position:'rt', offset:[0, 10]}}, y: {withLabel:true, label: {position:'rt', offset:[10, 0]}}}});
board1.create('functiongraph', function(x) {
    return Math.sin(x);
}, {strokeColor:'green'});
var p1 = board1.create('point', [0,0]);
var p2 = board1.create('point', [2*Math.PI,0]);
board1.create('segment', [p1,p2]);

var board2 = JXG.JSXGraph.initBoard('jxgbox2', {boundingbox: [-3, 1.5, 9, -1.5], keepAspectRatio:false, registerEvents:false, axis:true, grid:false, showCopyright:false, showNavigation:false, defaultAxes: {x: {withLabel:true, label: {position:'rt', offset:[0, 10]}}, y: {withLabel:true, label: {position:'rt', offset:[10, 0]}}}});
board2.create('functiongraph', function(x) {
    return Math.cos(x);
}, {strokeColor:'green'});
var p1 = board2.create('point', [Math.PI/-2,0]);
var p2 = board2.create('point', [(Math.PI/-2)+(2*Math.PI),0]);
board2.create('segment', [p1,p2]);

var board3 = JXG.JSXGraph.initBoard('jxgbox3', {boundingbox: [-3, 3, 4, -5], keepAspectRatio:false, registerEvents:false, axis:true, grid:false, showCopyright:false, showNavigation:false, defaultAxes: {x: {withLabel:true, label: {position:'rt', offset:[0, 10]}}, y: {withLabel:true, label: {position:'rt', offset:[10, 0]}}}});
board3.create('functiongraph', function(x) {
    return 2*Math.sin(2*x-2)-1;
}, {strokeColor:'green'});

var board4 = JXG.JSXGraph.initBoard('jxgbox4', {boundingbox: [-3, 3, 4, -5], keepAspectRatio:false, registerEvents:false, axis:true, grid:false, showCopyright:false, showNavigation:false, defaultAxes: {x: {withLabel:true, label: {position:'rt', offset:[0, 10]}}, y: {withLabel:true, label: {position:'rt', offset:[10, 0]}}}});
board4.create('functiongraph', function(x) {
    return 2*Math.sin(2*x-2)-1;
}, {strokeColor:'green'});
board4.create('functiongraph', function(x) {
    return -1;
}, {withLabel:true, name:'Ruhelage', label: {position:'rt', offset:[-40, 10]}});

var board5 = JXG.JSXGraph.initBoard('jxgbox5', {boundingbox: [-3, 3, 4, -5], keepAspectRatio:false, registerEvents:false, axis:true, grid:false, showCopyright:false, showNavigation:false, defaultAxes: {x: {withLabel:true, label: {position:'rt', offset:[0, 10]}}, y: {withLabel:true, label: {position:'rt', offset:[10, 0]}}}});
board5.create('functiongraph', function(x) {
    return 2*Math.sin(2*x-2)-1;
}, {strokeColor:'green'});
board5.create('functiongraph', function(x) {
    return -1;
}, {withLabel:true, name:'Ruhelage', label: {position:'rt', offset:[-40, 10]}});
board5.create('point', [-2,-1])
</script>