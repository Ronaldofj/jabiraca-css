<div align="center">

![](assets/logo.png)

</div>

## Overview

O Jabiraca é um Framework Css/Js, open source, criado inicialmente como parte de um trabalho de conclcusão de curso quem tem como tema a introdução de novos desenvolvedores ao mundo do Open Source.
A ideia é manter o código o mais simples possível, para o fácil entendimento de qualquer desenvolvedor, a contribuição também é aberta para qualquer nível de conhecimento.

## Índice

- [Instalação](#instalação)
- [Normalize](#normalize)
- [BEM](#bem)
- [Cores](#cores)
- [Elementos](#elementos)
  - [Button](#button)
  - [Listas](#listas)
  - [Alertas](#alertas)
  - [Cards](#cards)
- [Contribuição](#contribuição)
- [License](#license)

## Instalação

Para realizar a instalação é só utilizar o comando abaixo:

```
npm install jabiraca-css
```

### Normalize

O Jabiraca está usando o [Normalize](https://github.com/necolas/normalize.css) para trabalhar a parte de padronização/normalização do html.

## BEM

Todo o desenvolvimento do Jabiraca segue utilizando a metodologia de escrita de classes para o css de uma organizada. BEM significa B(_block_), E(_element_) e M(_modifier_), ou seja Bloco, Elemento e Modificador. A estrutra segue da seguinte maneira, todo o elemento pai será nomeado com uma usual, como "card", já o elemento filho, como "card\_\_header", vai ter o "\_\_" identificando que ele é um elemento do bloco "card". Por fim, se formos modificar de alguma forma nosso elemento, no caso o "card\_\_header", devemos repetir a classe com o seu modificador da seguinte forma, "card\*\*header card\_\_header--center", o "--" identifica o modificador da classe, que sempre irá realizar a ação de modificar alguma propriedade que estejá como padrão do elemento.

Exemplo de Código:

```
<div class='card'>
	<div class='card__header card__header--center>
		//...html
	</div>
	<div class='card__body card__body--center>
		//...html
	</div>
</div>
```

O BEM foi criado pelo time da Yandex, que é uma companhia de internet que tem sede da Russia, e que é um tipo de Google Russo. Segundo a Yandex as vantagens do BEM são:

- Facíl suporte a estrura do seu projeto à medida em que ele cresce
- Reutilização de Código
- Minimização de custo para atualizar o design, criar novos elementos e etc

## Cores

Segue abaixo a tabela que relaciona as cores com as classes que alteram a cor do elemnto.

| Classe Css | Cor (HEX) |
| ---------- | --------- |
| primary    | #5082ec   |
| success    | #57ff5f   |
| error      | #ff2119   |
| danger     | #ff7221   |

## Elementos

O Jabiraca conta com diversos elementos para ajudar no desenvolvimento do seu projeto.
Lembre-se, esse projeto não é perfeito e a sua sugestão é sempre bem vinda. =)

### Button

Há alguns tipos de botões com estilos pré-definidos para o uso instantâneo:

#### Botão padrão

Estilo padrão dos botões, apenas com as cores e um _hover_ bem sutil:

```
<button class='button'></button>
<button class='button button--primary'></button>
<button class='button button--successs'></button>
<button class='button button--error'></button>
<button class='button button--danger'></button>
```

#### Botão outline

Estilo com fundo sem cor, e com bordas coloridas, _hover_ preenchendo o botão com a mesma cor da borda:

```
<button class='button-outline'></button>
<button class='button-outline button--primary'></button>
<button class='button-outline button--successs'></button>
<button class='button-outline button--error'></button>
<button class='button-outline button--danger'></button>
```

#### Modificadores auxiliares dos botões

Preenchendo 100% do componente em que o botão foi inserido:

```
<button class='button button--primary button--full-size'>Button</button>
```

Há também os botões que se posicionam a cada lado do componente.

```

<button class='button button--primary button--left'>Button</button>
<button class='button button--primary button--right'>Button</button>

```

Há também os botões com box-shadow.

```

<button class='button button--shadow'>Button</button>
<button class='button button--primary button--shadow'>Button</button>
<button class='button button--success button--shadow'>Button</button>
<button class='button button--error button--shadow'>Button</button>
<button class='button button--danger button--shadow'>Button</button>

```

### Listas

O Jabiraca apresenta 2 tipos de layout de listas, numeradas ou não numeradas.

#### Listas não numeradas

Lista normal sem estilização.

```

<div class='list-ul'>
	<p class='list-ul__title'>Linguagens</p>
	<ul class='list-ul__body'>
		<li class='list-ul__item'>JavaScript</li>
		<li class='list-ul__item'>PHP</li>
		<li class='list-ul__item'>Java</li>
	</ul>
</div>
```

Lista com estilização e componentes centralizados.

```
<div class='list-ul list-ul--center'>
	<p class='list-ul__title list-ul__title--primary'>Linguagens</p>
	<ul class='list-ul__body'>
		<li class='list-ul__item'>JavaScript</li>
		<li class='list-ul__item'>PHP</li>
		<li class='list-ul__item'>Java</li>
	</ul>
</div>
```

#### Listas numeradas

Lista numerada normal sem estilização.

```
<div class='list-ol'>
	<p class='list-ol__title'>Linguagens</p>
	<ol class='list-ol__body'>
		<li class='list-ol__item'>JavaScript</li>
		<li class='list-ol__item'>PHP</li>
		<li class='list-ol__item'>Java</li>
	</ol>
</div>
```

Lista com estilização e componentes centralizados.

```
<div class='list-ol list-ol--center'>
	<p class='list-ol__title list-ol__title--primary'>Linguagens</p>
	<ol class='list-ol__body'>
		<li class='list-ol__item'>JavaScript</li>
		<li class='list-ol__item'>PHP</li>
		<li class='list-ol__item'>Java</li>
	</ol>
</div>
```

### Alertas

O Jabiraca tem também vários modelos de alertas.

```
<div class='alert alert--primary'>Alerta!!</div>
<div class='alert alert--success'>Alerta!!</div>
<div class='alert alert--error'>Alerta!!</div>
<div class='alert alert--danger'>Alerta!!</div>
```

Há também os alertas com um pouco mais de informação.

```
<div class='alert alert--primary'>
	<div class='alert__header'>
		Alerta!!
	</div>
	<div class='alert__body'>
		Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur est dolore culpa odit? Alias, corrupti. Iure, eveniet? Ipsam dolor aliquam incidunt sed explicabo rerum necessitatibus!
	</div>
</div>
```

### Cards

Há também os cards, há dois modifcadores com tamanhos pré definidos, "card--medium", que tem o width setado em "500px" e o "card-tiny", que tem o width setado em "300px"

```
<div class="card">
	<div class="card__header">
		Card Teste
	</div>
	<div class="card__body">
		Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae enim eius explicabo, impedit quisquam illum recusandae ipsa, veritatis eum tenetur minus vero ipsum quidem? Vel!
	</div>
	<div class="card__footer">
		<button class='button button--primary'>Ok</button>
	</div>
</div>
```

## Contribuição

## License

MIT © [Ronaldofj](https://github.com/Ronaldofj)
