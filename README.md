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