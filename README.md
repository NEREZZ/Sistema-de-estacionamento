Sistema de Estacionamento Automatizado
Este projeto implementa um sistema de estacionamento automatizado utilizando sensores ultrassônicos, LEDs e um servo motor. O sistema monitora duas vagas de estacionamento e controla uma catraca para gerenciar o acesso, indicando o estado das vagas (ocupadas ou livres) através de LEDs.

Funcionalidades
Detecção de Vagas Livres/Ocupadas: Utiliza sensores ultrassônicos para medir a distância e determinar se as vagas estão livres ou ocupadas.
Indicação Visual: LEDs indicam o estado das vagas de estacionamento:
LED verde indica vaga livre.
LED vermelho indica vaga ocupada.
Controle de Catraca: Um servo motor controla a abertura e fechamento da catraca com base na detecção de um objeto próximo, simulando o controle de acesso ao estacionamento.
Componentes Utilizados
Arduino
Sensores Ultrassônicos: Para medir a distância até os objetos e determinar se as vagas estão ocupadas.
LEDs: Para indicar visualmente o estado das vagas.
Servo Motor: Para controlar a catraca de acesso.
Estrutura do Código
Variáveis Globais: Armazena as leituras dos sensores e a posição do servo motor.
Função readUltrasonicDistance: Lê a distância usando os sensores ultrassônicos.
Setup: Configura os pinos de entrada e saída e inicializa o servo motor.
Loop: Monitora constantemente as leituras dos sensores e controla os LEDs e o servo motor com base nessas leituras.
Como Funciona
Os sensores ultrassônicos são usados para medir a distância até os objetos nas vagas de estacionamento.
Se a distância medida for menor ou igual a 10 cm, a vaga é considerada ocupada e o LED vermelho é aceso.
Se a distância medida for maior que 10 cm, a vaga é considerada livre e o LED verde é aceso.
O servo motor controla a catraca, que abre quando um objeto é detectado a menos de 10 cm do sensor da catraca, e fecha após um breve período.
