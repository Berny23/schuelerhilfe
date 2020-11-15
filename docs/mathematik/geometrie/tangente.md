<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<link rel="stylesheet" type="text/css" href="https://jsxgraph.uni-bayreuth.de/distrib/jsxgraph.css" />
<script type="text/javascript" src="https://jsxgraph.uni-bayreuth.de/distrib/jsxgraphcore.js"></script>
<style>
blockquotes {
    background: #f5f5f5;
    color: #656565;
    border-left: 8px #aaa solid;
    border-radius: 4px;
    padding: 10px 20px;
    margin: 30px 20px;
    font-size: 1.03em;
}
</style>


# Tangente

## Definition
Eine Tangente ist eine **Gerade**, die einen Funktionsgraphen **an einem Punkt berührt**.

## Formeln

> Allgemeine Tangentengleichung:
> <div class="math">$$t(x)=f'(a)\cdot(x-a)+f(a)$$</div>

> Allgemeine Geradengleichung:
> <div class="math">$$y=mx+t$$</div>

## Graph
<div id="jxgbox" class="jxgbox" style="max-width:100%; max-height:50%; height:400px; width:400px"></div>
<span class="math">$$f(x) = x^2$$</span>&nbsp;&nbsp;&nbsp;&nbsp;<span class="math">$$g(x) = 3x-2,25$$</span>

## Rechnungen
### Funktionsgleichung aufstellen


<script type="text/javascript">
JXG.Options.text.useMathJax = true;

var board = JXG.JSXGraph.initBoard('jxgbox', {boundingbox: [-3, 6, 2, -1], keepAspectRatio:true, registerEvents:false, axis:true, grid:false, showCopyright:false, showNavigation:false});
board.create('functiongraph', function(x) {
    return Math.pow(x, 2);
}, {strokeColor:'green'});
board.create('functiongraph', function(x) {
    return 3*x - 2.25;
}, {strokeColor:'red', strokeWidth:2});
board.create('point', [1.5, 2.25], {size:4});
</script>