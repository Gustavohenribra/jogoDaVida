# Engine jogo da vida

Este projeto é uma simulação do Jogo da Vida de Conway, implementado em C usando a biblioteca Raylib.

## Introdução

O Jogo da Vida de Conway foi criado pelo matemático britânico John Horton Conway em 1970, e é um jogo que objetiva simular os  movimentos das celulas. É um jogo que sua evolução é determinada pelo seu estado inicial, não exigindo nenhuma entrada adicional. Crie uma configuração inicial e observe como ela evolui.

## Regras do Jogo da Vida

O Jogo da Vida opera em uma grade bidimensional de células, cada uma das quais pode estar em um de dois estados possíveis: viva ou morta. A cada passo do tempo, as seguintes regras são aplicadas a cada célula:

1. **Subpopulação**: Qualquer célula viva com menos de dois vizinhos vivos morre, como se fosse por subpopulação.
2. **Sobrevivência**: Qualquer célula viva com dois ou três vizinhos vivos permanece viva para a próxima geração.
3. **Superpopulação**:  Qualquer célula viva com mais de três vizinhos vivos morre, como se fosse por superpopulação.
4. **Reprodução**: Qualquer célula morta com exatamente três vizinhos vivos se torna uma célula viva, como se fosse por reprodução.

## Requisitos

- Biblioteca [Raylib](https://www.raylib.com/) instalada.

## Uso

1. Clone o repositório:

    ```bash
    git clone https://github.com/Ayg0/conwaysGameOfLife.git
    ```

2. Navegue até o diretório do projeto:

    ```bash
    cd jogoDaVida
    ```

3. Compile o projeto:

    ```bash
    make
    ```

4. Execute o arquivo compilado:

    ```bash
    ./jogoDaVida
    ```

## Controles

- **P**: Pausar/Retomar a simulação.
- **+**: Aumentar a velocidade da simulação.
- **-**: Diminuir a velocidade da simulação.
- **CLIQUE ESQUERDO**: Adicionar uma célula viva --APENAS PAUSADO--.
- **CLIQUE DIREITO**: Remover uma célula viva --APENAS PAUSADO--.
- **N**: Avançar a simulação um quadro por vez --APENAS PAUSADO--.
