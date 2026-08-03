# 🥁 Alura Midi

Um teclado MIDI de percussão feito com **HTML, CSS e JavaScript**, onde cada tecla do teclado do computador aciona um som de bateria/percussão diferente. Projeto desenvolvido durante um curso da Alura.

## 🎧 Demonstração

Abra o `index.html` no navegador e clique nos botões (ou use o teclado) para tocar os sons.

## ⌨️ Mapeamento das teclas

| Botão  | Tecla do teclado | Som        |
| ------ | :--------------: | ---------- |
| Pom    |       `Q`        | `keyq.wav` |
| Clap   |       `W`        | `keyw.wav` |
| Tim    |       `E`        | `keye.wav` |
| Puff   |       `A`        | `keya.wav` |
| Splash |       `S`        | `keys.wav` |
| Toim   |       `D`        | `keyd.wav` |
| Psh    |       `Z`        | `keyz.wav` |
| Tic    |       `X`        | `keyx.wav` |
| Tom    |       `C`        | `keyc.wav` |

## 🛠️ Tecnologias utilizadas

- **HTML5** — estrutura da página e elementos `<audio>`
- **CSS3** — estilização do teclado (`css/reset.css`, `css/estilos.css`)
- **JavaScript** — lógica para tocar os sons ao clicar/pressionar as teclas

## 📁 Estrutura do projeto

```
midi/
├── css/        # Arquivos de estilo
├── images/     # Ícones e imagens (ex: favicon)
├── sounds/     # Arquivos de áudio (.wav) de cada tecla
└── index.html  # Página principal
```

## 🚀 Como executar

1. Clone o repositório:
    ```bash
    git clone https://github.com/Juniklx/midi.git
    ```
2. Entre na pasta do projeto:
    ```bash
    cd midi
    ```
3. Abra o arquivo `index.html` no navegador de sua preferência.

## 📌 Status

Projeto simples de estudo, com foco em manipulação de elementos `<audio>` e eventos de clique/teclado em JavaScript.

## 📄 Licença

Este projeto é livre para fins de estudo.
