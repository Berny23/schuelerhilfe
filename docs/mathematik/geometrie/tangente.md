<link rel="stylesheet" type="text/css" href="https://jsxgraph.uni-bayreuth.de/distrib/jsxgraph.css" />
<script type="text/javascript" src="https://jsxgraph.uni-bayreuth.de/distrib/jsxgraphcore.js"></script>

# Tangente

## Allgemein
Beispielgraph:
<div id="jxgbox" class="jxgbox" style="height:19.5em; width:28em"></div>

## Gleichung aufstellen


<script type="text/javascript">
var board = JXG.JSXGraph.initBoard('jxgbox', {boundingbox: [-5, 4, 5, -2], anchorX: 'middle', keepAspectRatio:true, registerEvents:false, axis:true, grid:false, showCopyright:false, showNavigation:false});
board.create('functiongraph', function(x) {
    return Math.pow((x + 1), 2) - 1;
});
</script>