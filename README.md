# Alura MIDI 🥁

Projeto de estudo desenvolvido durante o curso de JavaScript da [Alura](https://www.alura.com.br/), que simula um mini teclado/bateria eletrônica no navegador. Cada tecla, ao ser clicada, reproduz um som diferente.

## 🎯 Sobre o projeto

O **Alura MIDI** é uma interface simples com 9 teclas (botões), cada uma associada a um som de percussão. O projeto trabalha conceitos fundamentais de JavaScript, como:

- Manipulação do DOM (`querySelector`, `querySelectorAll`)
- Estruturas de repetição (`while`) para configurar todas as teclas dinamicamente
- Manipulação de eventos (`onclick`)
- Reprodução de áudio via elemento `<audio>`
- Template strings para montar seletores de forma dinâmica

## 🎹 Teclas disponíveis

| Tecla   | Som   |
|---------|-------|
| Pom     | keyq  |
| Clap    | keyw  |
| Tim     | keye  |
| Puff    | keya  |
| Splash  | keys  |
| Toim    | keyd  |
| Psh     | keyz  |
| Tic     | keyx  |
| Tom     | keyc  |

## 🛠️ Tecnologias utilizadas

- **HTML5** – estrutura da página e elementos de áudio
- **CSS3** – estilização do teclado
- **JavaScript** – lógica de interação e reprodução dos sons

## 📁 Estrutura do projeto

```
midi/
├── css/
│   ├── reset.css
│   └── estilos.css
├── images/
│   └── bateria.png
├── sounds/
│   ├── keyq.wav
│   ├── keyw.wav
│   ├── keye.wav
│   ├── keya.wav
│   ├── keys.wav
│   ├── keyd.wav
│   ├── keyz.wav
│   ├── keyx.wav
│   └── keyc.wav
├── index.html
└── index.js
```

## ▶️ Como executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/Juniklx/midi.git
   ```
2. Entre na pasta do projeto:
   ```bash
   cd midi
   ```
3. Abra o arquivo `index.html` no navegador (ou utilize a extensão **Live Server** do VS Code para ter recarregamento automático).

## 🔊 Como funciona

Cada tecla possui duas classes CSS: uma genérica (`tecla`) e outra específica do instrumento (ex: `tecla_pom`). O script percorre todas as teclas usando um laço `while`, monta dinamicamente o id do elemento de áudio correspondente e associa um evento de clique que dispara a reprodução do som:

```javascript
function tocaSom(idElementoAudio) {
    document.querySelector(idElementoAudio).play();
}

const listaDeTeclas = document.querySelectorAll('.tecla');
let contador = 0;

while (contador < listaDeTeclas.length) {
    const tecla = listaDeTeclas[contador];
    const instrumento = tecla.classList[1];
    const idAudio = `#som_${instrumento}`;

    tecla.onclick = function () {
        tocaSom(idAudio);
    };

    contador++;
}
```

## 📚 Aprendizados

Este projeto foi construído com fins didáticos, para praticar:

- Estruturas de repetição em JavaScript
- Seleção e manipulação de elementos do DOM
- Boas práticas ao evitar repetição de código (DRY)

## 👤 Autor

<div align="center">Desenvolvido por Marcelo Teixeira</div>
