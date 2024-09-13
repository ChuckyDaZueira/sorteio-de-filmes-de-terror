# sorteio-de-filmes-de-terror

function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);
}

let filmes = [

  "Hereditary (2018)", "A Bruxa (2015)", "Midsommar (2019)", "O Babadook (2014)", 

  "Corrente do Mal (2014)", "O Exorcista (1973)", "Psicose (1960)", "O Iluminado (1980)", 

  "Halloween (1978)", "Sexta-Feira 13 (1980)", "A Hora do Pesadelo (1984)", 

  "Atividade Paranormal (2007)", "Invocação do Mal (2013)", "A Entidade (2012)", 

  "Halloween (2018)", "O Massacre da Serra Elétrica (1974)", "Annabelle (2014)", 

  "Corra! (2017)", "Nós (2019)", "Host (2020)", "Sobrenatural (2010)", "A Morte do Demônio (2013)", 

  "O Chamado (2002)", "O Grito (2004)", "Jogos Mortais (2004)", "Alien: O Oitavo Passageiro (1979)", 

  "Cloverfield (2008)", "A Casa de Cera (2005)", "Doce Vingança (2010)", "O Segredo da Cabana (2012)", 

  "Silent Hill (2006)", "1408 (2007)", "A Órfã (2009)", "O Ritual (2011)", "Demônio (2010)", 

  "O Exorcismo de Emily Rose (2005)", "Carrie, A Estranha (1976)", "Olhos Famintos (2001)", 

  "It: A Coisa (2017)", "O Homem Invisível (2020)"
  
   

];

let filmeSorteado = "";

let button;

function setup() {

  createCanvas(800, 600);

  background(255, 0, 0);  // Fundo vermelho

  

  // Criar o botão

  button = createButton('Sortear Filme');

  button.position(350, 550);

  button.mousePressed(sorteio);

  // Exibir o texto inicial

  textSize(32);

  fill(255);  // Cor do texto branco

  textAlign(CENTER, CENTER);

  text(filmeSorteado, width / 2, height / 2);

}

function draw() {

  background(255, 0, 0);  // Fundo vermelho

  

  // Exibir o filme sorteado

  textSize(32);

  fill(255);  // Cor do texto branco

  textAlign(CENTER, CENTER);

  text(filmeSorteado, width / 2, height / 2);

}

function sorteio() {

  // Sortear um filme aleatório

  filmeSorteado = random(filmes);

}
