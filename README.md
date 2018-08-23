# IED_Programa-o-de-Interface_2018
Releitura da obra do artisma A. Michael Noll 


function setup() {
  createCanvas(500, 500);
}

function draw() {
background(255);
noLoop()
  for (var i = 0; i < 2000; i++) {

    var x = random(width);
    var y = random(height);
    var d = dist(x, y, width / 2, height / 2);
    var cor = color(random(0, 250), 10, 255);
    var cor2 = color(10, 255, random(0, 250));

    if (d < 200) {
      noStroke()
      rect(x, y,random(1, 8), random(1, 8));
      fill(cor);
      if (d < 50) {
        rect(x, y, random(2, 8), random(2, 8));
        fill(cor2);
      }
    }
  }
}
