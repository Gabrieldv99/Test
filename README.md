</> HTML
<canvas></canvas>

window.onload = function () {
canvas = document getElementsByTagName ("canvas")[0];
ctx = canvas •getContext ("2d");
canvas. width = canvas. height = 400;
ctx.fillrect(0, 0, 400, 400);
var r = 0;
for (var a = 0; a < MAX; a++) {
points. push([Math.cos(r), Math.sin(r), 0]);
r += (Math.PI * 2) / MAX;
}
for (var a = 0; a < MAX; a++) {
points.push ([0, points[a][0], points[a][1]]);
}
for (var a = 0; a < MAX; a++) {
points.push([points[a][1], 0, points[a][0]]);
}

rus();
