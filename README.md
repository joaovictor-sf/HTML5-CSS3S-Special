# HTML5 CSS3 Recursos Especiais

## Borda Circular
Para fazer uma borda com pontas circulares, e possivelmente até fazer um container em formado circular, utiliza-se a propriedade border-radius.
    
    -webkit-border-radius: 20px 90px;
    -moz-border-radius: 20px 90px;
    border-radius: 20px 90px;

### border-radius
Serve para arredondar as bordas de um container, quanto mais pixels tiver mais redondo é o container.

Pode ser usados para fazer um espaço para fotos de perfil

Você pode colocar valores diferentes para cada canto da borda se quiser

Navegadores mais antigos não suportam o border-radius, então para funcionar é bom adicionar mais duas versões

* <strong>-webkit-</strong> para versões antigas do Chorome e do Safari
* <strong>-moz-</strong> para versões antigas do Firefox

## Maior controle do tamanho do container

A propriedade “box-sizing” permite definir como o tamanho de um elemento deve ser interpretado em relação ao conteúdo, à borda e ao preenchimento(padding) do elemento.

Existem dois valores principais para a propriedade box-sizing: content-box (valor padrão) e border-box.

A escolha entre content-box e border-box depende da preferência e necessidades do desenvolvedor. O uso de border-box pode ser especialmente útil em layouts responsivos, onde o tamanho total de um elemento precisa ser controlado de maneira mais previsível. Ele permite que você defina o tamanho total do elemento e, em seguida, ajuste o conteúdo, a borda e o preenchimento dentro desse espaço sem que o elemento se expanda além do tamanho desejado.

Assim como no border-radius, é necessário acrescentar versões -webkit- e -moz- para funcionar em todos os navegadores.

## Opacidade
Para deixar algo transparente é necessário selecionar uma cor com rgb e acrescentar mais um valor, esse valor será a transparência, quanto menor mais transparente.

<strong>0</strong> - invisivel;

<strong>1</strong> - completamente visível;

Exemplo:

    rgb(0, 0, 0, 0.6)

## Degradê
Existem diversos tipos de degradê, aqui está alguns deles:
radial-gradient: degradê vindo do meio;
linear-gradient: degradê vindo dos lados;

Para mais informações olhar <a href="https://www.w3schools.com/colors/colors_gradient.asp">w3schools</a>

    background: radial-gradient(red, blue, green);
    background: linear-gradient(red, blue);
    background: linear-gradient(to bottom, #ff0000 0%, #0000ff 100%);
    background: linear-gradient(to right, #ff0000 0%, #0000ff 100%);
    background: linear-gradient(to top left, #ff0000 0%, #0000ff 100%);
    background: linear-gradient(to top right, #ff0000 0%, #0000ff 100%);
    background: linear-gradient(to top, #ff0000 0%, #0000ff 100%);
    background: linear-gradient(to left, #ff0000 0%, #0000ff 100%);
    background: linear-gradient(to bottom left, #ff0000 0%, #0000ff 100%);
    background: linear-gradient(to bottom right, #ff0000 0%, #0000ff 100%);

## Sombreamento
Para criar uma sombra, utiliza-se text-shadow(para texto) e box-shadow(para containers).

Eles funcionam da seguinte maneira:
        
        text-shadow/box-shadow: horizontal vertical blu(opcional)(fará a sombra fica borrada) cor(é interessante utilizar rgb para deixar a sombra com certa transparência);

No caso do box-shadow,  outra variável que é possível colocar: espaçamento, o quanto a sombra se espalha ou diminui.

    text-shadow: 3px -3px 5px rgb(0, 0, 0, 0.6);
    box-shadow: 5px 5px 5px 5px rgb(0, 0, 0, 0.6);

## Animação
Existe um mundo inteiro de maneiras de criar animações com css, é sinceramente incrível

Explicarei apenas o básico:
    
    @keyframes sinaliza que você está iniciando uma animação animation chamará a animação e a edita.

Assim como o border-radius, é necessário utilizar versões diferentes para funcionar em navegadores específicos: 

        @-webkit-keyframes
        @-moz-keyframes
        @-o-keyframes

animation também precisa dos prefixos:

        -webkit-animation
        -moz-animation
        -o-animation

### Tipos de animation

Chama a animação: animation-name: animacao-caixa;

Quanto tempo ela irá durar: animation-duration: 5s;

Quanto tempo até ela começar: animation-delay: 3s;

Quantas vezes ela irá se repetir, infinite faz a animação se repetir infinitamente: animation-iteration-count: 2;

Decide se a animação teve acontecer em reverso: animation-direction: alternate;

Esses tipos podem ser juntados em um só
animation: animacao-caixa 5s 3s infinite alternate;

## Transições
A propriedade transition serve para atrasar a transformação de um objeto, criando uma "animação".

Assim como outros exemplos, é necessário versões com -o-, -moz- e -webkit-

Pode ser feito com apenas um componente, atrasando todos os efeitos, ou você pode especificar quanto tempo você quer que cada mudança aconteça.

    transition: 3s;
    ou
    transition: width 3s, background 10s;
