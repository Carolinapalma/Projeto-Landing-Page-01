# <h1 align="center">Projeto Landing Page 01</h1>

## Indice


* [Visão geral](#visão-geral)
   * [Sobre](#sobre)
   * [Captura de tela](#captura-de-tela)
- [Processo](#processo)
   * [Construído com](#construído-com)
   * [O que eu aprendi](#o-que-eu-aprendi)
   * [Acesso a Página](#acesso-a-página)
   * [Autora](#autora)
---

## <p align="center">Visão geral</p>

### Sobre

Primeiro projeto de página única a partir do curso Dev em Dobro, que consiste em desafio de HTML e CSS avançado afim de aprimorar conhecimentos adquiridos e através de boas metodologias atualmente usadas no mercado de trabalho.


---

### Captura de tela

<img src="Landing-page.gif" alt="gif tela inicial do projeto agência xyz">
<br>

<p align="center">
<img src="Landing-page-responsivo.gif" align="center" alt="gif tela inicial responsivo do projeto agência xyz">

---
  
## <p align="center">Processo</p>

### Construído com

  * HTML semântica;
  * Animation CSS;
  * FlexBox;
  * GridBox;
  * Menu de Navegação;
  * Responsividade para dispositivos móveis.

---

### O que eu aprendi

Além das metodologias foram criados itens extras:

#### Menu Hamburguer

<br>

* Menu com propriedade transition pseudo-elementos (after e before):
```css
.header .hamburguer{
	background-color: #000;
	position: relative;
	display: block;
	width: 30px;
	height: 2px;
	top: 29px;
	left: 15px;
	transition: 0.5s ease-in-out; } 

.header .hamburguer::before, 
.header .hamburguer::after{
	background-color: #000;
	content: "";
	display: block;
	width: 100%;
	height: 100%;
	position: absolute;
	transition: 0.2s ease-in-out; }
```

* Menu com pseudo-elemento checked:
```css
.header input{
	display: none; }

.header input:checked ~ label .hamburguer{
	transform: rotate(45deg); }

.header input:checked ~ label .hamburguer::before{
	transform: rotate(90deg);
	top: 0; }

.header input:checked ~ label .hamburguer::after{
	transform: rotate(90deg);
	bottom: 0; }
```

#### Animação de seta no painel.

* Seta Animation
```css
.hero::after{
	content: url('../images/seta_preta.png');
	height: 35px;
	bottom: 40px;
	position: absolute;
	animation: downarrow 0.6s infinite alternate ease-in-out; }

@-webkit-keyframes downarrow {
	0%  {-webkit-transform: translateY(0); opacity: 0.4;}
	100%  {-webkit-transform: translateY(0.4em);
	opacity: 0.9;} }
```
---

### Acesso a Página

- [GitHub Page](https://carolinapalma.github.io/projeto-landing-page-01/)

---

## <p align="center">Autora</p>

### Carolina Palma
  
 * [LinkedIn](https://www.linkedin.com/in/carolina-palma-medeiros/) 
  
 * [GitHub](https://github.com/Carolinapalma)
