# Aplicando Debounce no botão:

  Fala, pessoal! Vocês já ouviram falar do botão utilizando a técnica debounce? Este procedimento nos permite ter um comportamento confiável do botão, evitando leituras falsas e possíveis erros no projeto que está sendo desenvolvido.
                                    
<div align="center">
<h3>Figura 1: Circuito no Tinkercad</h3>	
<img width="1263" height="545" alt="Image" src="https://github.com/user-attachments/assets/a89f23be-dacd-4385-a058-538c1f86ab81" />
<h4>Fonte: Circuito autoral </h4>
</div>

O botão debounce é uma aplicação que permite maior controle no circuito, realizar várias funções dentro do código utilizando um único botão, permitindo um circuito menor com várias funcionalidades, o exemplo é o que vai ser montado e explicado neste documento. 

# Materiais Necessários:
- Protoboard (Placa de ensaio);
- 1 resistor de 1KΩ;
- 2 resistores de 330Ω;
- 1 botão;
- 1 arduino;
- 1 led rgb;
- Jumper macho-macho.

# Circuito:
Nesta parte, utilizaremos o led rgb que nos permite entender melhor a lógica e ter uma visualização melhor do funcionamento proposto para o circuito.

<div align="center">
<h3>Figura 1: Circuito no Tinkercad</h3>	
<img width="1263" height="545" alt="Image" src="https://github.com/user-attachments/assets/a89f23be-dacd-4385-a058-538c1f86ab81" />
<h4>Fonte: Circuito autoral </h4>
</div>

Para montar esse circuito, vamos começar alimentando a protoboard, para isso conectamos a fileira indicada com o símbolo positivo, ‘+’, no pino de 5 volts do arduino e a fileira com o símbolo negativo, ‘-’, no GND da placa. 

Agora podemos começar a montar o botão. Primeiro, utilizaremos um resistor de 1kΩ para conectar um dos terminais do botão na parte negativa da protoboard. Depois, com um outro fio (vermelho, no nosso caso), conectamos o outro terminal na fileira do Vcc. Por fim, conectaremos o terminal de cima, do mesmo lado do resistor, pois estamos utilizando um botão pull down no circuito, no qual só permite a passagem da corrente quando está sendo pressionado, na porta digital do Arduino (10), que trabalha com valores 0 ou 1, ou seja, ligado ou desligado, para que o circuito possa funcionar pressionando o botão.

Após realizar a montagem dos botões, iremos para a parte onde o funcionamento do botão debounce irá ser mostrado através do led RGB. A montagem deste led é simples e pode ser feita rapidamente, ao analisarmos o componente (Led RGB), pode-se perceber que o mesmo tem um terminal maior, onde iremos conectar o GND “-”. Com essa etapa finalizada, podemos prosseguir com a montagem do circuito, um ponto importante é que este led tem 3 cores diferentes, por isso o seu nome, RGB, (R - red, G - green e B - blue), como mostrado na figura do circuito, realizei a ligação com os jumpers nas suas cores correspondentes, lembrando a vocês que é necessário a utilização de resistores, neste caso, utilizei os de 330Ω. 

Bom pessoal, se realizaram todos os passos acima corretamente, o circuito já está pronto para funcionamento, o que falta neste momento é a explicação do código.
