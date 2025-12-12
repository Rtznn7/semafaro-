Este projeto simula um semáforo interativo usando HTML, CSS e JavaScript puro.
A proposta é simples: permitir que o usuário alterne entre as cores do sinal de trânsito ou ative um modo automático que troca as luzes sozinho.

O foco aqui é treinar manipulação de eventos, atualização dinâmica de imagem e controle de intervalos no JavaScript.

Como funciona

A interface exibe uma imagem representando o estado atual do semáforo e quatro botões:

Vermelho

Amarelo

Verde

Automático

Cada botão altera a imagem exibida, trocando para:

vermelho.jpg

amarelo.jpg

verde.jpg

O botão Automático ativa uma troca contínua entre as três cores, com um intervalo de 1 segundo. Ao clicar novamente, o modo automático é interrompido.

O código ainda evita conflitos: ao clicar em qualquer botão manual, o modo automático é interrompido imediatamente.

 Lógica do JavaScript

A maior parte da lógica gira em torno de:

turnOn: objeto que define a ação para cada botão

changeColor(): troca cíclica de cores

setInterval / clearInterval: controle do modo automático

Eventos de clique para capturar qual botão foi pressionado

Exemplo do controle de mudança automática:

const colors = ['red', 'yellow', 'green'];
const changeColor = () => {
    const color = colors[colorIndex];
    turnOn[color]();
    nextIndex();
};


O ID do botão muda dinamicamente entre automatic e stop, garantindo que o usuário tenha controle total do processo.

 Estilo e Animação

O projeto usa um fundo animado em gradiente dinâmico, criando um efeito visual vibrante.
Outros detalhes:

Botões com brilho e animação de escala

Imagem do semáforo com efeito de drop-shadow

Layout centralizado usando Flexbox

Estética moderna e responsiva

Esse visual dá um aspecto “anime”, combinando com o tema sugerido.

 Estrutura de Arquivos
/
│ index.html
│ style.css
│ semaforo.js
│ normal.jpg
│ vermelho.jpg
│ amarelo.jpg
│ verde.jpg

Objetivo do Projeto

Esse código serve como treino para:

DOM e eventos

Manipulação de imagens e estados

Controle de fluxo

Timers (setInterval)

Estruturação modular com objetos de funções
