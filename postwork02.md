## Escribe la diferencia entre px y rem como unidades de medida.

El `pixel` es una unidad absoluta para definir el tamaño o posición de un elemento en el navegador que no cambia, sin embargo, tenemos muchos tipos de dispositivos con pantallas de muchos tamaños y esto nos lleva a cambiar la forma de crear las páginas web bajo un diseño responsivo.

El diseño responsivo permite que las páginas se adapten a los distintos tipos de pantalla, utilizando unidades como `rem`, los porcentajes y `em`.

`rem` es una unidad relativa, que nos permite contruir diseños escalables.

La unidad `rem` depende del elemento raíz (HTML). Esto quiere decir que se basa en el tamaño de la fuente del elemento raíz que es de 16px, por lo tanto:

1 `REM` = 16`px`

#### Ejemplo:

Definiremos el tamaño de la fuente de todo el sitio, que es de 16px y configuraremos una clase con un tamaño de 2rem y un elemento de 3rem.

El elemento `div` es de 2 rem, que equivale a 32px.

El elemento `div` con la clase top-div es de 3rem, que equivale a 48px.

![test-imagen](/test01.png)

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>postwork02</title>
    <!-- vinculo con archivo CSS -->
    <link rel="stylesheet" href="styles.css" type="text/css">
  </head>
  <body>
    <div>
      Titulo: Practica de REM
    </div>
    <div class="top-div">
      Aqui practicaremos un poco usando REM
    </div>
    <p>El dia es genial, difrutalo.</p>
  </body>
</html>
```

```css
html {
  font-size: 16px;
}

div {
  font-size: 3rem;
  border: 1px solid black;
}

.top-div {
  font-size: 2rem;
  border: 1px solid red;
}
```

## Trata de resolver tres problemas de Learn Git Branching.

![juego-imagen](/game01.png)

## Incluir dos fuentes de Google fonts en tu proyecto

![ejecucion-imagen](/sitio01.png)

```html
<!DOCTYPE html>
<html>
    <head>
        <!-- Aqui va la informacion importante pero no visible en el navegador -->
        <meta charset="utf-8">
        <title>
            Matcha WebPage
        </title>
        <!-- Aqui va el codigo de estilos, cuando no hay archivo CSS 
        <style>
            h1 {
                color: #025157;
            }
        </style>
        -->
        <!-- vinculo con archivo CSS -->
        <link rel="stylesheet" href="styles.css" type="text/css">
        <!-- fuentes -->
        <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
        <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Audiowide">

    </head>
    <body>
        <!-- Esto es lo que se vera en el navegador -->
        <header class="header">
            <!-- Logo con el link a la página principal -->
            <a href="/" class="logo">
                <img src="https://getmatcha.com/wp-content/uploads/2020/01/Icon-green.png" alt="imagen-logo-matcha"/>
            </a>
            <!-- Menu de navegacion -->
            <nav class="navbar">
                <ul>
                    <li class="menu-item">Platform</li>
                    <li class="menu-item">Pricing</li>
                    <li class="menu-item">Customers</li>
                    <li class="menu-item">Resources</li>
                    <li class="menu-item">About</li>
                </ul>
            </nav>
            <!-- Contenedor de acciones de usuario -->
            <div class="actions">
                <a>Sign In</a>
                <button>Start Free Trial</button>
            </div>
        </header>
        <section class="main">
            <h1> Build your blog. Build your bussiness. </h1>
            <p class="text-title">
                Instantly publish articles, drive more traffic, grow your email list, 
                and see your blog's impact on sales
            </p>
            <form>
                <input type="email" />
                <button class="btn-submit" type="submit">
                    Try it now ⇒
                </button>
            </form>
            <p class="text-promo"> Start publishing today with a <strong>free 7-day trial.</strong> </p>
            <p class="text-info"> <strong>No credit card</strong> required. </p>
            <img class="img-capterra" src="https://ignos.blog/wp-content/uploads/2021/04/capterra.png" alt="capterra image" />
            <img class="img-matcha" src="https://getmatcha.com/wp-content/uploads/2019/09/intro_group_image.png" alt="matcha image"/>
        </section>

    </body>
</html>
```

```css
body {
    background-color: #fffbf7;
}

.header {
    /* margin-top: 40px;
    margin-left: 20px;
    margin-right: 20px; */
    margin: 40px 20px 0px;
    font-size: 0;
    font-family: sans-serif;
    height: 45px;
}

.header > * {
    display: inline-block;
    font-size: 16px;
    vertical-align: middle;
    height: 100%;
    line-height: 45px;
}

.logo {
    width: 15%;
}

.logo > img {
    width: 15%;
}

.navbar {
    width: 70%;
    text-align: center;
    color: #025157;
    font-weight: 500;
}

.menu-item {
    margin-right: 25px;
    margin-left: 25px;
}

.actions {
    width: 15%;
    text-align: left;
    font-size: 14px;
    font-weight: 600;
}

.actions > * {
    margin-right: 10px;
    margin-left: 10px;
}

.actions a {
    color: #67b54b;
}

li {
    display: inline;
}

.main {
    margin-top: 140px;
    text-align: center;
}

h1 {
    color: #46484c;
    font-family: "Sofia", sans-serif;
    font-size: 30px;
    text-align: center;
}

p {
    color: #8b8b8bcc;
    font-family: Verdana;
    font-size: 20px;
}

.text-info {
    font-family: "Audiowide", sans-serif;
    font-size: 25px;
}

button {
    color: white;
    background-color: #67b54b;
    padding: 14px 12px 14px 12px;
    border: 0;
    border-radius: 5px;

}

img {
    display: block;
    margin-left: 15%;
    max-width: 70%;
}

.img-capterra{
    max-width: 40%;
    margin-left: 30%;
}
```
