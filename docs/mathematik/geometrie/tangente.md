<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<script type="text/javascript" src="https://jsxgraph.uni-bayreuth.de/distrib/jsxgraphcore.js"></script>
<link rel="stylesheet" type="text/css" href="https://jsxgraph.uni-bayreuth.de/distrib/jsxgraph.css" />
<link rel="stylesheet" type="text/css" href="../../main.css" /><!-- ← relative path to custom css -->

# Tangente

## Definition
Eine Tangente ist eine **Gerade**, die einen Funktionsgraphen **an einem Punkt berührt**.

## Formeln
> **Allgemeine Tangentengleichung**
> <div class="math">$$t(x)=f'(a)\cdot(x-a)+f(a)$$</div>

> **Allgemeine Geradengleichung**
> <div class="math">$$y=mx+t$$</div>

## Graph
<div id="jxgbox" class="jxgbox" style="max-width:100%; max-height:50%; height:400px; width:400px"></div>
<span class="math">$$f(x)=x^2$$&nbsp;&nbsp;&nbsp;&nbsp;$$t(x)=3x-2,25$$&nbsp;&nbsp;&nbsp;&nbsp;$$A(1,5/2,25)$$</span>

## Rechnungen
### Funktionsgleichung aufstellen


<script type="text/javascript">
JXG.Options.text.useMathJax = true;

var board = JXG.JSXGraph.initBoard('jxgbox', {boundingbox: [-3, 6, 2, -1], keepAspectRatio:true, registerEvents:false, axis:true, grid:false, showCopyright:false, showNavigation:false, defaultAxes: {x: {withLabel:true, label: {position:'rt', offset:[0, 10]}}, y: {withLabel:true, label: {position:'rt', offset:[10, 0]}}}});
board.create('functiongraph', function(x) {
    return Math.pow(x, 2);
}, {strokeColor:'green', withLabel:true, name:'$$G_f$$'});
board.create('functiongraph', function(x) {
    return 3*x - 2.25;
}, {strokeWidth:2, withLabel:true, name:'$$T_f$$'});
board.create('point', [1.5, 2.25], {size:4, withLabel:true, name:'$$A$$'});
</script>