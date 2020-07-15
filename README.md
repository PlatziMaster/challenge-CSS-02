# 🎨 Challenge CSS 02

SASS Practice

## 🎨 ¿En qué consiste?

En este reto tendrás tres componentes: un código HTML, una fracción de código SASS y una fracción de código CSS. La idea, es que transformes el código CSS a SASS usando la metodología BEM. 

> * Código base: [Aquí](https://codepen.io/teffcode_/pen/xxZJNpo?editors=1100)
> * Guía base para instalación: [Aquí](https://github.com/teffcode/sass-workshop) // También puedes usar Codepen

Te dejo la siguiente documentación sobre SASS:

* [Documentación oficial | En inglés](https://sass-lang.com/guide)
* [Sass cheatsheet | En inglés](https://devhints.io/sass)
* [Introducción a SASS/SCSS | En español](https://galuxui.com.es/#/sass-facilito-parte-1)
* [SASS/SCSS para principantes | En español](https://galuxui.com.es/#/sass-facilito-parte-2)
* [SASS/SCSS intermedio | En español](https://galuxui.com.es/#/sass-facilito-parte-3)
* [SASS News | En inglés](http://thesassway.com/)

Te dejo la siguiente documentación sobre BEM:

* [What is BEM? And Why you should use it in your project. | En inglés](https://medium.com/@dannyhuang_75970/what-is-bem-and-why-you-should-use-it-in-your-project-ab37c6d10b79)
* [BEM Methodology | En inglés](https://en.bem.info/methodology/)
* [Get BEM | En inglés](http://getbem.com/introduction/)

### HTML

```
<header>
  <p>LOGO</p>
  <ul>
    <li>ABOUT</li>
    <li>ARTICLES</li>
    <li>SUBSCRIBE</li>
  </ul>
</header>
<main>
  <h1>GREEN</h1>
  <h2>HOLISTIC HEALTH</h2>
</main>
<section class="cards">
  <section class="card">
    <img class="card__img" src="https://images.pexels.com/photos/3674030/pexels-photo-3674030.jpeg?auto=compress&cs=tinysrgb&dpr=2&w=500" alt="">
    <h2 class="card__title">Title</h2>
    <p class="card__subtitle">Subtitle</p>
  </section>
  <section class="card">
    <img class="card__img" src="https://images.pexels.com/photos/3865676/pexels-photo-3865676.jpeg?auto=compress&cs=tinysrgb&dpr=2&w=500" alt="">
    <h2 class="card__title">Title</h2>
    <p class="card__subtitle">Subtitle</p>
  </section>
  <section class="card">
    <img class="card__img" src="https://images.pexels.com/photos/3059398/pexels-photo-3059398.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260" alt="">
    <h2 class="card__title">Title</h2>
    <p class="card__subtitle">Subtitle</p>
  </section>
</section>
<section class="social">
  <button class="social__button">ABOUT</button>
  <button class="social__button">ARTICLES</button>
  <button class="social__button">SUBSCRIBE</button>
</section>
<footer>
  <p>Gracias por visitarnos</p>
  <p>Estas son nuestras redes sociales</p>
  <div class="links">
    <a class="link-1" href="/">Facebook</a>
    <a class="link-2" href="/">Instagram</a>
    <a class="link-3" href="/">Twitter</a>
  </div>
</footer>
```

### SASS hasta el momento:

```
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');

body {
  margin: 0;
  padding: 0;
  font-family: 'Roboto', sans-serif;
}

header {
  background: HONEYDEW;
  display: flex;
  justify-content: space-between;
  padding: 0px 20px;
}

main {
  text-align: center;
}

.cards {
  display: flex;
  justify-content: space-evenly;
  margin-bottom: 30px;
}

.card {
  border-radius: 15px;
  overflow: hidden;
  background: HONEYDEW;
  display: flex;
  flex-direction: column;
  align-items: center;
  &__img {
    width: 200px;
    height: 120px;
    object-fit: cover;
  }
  &__subtitle {
    margin-top: 0px;
  }
}

.social {
  display: flex;
  justify-content: space-evenly;
  padding-bottom: 30px;
  &__button {
    padding: 10px 20px;
    border-radius: 20px;
    border: 3px solid HONEYDEW; 
  }
}
```

### CSS que debes "transformar" a SASS usando BEM:

Puedes usar mixins con parámetros 🤫

```
footer {
  background: HONEYDEW;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 30px 0px;
}

footer p {
  margin: 0px;
}

.links {
  margin: 15px 0px;
}

.link-1 {
  color: ORCHID;
}

.link-2 {
  color: MEDIUMTURQUOISE;
}

.link-3 {
  color: SALMON;
}
```

## 🎨 Pasos a seguir:

1. Hacer un "Fork" de este proyecto.
2. Resolver el reto.
3. Crear un Pull Request hacia este repositorio.

## 🎨 ¿Cómo contribuir?

Si quieres agregar o mejorar algo, te invito a colaborar directamente en este repositorio: [challenge-CSS-02](https://github.com/PlatziMaster/challenge-CSS-02)

## 🎨 Licencia

challenge-CSS-02 se lanza bajo la licencia [MIT](https://opensource.org/licenses/MIT).
