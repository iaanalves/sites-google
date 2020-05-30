[ SOBRE O HTML ]
- Utilizei um recurso chamado "reset css", que reseta sua página, deixando sem formatação nenhuma para que você possa codificar sem ter fogo-amigo do browser. 
Mas porque o reset css? 
Porque todo browser, possui por padrão, uma configuração padrão de estilos (pra cor, estilo de hyperlinks como a tag <a>, tamanho de <div>, etc), sendo assim, ele zera todos os valores e te deixa aplicar seu estilo customizado
- Removi todo o CSS do arquivo de HTML, e o joguei para o arquivo de CSS, dentro da pasta CSS
- O uso das tags <figure> e <figcaption> estavam certas, porém elas possuem um outro foco (futuramente eu explico), por isso, as troquei por <section> e <h2>, respectivamente.
- A <div> é uma tag útil, mas sementicamente, ela é genérica da genérica, a melhor utilização, são as tags do HTML5, onde ela deve ser substituida por <section>. Pra saber mais:
https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element#Separa%C3%A7%C3%A3o_de_conte%C3%BAdo
- Removi as propriedades "height" e "weight" (que no caso deveria ser width, de largura) das tags de <img>, e deixei para que o CSS manipulasse estes tamanhos, já que é trabalho do CSS ordenar o estilo que ele terá
- Removi as tags <br/>, elas são úteis, em caso de emergência, ou pra alguma gambiarra, num geral, o trabalho de quebra de layout, deve ser feito pelo CSS, pois como estava no layout proposto, o ESTILO DE CADA BOX, deveria ser: centralizado e um abaixo do outro, por isso a regra deve estar no CSS
- Uso do Flexbox: https://www.w3schools.com/css/css3_flexbox.asp , neste site explica com detalhs e exemplos, os vários jeitos que foram feitos. Neste projeto, usei o com space-between
 
[ SOBRE O CSS ]
- Usei um recurso de @import, para trazer o link das fonts para o CSS, já que as regras de estilo devem ficar nele
- Utilizei alguns recursos do CSS, (como uma hierarquia de elementos, não vou lembrar o nome ao certo disso, mas entenda por enquanto como hierarquia), ao invés de você precisar criar um class ou um id para os elementos. Exemplo:
#container section h2 { color: red}
Onde: dentro da tag con id container, TODO elemento html que seja do tipo SECTION, e que tenha um H2 dentro de sí, tenha a cor de texto vermelha
- Na ultima regra CSS, que tem um comentário BONUS, eu fiz um #container section a, e logo após um #container section a:hover. Este hover, indica que ao passar um mouse em cima, deve ter algum estilo aplicado, no caso, um color diferente, como está na regra feita
- box-sizing: border-box. Ex: se você tem uma <section> com 100px de width (largura) e resolve colocar um padding de 200px, automaticamente sua <section> vai aumentar de tamanaho, e vai ultrapassar 100px, com esta propriedade CSS chamada "box-sizing: border-box", você evita que isso acontece, mantendo sempre 100px de with na sua <section>
