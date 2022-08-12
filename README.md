# MeusProjetos
Projetos de t.i
Ola meu nome e renan e eu reproduzi um classico dos anos 70  o jogo pong, decidi recriar o jogo atraves da linguagem de programaçao java]
Codigo







Cookies
The p5.js Editor uses cookies. Some are essential to the website functionality and allow you to manage an account and preferences. Others are not essential—they are used for analytics and allow us to learn more about our community. We never sell this data or use it for advertising. You can decide which cookies you would like to allow, and learn more in our Privacy Policy.


Allow All

Allow Essential
File
Edit
Sketch
Help
English
Hello, renanrodriges23!



Auto-refresh

Misty bactrosaurus
by renanrodriges23


Sketch Files


i
nde
x
.html

p
5.collide2
d
.js

p
ont
o
.mp3

r
aquetad
a
.mp3

s
ketc
h
.js


s
tyl
e
.css

t
rilh
a
.mp3

sketch.js
Saved: 22 minutes ago
1
//variaveis da bolinha
2
let xBolinha = 300;
3
let yBolinha = 200;
4
let Diametro = 13;
5
let raio = Diametro / 2 ;
6
​
7
//velocidade da bolinha
8
let VelocidadexBolinha = 6;
9
let MovimentaçaoyBolinha = 6;
10
​
11
//variaveis da raquete 
12
let xRaquete = 5;
13
let yRaquete = 150;
14
let raqueteComprimento = 10;
15
let raqueteAltura = 90;
16
let colidiu = false;
17
​
18
//variaveis do oponente
19
let xRaqueteOponente = 585;
20
let yRaqueteOponente = 150;
21
let velocidadeYOponente;
22
let chanceDeErrar = 0;
23
​
24
//placar do jogo
25
let meusPontos = 0;
26
let pontosOponente =0;
27
​
28
//sons do jogo
29
let raquetada;
30
let ponto;
31
let trilha;
32
​
33
function preload(){
34
  trilha = loadSound("trilha.mp3");
35
  ponto = loadSound("ponto.mp3");
36
  raquetada = loadSound("raquetada.mp3");
37
}
38
​
39
    function setup() {
40
  createCanvas(600, 400);
41
      trilha.loop();
42
}
43
​
44
function draw() {
45
  background(0);
46
  mostraBolinha();
47
  movimentaBolinha();
48
  verificaColisaoBorda();
49
  mostraRaquete(xRaquete, yRaquete);
warning in line113 :Misleading line break before '+'; readers may interpret this as an expression boundary.
Current lineline 166

Console
Clear

Preview
