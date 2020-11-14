<link rel="stylesheet" type="text/css" href="https://jsxgraph.uni-bayreuth.de/distrib/jsxgraph.css" />
<script type="text/javascript" src="https://jsxgraph.uni-bayreuth.de/distrib/jsxgraphcore.js"></script>

# Tangente

## Allgemein
Beispielgraph:
<div id="jxgbox" class="jxgbox" style="width:500px; height:400px;"></div>

## Gleichung aufstellen


<script type="text/javascript">
var board = JXG.JSXGraph.initBoard('jxgbox', {boundingbox: [-4, 4, 4, -4], axis:true, grid:false, showNavigation:false});
board.create('functiongraph', function(x) {
    return Math.pow((x + 1), 2) - 1;
});
</script>