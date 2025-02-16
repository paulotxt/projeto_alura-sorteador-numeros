# Sorteador de Números

Este é um projeto simples que utiliza lógica de programação para criar um sorteador de números. O objetivo é gerar números aleatórios dentro de um intervalo especificado pelo usuário, garantindo que cada número tenha a mesma probabilidade de ser sorteado.

## Funcionalidades

- **Definir Intervalo**: O usuário pode definir um intervalo de números para o sorteio.
- **Quantidade de Números**: O usuário pode escolher quantos números deseja sortear.
- **Sorteio Único**: Cada número sorteado é único dentro do intervalo especificado.
- **Reiniciar Sorteio**: O usuário pode reiniciar o sorteio para gerar novos números.

## Como Usar

1. **Defina a Quantidade de Números**: Insira a quantidade de números que deseja sortear no campo "Quantidade de números".
2. **Defina o Intervalo**: Insira o número inicial no campo "Do número" e o número final no campo "Até o número".
3. **Clique em Sortear**: Clique no botão "Sortear" para gerar os números aleatórios.
4. **Reiniciar**: Clique no botão "Reiniciar" para limpar os campos e realizar um novo sorteio.

## Estrutura do Projeto

- **index.html**: Contém a estrutura HTML da interface do usuário.
- **app.js**: Contém a lógica de programação para o sorteio e manipulação dos elementos da interface.
- **style.css**: Contém os estilos CSS para a interface do usuário.

## Exemplo de Uso

```html
<div class="container">
    <div class="container_conteudo">
        <div class="container_informacoes">
            <div class="container_texto">
                <h1>Sorteador<span class="container_texto-azul"> de números</span></h1>
                <div class="container_campo">
                    <label class="texto_paragrafo">Quantidade de números</label>
                    <input class="container_input" id="quantidade" type="number" min="1">
                </div>
                <div class="container_campo">
                    <label class="texto_paragrafo">Do número</label>
                    <input class="container_input" id="de" type="number" min="1">
                </div>
                <div class="container_campo">
                    <label class="texto_paragrafo">Até o número</label>
                    <input class="container_input" id="ate" type="number" min="1">
                </div>
            </div>
            <div class="chute container_botces">
                <button onClick="sortear()" id="btn-sortear" class="container_botao">Sortear</button>
                <button onClick="reiniciar()" id="btn-reiniciar" class="container_botao-desabilitado">Reiniciar</button>
            </div>
            <div class="container_texto" id="resultado">
                <label class="texto_paragrafo">Números sorteados: nenhum até agora</label>
            </div>
        </div>
        <img src="./img/ia.png" alt="Uma pessoa com capacete de astronauta" class="container_imagem-pessoa" />
    </div>
</div>
