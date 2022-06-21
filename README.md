# Omnifood landing page

## Conteúdo

- [Projeto](#projeto)
  - [Desafio](#desafio)
  - [Midia](#midia)
  - [Links](#links)
  - [Processo de Criação](#processo-de-criação)
    - [Construído com](#construído-com)
    - [Definição e Planejamento do projeto](#definição-e-planejamento-do-projeto)
    - [Esboço e criação das ideias para Layout](#esboço-e-criação-das-ideias-para-layout)
    - [Organização do primeiro design e o desenvolvimento das etapas](#organização-do-primeiro-design-e-o-desenvolvimento-das-etapas)
  - [Aprendizado](#aprendizado)
- [Autor](#autor)

## Projeto

Projeto final do curso da Udemy _Build Responsive Real-World Websites with HTML and CSS_.

O projeto consiste em uma empresa de tecnologia em primeiro lugar, mas com grande foco no bem-estar do consumidor por meio de uma alimentação saudável. A maioria das pessoas está muito ocupada com seus trabalhos, família e amigos e outras atividades importantes, o que não deixa muito tempo para cozinhar. Isso pode levar a uma dieta pobre e consequências duradouras para a saúde. Queremos resolver esse problema usando uma abordagem centrada em IA. Os usuários podem usar nosso aplicativo para selecionar sua dieta e alimentos que gostam e não gostam, e nosso algoritmo de IA criará um plano de refeições semanal personalizado e individual. Mas não paramos por aí. Fazemos parcerias com restaurantes e outros parceiros de culinária para realmente cozinhar e entregar todas as refeições dos planos de refeições gerados, em cidades selecionadas. Tudo isso será embalado em uma assinatura mensal, onde os usuários podem escolher entre receber uma ou duas refeições por dia, todos os dias do mês.

### Desafio

O projeto consiste em trabalhar tudo visto no curso de uma forma geral com HTML e CSS.

O maior desafio desse projeto foi personalizar a responsividade do seu jeito e como todas as @medias iriam se comportar de acordo com cada tamanho
de dispositivo.

### Midia

<div style="display: flex"  align="center"><br>
   <img height="400em" src="/assets/responsive-landing-page-web.gif" align="center" alt="web-lp" > <br><br><br>
   <img height="400em" src="/assets/form.gif" align="center" alt="form" > <br><br><br>
   <img height="400em" src="/assets/responsive-landing-page-medias.gif" align="center" alt="medias-lp" > <br><br><br>
   <img height="400em" src="/assets/lighthouse-test.png" align="center" alt="lighthouse" >
  <br><br>
</div>

### Links

- URL para o Site: [omnifood](https://omnifood-bruno-almeida.netlify.app/)

- _UI Faces_ para a implementação das fotos de rostos.
  [UIfaces](https://www.uifaces.co/browse-avatars/)

- _unsplash_ para a implementação das fotos de comidas e restaurante.
  [unsplash](https://unsplash.com/)

- _yeun_ para a obtenção da cor primária.
  [yeun](https://yeun.github.io/open-color/)

- _tints sand Shades_ para a determinação de cores mais escuras e mais claras par contrastes.
  [maketintsandshades](https://maketintsandshades.com/#e67e22)

- _ionic_ para a implementação dos icones.
  [ionic](https://ionic.io/ionicons)

- _coolors_ para a verificação de um bom contraste para melhor leitura do usuário
  [coolors](https://coolors.co/contrast-checker/112a46-acc8e5)

- _caniuse_ para a verificação de algumas propriedades funcionalidades do projeto corresponde à determinados browsers e suas versões, ex: _backdrop filter_
  [caniuse](https://caniuse.com/?search=backdrop%20filter)

- _squooshs_ para o redimensionamento das imagens tornarem o carregamento da landing page com melhor desempenho.
  [squoosh](https://squoosh.app/)

- _netlify_ para o deploy e back-end dos formulários.
  [netlify](https://www.netlify.com/)

## Processo de Criação

- Foram divididos em três partes do projeto: construção da estrutura completa inicialmente pra versão WEB; responsividade em todas as médias; e otimizações e deploy.

### Construído com

- HTML
- CSS
- Javascript

### Definição e Planejamento do projeto.

Foram divididos em três partes do projeto: construção da estrutura completa inicialmente pra versão WEB; responsividade em todas as médias; e otimizações e deploy.

Antes de tudo o mais importante é pensar na idéia do projeto e qual publico(nicho) irá atingir. Com a tecnologia e as AI que estão chegando no mercado com mais facilidade, esse projeto foi pensado para atingir pessoas que não tem tempo para cozinhar e que preservam sua saúde ao mesmo tempo.

### Esboço e criação das ideias para Layout

Com a ideia definida do projeto, chega a hora de rabiscar como será o layout. Essa primeira versão será feita de grafite para facilitar a criatividade de expor a ideia em um papel. Ideias de outros layouts de landing pages diferentes poderá lhe ajudar na criação das suas como mostra na sessão [Fotos e Video](#fotos-e-video). Após isso, caso consiga fazer o design do projeto em uma ferramenta como por exemplo o [Figma](https://www.figma.com/) a experiência será mais agradável na construção da landing page.

### Organização do primeiro design e o desenvolvimento das etapas

Essa etapa será como será organizado o projeto e quais ferramentas serão utilizadas como mostro na sessão [Links](#links). Será mais organizado se definirmos a padronização de core; typografia do sistema; tamanho de fontes; peso das fontes; cores; sobras; raio das bordas antecipadamente para uma experiência mais agradável.

### Aprendizado

O projeto consiste em uma criação de uma Landing Page moderna e com várias funcionalidades que o mercado presente utiliza.

Nesse projeto foi utilizada uma série de truques referentes a css como:

```
/* Imagem é elevada para cima ao passar o mouse*/
.meal:hover {
  transform: translateY(-1.2rem);
  box-shadow: 0 3.2rem 6.4rem rgba(0, 0, 0, 0.175);
}
```

```
/* Imagem é escalonada ao passar o mouse*/
.gallery-item img:hover {
  transform: scale(1.1);
}
```

```
/* Foi adicionado uma fita de melhor valor*/
.pricing-plan--complete::after {
  content: 'Best value';
  position: absolute;
  top: 6%;
  right: -18%;

  text-transform: uppercase;
  font-size: 1.4rem;
  font-weight: 700;
  color: var(--text-gray);
  background-color: #ffd43b;
  padding: 0.8rem 8rem;
  transform: rotate(45deg);
}
```

```
/* Foi implementado uma transparencia na imagem*/
.cta-img-box {
  background-image: linear-gradient(
      to right bottom,
        rgba(235, 151, 78, 0.35),
      rgba(230, 125, 34, 0.35)
    ),
    url(/img/eating.jpg);

  background-size: cover;
  background-position: center;
}
```

Poderia falar muito mais truques em que aprendi nesse projeto mas iria ficar muito grande esse readme.

A parte das @medias, foi algo que aprendi totalmente do zero, desde a criação da maior tela que seriam os desktops maiores, ate o mobile com o icone de navegação utilizando JavaScript caso o tamanho da tela seja estreito demais entre os tablents e os celulares. Outra parte interessante foi a grande vantagem do "display: grid" e do "grid-template-columns" para a manipulação da responsividade, tento classes predefinidas no "general.css" foi mais simples organizar os grids.

Foi utilizado o netlify para o deploy juntamente com o formulário, isso foi algo novo e de grande aprendizado utilizar uma ferramenta que hospede o back-end dos formulários.

Foi testado a eficiência do site utilizando a ferramenta do desenvolvedor do google [Lighthouse](https://web.dev/measure/) como você pode ver na sessão [Fotos e Video](#fotos-e-video) os resultados.

O objetivo dessa landing page e servir de modelo para novos projetos front-end e criação de landing pages semelhantes.

## Autor

<table>
  <tr>
    <td align="center">
      <a href="https://www.linkedin.com/in/rafael99ldm/">
        <img src="https://github.com/BrunoGaruda.png" width="100px;" alt="Foto de Bruno Almeida do GitHub"/><br>
        <sub>
          <b>Bruno Almeida</b>
        </sub>
      </a>
    </td>
  </tr>
</table>
