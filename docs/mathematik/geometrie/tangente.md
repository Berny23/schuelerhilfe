<link rel="stylesheet" type="text/css" href="https://jsxgraph.uni-bayreuth.de/distrib/jsxgraph.css" />
<script type="text/javascript" src="https://jsxgraph.uni-bayreuth.de/distrib/jsxgraphcore.js"></script>

# Tangente

## Allgemein
Beispielgraph:
<div id="jxgbox" class="jxgbox" style="max-width:100%; height:400px; width:600px"></div>

## Gleichung aufstellen


<script type="text/javascript">
var board = JXG.JSXGraph.initBoard('jxgbox', {boundingbox: [-6, 6, 6, -3], keepAspectRatio: true, zoom: {enabled: false}, pan: {enabled: false}, axis: true, grid: false, showCopyright: false, showNavigation: false});
board.create('functiongraph', function(x) {
    return Math.pow((x + 1), 2) - 1;
});
</script>