<div align="center">

![](assets/logo.png)

</div>

## Overview

O Jabiraca é um Framework Css/Js, open source, criado inicialmente como parte de um trabalho de conclcusão de curso quem tem como tema a introdução de novos desenvolvedores ao mundo do Open Source.
A ideia é manter o código o mais simples possível, para o fácil entendimento de qualquer desenvolvedor, a contribuição também é aberta para qualquer nível de conhecimento.

## Índice

- [Instalação](#instalação)
- [Normalize](#normalize)
- [Elementos](#elementos)
  - [Button](#button)
  - [Lista](#lista)
  - [Alertas](#alertas)
- [Contribuição](#contribuição)
- [License](#license)

## Instalação

Para realizar a instalação é só utilizar o comando abaixo:

```
npm install jabiraca-css
```

### Normalize

O Jabiraca está usando o [Normalize](https://github.com/necolas/normalize.css) para trabalhar a parte de padronização/normalização do html.

## Elementos

Até o momento o Jabirca conta com apenas 4 Elementos, button, footer, navbar e modal.

### Button

O Jabiraca apresenta alguns tipos de estilos botões pré-desenvolvidos para o uso, cada qual com sua necessidade.

```
<button class='button'></button>
<button class='button button__primary'></button>
<button class='button button__successs'></button>
<button class='button button__error'></button>
<button class='button button__danger'></button>
```

Há também os botões com estilo outline.

```
<button class='button-outline'></button>
<button class='button-outline button__primary'></button>
<button class='button-outline button__successs'></button>
<button class='button-outline button__error'></button>
<button class='button-outline button__danger'></button>
```

Há também os botões que preenche 100% do componente pai.

```
<button class='button button__primary button--full-size'>Button</button>
```

Há também os botões que se posicionam a cada lado do componente.

```
<button class='button button__primary button--left'>Button</button>
<button class='button button__primary button--right'>Button</button>
```

Há também os botões com box-shadow.

```
<button class='button button--shadow'>Button</button>
<button class='button button__primary button--shadow'>Button</button>
<button class='button button__success button--shadow'>Button</button>
<button class='button button__error button--shadow'>Button</button>
<button class='button button__danger button--shadow'>Button</button>
```

### Lista

O Jabiraca apresenta 2 tipos de layout de listas, numeradas ou não numeradas.

#### Lista não numeradas

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

#### Lista numeradas

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
<div class='alert alert__primary'>Alerta!!</div>
<div class='alert alert__success'>Alerta!!</div>
<div class='alert alert__error'>Alerta!!</div>
<div class='alert alert__danger'>Alerta!!</div>
```

## Contribuição

A contribuição é distribuição do conteúdo do framework segue todas as normas impostas pelo GitHub e pela Licença do projeto.

## License

MIT © [Ronaldofj](https://github.com/Ronaldofj)
