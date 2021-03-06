# Proyecto para Curso Práctico Responsive Design Platzi 👩‍💻 🤖 👀

## Documentación y recursos entregados por Platzi

- Coach: Diego De Granda

- [Wireframes o Mockups en Figma](https://www.figma.com/file/sMmlQaZldfDcLERYYWe6h4/Bata-Bit)

- [Diseño Mobile](https://www.figma.com/proto/sMmlQaZldfDcLERYYWe6h4/Bata-Bit?node-id=44%3A594&scaling=scale-down)



## Paso a paso desarrollo del proyecto🏃‍♀️📝🏃‍♀️

## Dia 1

1. Lo primero que se realizó fue abrir la carpeta del proyecto con el editor de código (Visual Studio Code) y crear el archivo "readme.md" para comenzar a documentar el proceso.

2. Se creo la carpeta del proyecto en GitHub con el nombre de "batatabitPlatzi" para contar con el proyecto dentro de los repositorios de GitHub y asi ir subiendo los avances en este proyecto.

3. Ahora se conectará y se subirá los adelantos que hasta el momento se tienen en el repositorio local al repositorio en GitHub.

    Lo primero es inicializar el repositorio git en mi carpeta local:
    ```
    git init
    ```
    Despues se hace git add . para agregar a la trazabilidad del proyecto los archivos y carpetas que tenemos hasta el momento
    ```
    git add .
    ```
    Despues realizamos un git commit con el mensaje de este commit para documentar mejor la trazabilidad en git.
    ```
    git commit -m "Inicio del proyecto, documentando paso a paso inicial en archivo readme.md"
    ```

    Ahora sí siguiendo las instrucciones que en GitHub aparecen para subir el repositorio local al repo remoto de GH:

    **…or push an existing repository from the command line**
    ```
    git remote add origin https://github.com/KGISELLE/batatabitPlatzi.git
    git branch -M main
    git push -u origin main
    ```

4. En la [Clase 2: Analizando el diseño](https://platzi.com/clases/2030-mobile-first/32493-analizando-el-diseno/), revisamos los wireframes(Mockups) del diseño en Figma para conocer así el proyecto.

5. Algunas notas de la [Clase 3: El valor de Mobile First](https://platzi.com/clases/2030-mobile-first/33281-el-valor-de-mobile-first/):

    - **Responsive Design:** En responsive design un diseño se adaptará a distintas vistas independientemente para cuál dispositivo se desarrolló primero y con este estándar (Mobile First) primero crearemos para dispositivos móviles.

    - **¿Por que es importante el Resposive Design?**
    1. Pasar un desarrollo con vista de escritorio a móvil requiere de realizar diversas consideraciones, puede tornarse complejo pues además esto implica tener que eliminar elementos de la vista y generalmente es más fácil añadirlos.
    2. Google comenzó trabajar a inicios de 2018 con un algoritmo que otorga de mayor relevancia a aquellos sitios optimizados para móviles. Esto no afectará a aquellos sitios que tengan una versión de escritorio y móvil, pero sí penalizará a los que carezcan de una alternativa móvil.
    
6. En la [Clase 4: Arquitectura inicial](https://platzi.com/clases/2030-mobile-first/32301-arquitectura-inicial/), revisamos los wireframes(Mockups) del diseño en Figma para comenzar la arquitectura inicial en HTML.
    - **Arquitectura web:** Se puede definir como la forma en que las páginas de un sitio web están estructuradas y enlazadas entre sí (de manera lógica y coherente). Una arquitectura web ideal ayuda a los usuarios y a los motores de búsqueda a encontrar fácilmente lo que están buscando en un sitio web.  ***Arquitectura del proyecto:*** *Header *4 secciones *Footer

<br>

7. Se crea el archivo "index.html" en el proyecto y creamos nuestra estructura inicial html:5.
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        <header></header>
        <main>
            <section></section>
            <section></section>
            <section></section>
            <section></section>
        </main>
        <footer></footer>
    </body>
    </html>
    ```

    ***Nota: Cuando yo pongo el proyecto en un servidor, lo primero que este servidor busca es el archivo index.html para poder iniciar el proyecto, es decir lo primero que el navegador renderiza.***

8. En la [Clase 5: Assets de nuestro proyecto](https://platzi.com/clases/2030-mobile-first/32302-assets-de-nuestro-proyecto/), creamos la carpeta assets para poder almacenar allí las imagenes y los iconos que utilizaremos en el proyecto, creando asi mismo estas dos carpetas dentro de la carpeta assets.

9. Descargamos estas imagenes e iconos del diseño en Figma que nos entregan los diseñadores y las almacenamos en la carpeta📁 "assets", intentar en lo posible exportar las imagenes en figma en formato SVG para que nuestras imagenes no se pixelen en la interfaz.

10. Importante cambiar los nombres de las imagenes y los iconos que vienen por defecto de Figma, porque el nombre de estos debe ser muy descriptivo en nuestro proyecto, sin dejar espacios en el nobre podemos remplazarlo por - o _ y que los nombres de los archivos esten todos en minuscula.

11. En la [Clase 6: Fuentes de nuestro proyecto](https://platzi.com/clases/2030-mobile-first/32303-fuentes-de-nuestro-proyecto/), agregamos los tipos de fuentes que utilizaremos en el proyecto desde Google Fonts.

12. Buscamos en el diseño de figma las fuentes sugeridas.

    ***Nota: Por buena práctica en el diseño no podemos agregar más de dos tipos de fuentes, las fuentes son "DM Sans" e "Inter".***

13. Las dos fuentes del diseño las buscamos en [Google Fonts](https://fonts.google.com/), agremos para la fuente "DM Sans" las fuentes con peso 400, 500 y 700, y para la fuente "Inter" las fuentes con peso 300, 500 y 700.

14. Ahora vamos a pegar el link en nuestro archivo inicial "index.html" para agregarlas a nuestro proyecto. Copiamos el link dentro de la etiqueta `<head>`, despues de la etiqueta `<title>`.
    ```html
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>

        <!-- Fuentes DM sans e Inter agregadas desde google fonts -->
        <link rel="preconnect" href="https://fonts.googleapis.com">
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
        <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;700&family=Inter:wght@300;500;700&display=swap" rel="stylesheet">
    </head>
    ```

    ***Nota: Por buena práctica cuando tenemos mas de una fuente descargada de Google Fonts, es mejor agregarla a nuestro proyecto por medio de la etiqueta `<link>` en el archivo HTML y NO usando el @import en el CSS.***

15. En la [Clase 7: Estilos base](https://platzi.com/clases/2030-mobile-first/32304-estilos-base/), agregamos los estilos iniciales y las variables que nos ayudarán a realizar el proyecto.

16. Creamos el archivo "styles.css", para comenzar a declarar nuestras variables de estilo, quedando así:
    ```css
    :root {
        /* Colores */
        --bitcoin-orange: #F7931A;
        --soft-orange: #FFE9D5;
        --secondary-blue: #1A9AF7;
        --soft-blue: #E7F5FF;
        --warm-black: #201E1C;
        --black: #282623;
        --grey: #BABABA;
        --off-white: #FAF8F7;
        --just-white: #fff;
        --font-sm: 1.4rem;
        --font-md: 1.8rem;
        --font-lg: 2.4rem;
    }

    /* Utilizamos el selector universal para resetar nuestros estilos iniciales */
    * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
    }
    /* utilizamos este selector html para hacer uso del rem */
    html {
        font-size: 62.5%;
        font-family: 'DM Sans', sans-serif;
        font-family: 'Inter', sans-serif;
    }
    ```

17. Para crear las variables de color, tomamos como referencia las variables que ya estan creadas en Figma y las replicamos en nuestro archivo "styles.css

***Nota: Utilizar convenciones recomendas para organizar nuestras variables.***

    1. Posicionamiento --> static, absolute, relative, fixed
    2. Modelo de caja (Box model) --> margin, border, padding, content
    3. Tipografía --> tipos, tamaños de fuente, etc
    4. Estilos visuales --> box-shadow, border-radius, gradient, etc
    5. Otros --> reglas CSS y más

18. Despues utilizamos el selector universal para resetar nuestros estilos iniciales.

19. y por último utilizamos el selector de la etiqueta html para hacer uso del rem en vez de pixeles cuando trabajamos fuentes.
    ```html
    Nota: Explicación regla font-size: 62.5%;
    * 1 rem = 16px 
    * 62.5% * 16px = 10px 
    => 10px = 1 rem.

    * Y con regla de 3 se halla el 62.5%
    16px = 100%
    10px = x
    ```

    >"Históricamente se ha dicho que para poder usar REM en CSS, debemos primero pasar el font size del selector HTML a 62.5%, de tal forma que nos resulte sencillo usar la medida REM asimilándolo con pixeles. Así por ejemplo, para conseguir una medida de 12px, deberíamos usar 1.2rem. 
    
    >Es algo bastante útil y sencillo, pero hace que el navegador tenga que dar vueltas innecesarias para calcular las medidas de los elementos e ignoremos las configuraciones de tamaño que el usuario tenga en su navegador y esto puede tener algunos efectos visuales indeseados, por eso, lo que propongo con esta herramienta es que usemos REM, sin la necesidad de cambiar el tamaño base de HTML manteniendo su ***medida estándar que originalmente es 16px***." -[@FranciscoAMK](https://franciscoamk.com/herramientas/rem/#:~:text=Hist%C3%B3ricamente%20se%20ha%20dicho%20que,12px%2C%20deber%C3%ADamos%20usar%201.2rem.)


    >Siempre es mejor usar font-size: 62.5%. Lo que hace CSS es calcular el 62.5% del valor de font size que el navegador le indique (por defecto es 16). Es indispensable usar esto y no 10px ya que los píxeles son unidades absolutas y el % es relativo. Si usamos la medida relativa (62.5), cuando un usuario con problemas visuales aumente el tamaño de letra desde el navegador, la letra escalará de tamaño, en cambio si usamos píxeles la letra no escalará de tamaño ya que los píxeles son fijos (absolutos). -[ramirouffelmann](https://platzi.com/discusiones/2008-html-css/111887-al-hacer-el-truco-de-emfont-size-625em-625-16px-10px-si-la-etiqueta-html-tendra-ese-valor-10px-de-font-size-entonces/)


20. Tambien dentro del selector de la etiqueta html, agregamos el estilo de las fuentes de google fonts.


## Dia 2

### Realizando el Header

1. En la [Clase 8: Maquetación del header](https://platzi.com/clases/2030-mobile-first/32305-maquetacion-del-header/),comenzamos con  la estructura inicial del header.
    ```html
    <header>
        <img src="./assets/imgs/logo.svg" alt="logo">
        <div>
            <h1>La próxima revolución en el intercambio de criptomonedas.</h1>
            <p>Batatabit te ayuda a navegar entre los diferentes precios y tendencias.</p>
            <a href="">Conoce Nuestros Planes <span>i</span></a>
        </div>
    </header>
    ```

2. En la [Clase 9: Implementando BEM](https://platzi.com/clases/2030-mobile-first/32306-implementando-bem/),comenzamos a generar las clases para nuestras etiquetas basados en la metodologia BEM. * Se aconseja repasar documentación acerca de la [metodologia BEM](https://en.bem.info/methodology/faq/#why-bem) para tener una guia de como nombrar nuestras clases.

    ```
    class="header--title-container"
    class="bloqueprincipal--elemento"
    ```

    ```html
    <header>
        <img src="./assets/imgs/logo.svg" alt="logo">
        <div class="header--title-container">
            <h1>La próxima revolución en el intercambio de criptomonedas.</h1>
            <p>Batatabit te ayuda a navegar entre los diferentes precios y tendencias.</p>
            <a href="" class="header--button">Conoce Nuestros Planes <span>i</span></a>
        </div>
    </header>
    ```


    ***Nota: El `<header>` al ser una etiqueta principal que solo usaremos una vez, es decir no la vamos a replicar en el proyecto, no necesita una clase.***

    ***Nota: En el caso de `<img>` podemos utilizar la especificidad de CSS para llamar esta etiqueta a través del header si no tenemos más img en el proyecto dentro de una etiqueta de header.***

    ***Nota: En el caso de los `<div>` si tendremos que colocar una clase porque esta etiqueta es muy comun en la estructura del proyecto.***

    <br>

3. En la [Clase 10: Uso de linear-gradient](https://platzi.com/clases/2030-mobile-first/32307-uso-de-linear-gradient//), una vez agregadas las clases a nuestros elementos html, vamos al archivo "style.css", pero sin olvidarnos de vincular esta hoja de estilos en nuestro html.
    ```css
    header {
        position: relative;
        display: flex;
        flex-direction: column;
        justify-content: center;
        width: 100%;
        min-width: 320px;
        height: 334px;
        text-align: center;
        background: linear-gradient(207.8deg, #201E1C 16.69%, #F7931A 100%);
    }
    header img {
        width: 150px;
        height: 24px;
        margin-top: 60px;
        align-self: center;
    }
    .header--title-container {
        width: 90%;
        min-width: 288px;
        max-width: 900px;
        height: 218px;
        margin-top: 40px;
        text-align: center;
        align-self: center;
    }
    .header--title-container h1 {
        font-size: var(--font-xl);
        font-weight: bold;
        line-height: 2.6rem;
        color: var(--just-white);
    }
    .header--title-container p {
        margin-top: 25px;
        font-size: var(--font-sm);
        font-weight: 500;
        line-height: 1.8rem;
        color: var(--soft-orange);
    }
    ```

4. En la [Clase 11: Uso de position para botón flotante](https://platzi.com/clases/2030-mobile-first/32308-uso-de-position-para-boton-flotante/), para finalizar el header vamos a darle estilos al botón flotante. En esta clase se aprendio a utilizar flex para posicionar de forma mas sencilla los elementos en un contenedor, box-shadow para darle sombra al botón para que se vea flotante, composition para posicionar ciertos elementos que esten en el layout

    ***Nota: Recoremos que el position: absolute; toma como position: relative; a su padre directo, que en el caso es el header y le da el beneficio de poderse reposicionar en cualquier parte del header, a pesar de que existan más elementos en la sección del header.***

## Realizando Section exchange dentro del main

5. En la [Clase 12: Estructura base de la sección de intercambio](https://platzi.com/clases/2030-mobile-first/32309-estructura-base-de-la-seccion-de-intercambio/), comenzamos con la estructrura inicial en html.
    ```html
    <section class="main--exchange-container">
        <div class="backgroundImg"></div>
        <div class="main--exchange-container-title">
            <h2>Visibilizamos todas las tasas de cambio.</h2>
            <p>Traemos información en tiempo real de las casas de cambio y las monedas más importantes del mundo.</p>
        </div>
        <section class="main--tables-container">
            <div>

            </div>
        </section>
    </section>
    ```
6. Seguimos con los estilos en el archivo "styles.css"
    ```css
    main {
        width: 100%;
        height: auto;
        background-color: var(--off-white);
    }
    .main--exchange-container {
        width: 100%;
        height: auto;
        padding-top: 80px;
        padding-bottom: 30px;
        text-align: center;
    }
    .main--exchange-container-title {
        width: 90%;
        min-width: 288px;
        max-width: 900px;
        margin: 0 auto;
    }
    ```
7. En la [Clase 13: Imagen de background](https://platzi.com/clases/2030-mobile-first/32310-imagen-de-background/), agregamos la imagen del bitcoin como background en CSS.
    ```css
    .main--exchange-container .backgroundImg {
        width: 200px;
        height: 200px;
        margin: 0 auto;
        margin-bottom: 50px;
        background-image: url("./assets/imgs/bitcoin.svg");
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
    }
    ```

    ***Nota: Tener en cuenta que si no le damos propiedades de tamaño a nuestro `<div class="backgroundImg">` no se nos mostrará la imagen introducida en css con `background-image: url("./assets/imgs/bitcoin.svg");`.***

    ***Nota: Para evitar que nuestra imagen se deforme al agrandar o achicar la pantalla existen buenas practicas para arreglar esto, que es utilizar `background-size: cover;` `background-position: center;` `background-repeat: no-repeat;`.***

8. Ahora agregramos los estilos al texto que esta dentro de esta sección.
    ```css
    /** Estilos section exchange */
    .main--exchange-container {
        width: 100%;
        height: auto;
        padding-top: 60px;
        padding-bottom: 30px;
        text-align: center;
    }
    .main--exchange-container-title {
        width: 90%;
        min-width: 288px;
        max-width: 900px;
        margin: 0 auto;
    }
    .main--exchange-container .backgroundImg {
        width: 200px;
        height: 200px;
        margin: 0 auto;
        margin-bottom: 50px;
        background-image: url("./assets/imgs/bitcoin.svg");
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
    }
    .main--exchange-container h2 {
        margin-bottom: 30px;
        font-size: var(--font-lg);
        font-weight: bold;
        line-height: 2.6rem;
        color: var(--warm-black);
    }
    .main--exchange-container p {
        margin-bottom: 30px;
        font-size: var(--font-sm);
        font-weight: 500;
        line-height: 1.8rem;
        color: #757575;
    }
    ```

## Dia 3

## Seguimos con Section exchange dentro del main

1. En la [Clase 14: Estructura de tabla de monedas](https://platzi.com/clases/2030-mobile-first/32311-estructura-de-tabla-de-monedas/), creamos la tabla donde se agregará la info sobre las monedas, las tablas se pueden trabajar con las etiquetas de tabla en HTML ó con grid en CSS, para este caso se trabjará con las etiquetas de tabla.
    ```html
    <section class="main--tables-container">
        <div class="main-currency-table">
            <p class="currency-table--title">Monedas</p>
                <div class="currency-table--container">
                    <table>
                        <tr>
                            <td class="table__top-left">Bitcoin</td>
                            <td class="table__top-right table__right">$1.96 <span>i</span></td>
                        </tr>
                        <tr>
                            <td>Ethereum</td>
                            <td class="table__right">$0.07 <span>i</span></td>
                        </tr>
                        <tr>
                            <td>Ripple</td>
                            <td class="table__right">$2.15 <span>i</span></td>
                        </tr>
                        <tr>
                            <td class="table__bottom-left">Stellar</td>
                            <td class="table__bottom-right table__right">$4.96 <span>i</span></td>
                        </tr>
                    </table>
                </div>
                <div>
                    <p><b>Actualizado:</b> 19 Julio 23:45</p>
                </div>                                                   
        </div>            
    </section>                              
    ```

2. En la [Clase 15: Estilos base de tabla de monedas](https://platzi.com/clases/2030-mobile-first/32312-estilos-base-de-tabla-de-monedas/), le damos estilos a la table creada en la anterior clase.
    ```css
    .main-currency-table {
        width: 70%;
        min-width: 235px;
        max-width: 500px;
        height: 360px;
        margin: 0 auto;
        font-family: 'Inter', sans-serif;
    }
    .main-currency-table .currency-table--title {
        margin-bottom: 15px;
        font-size: 1.8rem;
        font-weight: bolder;
        line-height: 2.3rem;
        color: var(--bitcoin-orange);
    }
    .currency-table--container {
        width: 90%;
        min-width: 230px;
        max-width: 300px;
        height: 250px;
        margin: 0 auto;
    }
    .currency-table--container table {
    width: 100%;
    height: 100%;
    }
    .currency-table--container td {
        font-size: 1.6rem;
        font-weight: 500;
        line-height: 1.9rem;
        color: var(--grey);
        background-color: var(--just-white);
    }
    ```

3. En la [Clase 16: Detallando estilos de tabla de monedas](https://platzi.com/clases/2030-mobile-first/32314-detallando-estilos-de-tabla-de-monedas/), en esta clase detallamos algunos estilos de la tabla que nos faltaban, dentro de los cuales añadimos el icono de la moneda cuando sube y baja.
    ```css
    .main-currency-table, .main-commissions-table {
        width: 70%;
        min-width: 235px;
        max-width: 500px;
        height: 360px;
        margin: 0 auto;
        font-family: 'Inter', sans-serif;
    }
    .main-currency-table .currency-table--title {
        margin-bottom: 15px;
        font-size: 1.8rem;
        font-weight: bolder;
        line-height: 2.3rem;
        color: var(--bitcoin-orange);
    }
    .currency-table--container, .commissions-table--container {
        width: 90%;
        min-width: 230px;
        max-width: 300px;
        height: 250px;
        margin: 0 auto;
    }
    .currency-table--container table, .commissions-table--container table {
        width: 100%;
        height: 100%;
    }
    .currency-table--container td, .commissions-table--container td {
        font-size: 1.6rem;
        font-weight: 500;
        line-height: 1.9rem;
        color: var(--grey);
        background-color: var(--just-white);
    }

    .currency-table--container .table__top-left, .commissions-table--container .table__top-left {
        border-radius: 15px 0 0 0;
    }
    .currency-table--container .table__top-right, .commissions-table--container .table__top-right {
        border-radius: 0 15px 0 0;
    }
    .currency-table--container .table__bottom-left, .commissions-table--container .table__bottom-left {
        border-radius: 0 0 0 15px;
    }
    .currency-table--container .table__bottom-right, .commissions-table--container .table__bottom-right {
        border-radius: 0 0 15px 0;
    }
    .currency-table--container .table__right,.commissions-table--container .table__right {
        font-size: 1.4rem;
        font-weight: normal;
        line-height: 1.7rem;
        color: #757575;
    }
    .currency-table--container .down {
        display: inline-block;
        width: 15px;
        height: 15px;
        margin-left: 10px;
        background-image: url("./assets/icons/trending-down.svg");
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
    }
    .currency-table--container .up {
        display: inline-block;
        width: 15px;
        height: 15px;
        margin-left: 10px;
        background-image: url("./assets/icons/trending-up.svg");
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
    }

    .main-commissions-table .commissions-table--title {
        margin-bottom: 15px;
        font-size: 1.8rem;
        font-weight: bolder;
        line-height: 2.3rem;
        color: #1A9AF7;
    }
    ```

4. En la [Clase 17: Finalizando estilos de tabla de monedas](https://platzi.com/clases/2030-mobile-first/32315-finalizando-estilos-de-tabla-de-monedas/), en esta clase finalizamos los estilos de la tabla de moneda.
    ```css
    .currency-table--date {
        width: 190px;
        height: 30px;
        margin: 0 auto;
        margin-top: 15px;
        padding: 8px;
        background-color: var(--soft-orange);
        border-radius: 8px;
    }
    .currency-table--date p, .commissions-table--date p {
        font-size: 1.2rem;
        font-weight: 300;
        line-height: 1.5rem;
        color: var(--warm-black);
    }
    .commissions-table--date {
        width: 190px;
        height: 30px;
        margin: 0 auto;
        margin-top: 15px;
        padding: 8px;
        background-color: #E7F5FF;
        border-radius: 8px;
    }
    ```

    ***Nota: Tener cuidado con la herencia de algunas propiedades que nos pueden afectar nuestros estilos (Conflicto de herencia), hay que identificarlos y darles solucion, el problema es que la especificidad de `.currency-table--date p` es igual a la especificidad de `.main-exchange-container p`, y lo unico para solucionarlo es agregarle a `.currency-table--date p` el grosor de la letra que estamos buscando, por lo que estos estilos fueron los ultimos en escribirse tienen predominancia sobre `.main-exchange-container p`.***

<br>

## Sección beneficios

5. En la [Clase 18: Estructura base de la sección de beneficios](https://platzi.com/clases/2030-mobile-first/32317-estructura-base-de-la-seccion-de-beneficios/), comenzamos la maquetación en html de la seccion de beneficios que va dentro del `<main>`.
    ```html
    <section class="main-product-detail">
        <span class="product-detail--batata-logo"></span>
        <div class="product-detail--title">
            <h2>Creamos un producto sin comparación.</h2>
            <p>Confiable y diseñado para su uso diario.</p>
        </div>
        <section class="product-cards--container">
            <article class="product-datail--card">
                <span class="clock"></span>
                <p class="product--card-title">Tiempo real</p>
                <p class="product--card-body">Nuestro API toma información minuto a minuto sobre las tasas que más determinan el comportamiento.</p>
            </article>
        </section>
    </section>    
    ```

6. En la [Clase 19: Estilos de la sección de beneficios](https://platzi.com/clases/2030-mobile-first/32318-estilos-de-la-seccion-de-beneficios/), vamos a darle estilos al maquetado de la sección beneficios.
    ```css
    .main-product-detail {
        position: relative;
        width: 100%;
        min-width: 320px;
        height: auto;
        padding: 20px 10px;
        background-color: var(--warm-black);
    }
    .product-detail--batata-logo {
        position: absolute;
        width: 40px;
        height: 25px;
        top: -10px;
        left: calc(50% - 20px);
        background-image: url("./assets/icons/batata-icon.svg");
    }
    .product-detail--title {
        width: 90%;
        min-width: 288px;
        height: auto;
        margin: 0 auto;
        margin-top: 50px;
        text-align: center;
    }
    .product-detail--title h2 {
        margin-bottom: 20px;
        font-size: 2.4rem;
        font-weight: bold;
        line-height: 2.6rem;
        color: var(--just-white);
    }
    .product-detail--title p {
        margin-bottom: 20px;
        font-size: 1.4rem;
        font-weight: 500;
        line-height: 1.8rem;
        color: #808080;
    }
    ```

    ***Nota: Hacemos uso de calc() en css para poder calcular el centro de nuestro espacio donde irá nuestra imagen de batata-icon, esto toma como refrencia tambien el width de nuestra imagen que es `width: 40px;`, siendo la mitad de la imagen 20px, de hay los valores de `left: calc(50% - 20px);`***

7. En la [Clase 20: Maquetando tarjetas de beneficios](https://platzi.com/clases/2030-mobile-first/32320-maquetando-tarjetas-de-beneficios/), ahora vamos a darle estilos a las tarjetas que van dentro de la sección beneficios para terminar esta vista.
    ```css
    .product-detail--card {
        width: 90%;
        min-width: 288px;
        max-width: 400px;
        height: auto;
        margin: 15px auto;
        padding: 15px;
        background-color: var(--black);
        border-radius: 5px;
        box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.16);
    }
    .product-detail--card .icon-card {
        display: inline-block;
        width: 24px;
        height: 24px;
        margin-bottom: 10px;
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
    }
    .clock {
        background-image: url("./assets/icons/clock.svg");
    }
    .eye {
        background-image: url("./assets/icons/eye.svg");
    }
    .dollar {
        background-image: url("./assets/icons/dollar-sign.svg");
    }
    .check {
        background-image: url("./assets/icons/check-circle.svg");
    }
    .product--card-title {
        margin-bottom: 15px;
        font-size: 1.8rem;
        font-weight: bold;
        line-height: 1.8rem;
        color: var(--just-white);
    }
    .product--card-body {
        font-size: 1.4rem;
        font-weight: 500;
        line-height: 1.8rem;
        color: #808080;
    }
    ```

## Dia 4

## Sección beneficios - Una anotación importante

***Nota: si te encontraste con un problema de contenido de las tarjetas, que el contenido se desborda de la tarjeta esta es una forma de solucionarlo: Al colocarle el height de la tarjeta en px estamos limitando el tamaño de esta tarjeta y no se tiene enciuenta el contenido para arreglar esto hay que colocar en vez de height `min-height: 150Px`.*** 

## Sección Comodín

Lleva una sola imagen y un titulo

1. En la [Clase 21: Maquetando sección comodín](https://platzi.com/clases/2030-mobile-first/32321-maquetando-seccion-comodin/), realizamos el maquetado en html y los estilos en CSS de loq ue llamamos seccion comodín que solo tiene una imagen y un titulo.
    ```html
    <section class="bitcoin-img-conatiner">
        <h2>Conócelo hoy.</h2>
    </section>
    ```

    ```css
    .bitcoin-img-conatiner {
        width: 100%;
        min-width: 320px;
        height: 50vh;
        background-image: url("./assets/imgs/bitcoinbaby2x.jpg");
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;
        text-align: center;
    }
    .bitcoin-img-conatiner h2 {
        padding-top: 60px;
        font-size: 2.4rem;
        font-weight: bold;
        line-height: 2.6rem;
        color: var(--just-white);
    }
    ```

## Sección Planes

2. En la [Clase 22: Estructura de sección de planes](https://platzi.com/clases/2030-mobile-first/32322-estructura-de-seccion-de-planes/), realizamos la sección donde se muestra la info sobre los planes, en esta sección encontramos tres tarjetas con un slice.
    ```html
    <section id="plans" class="main-plans-container">
        <div class="plans--title">
            <h2>Escoge el plan que mejor se ajuste a ti.</h2>
            <p>Cualquier plan te da acceso completo a nuestra plataforma.</p>
        </div>
        <section class="plans-container--slider">
            <article class="plans-container--cards">
                <p>Recomendado</p>
                <div>
                    <h3>Pago Anual</h3>
                    <p><sup>$</sup> 99</p>
                    <p>*Ahorras $129 comparado al plan mensual.</p>
                    <button>Escoger este <span>i</span></button>
                </div>
            </article>
        </section>        
    </section>
    ```

    ***Nota: colocar `<section id="plans">` a la sección planes para poder vincularlo con el boton que realizamos al principio de conoce nuestros planes con la etiqueta anchor `<a href="#plans" class="header--button">Conoce Nuestros Planes <span></span></a>`.***

3. En la [Clase 23: Aplicando estilos a sección de planes](https://platzi.com/clases/2030-mobile-first/32323-aplicando-estilos-a-seccion-de-planes/), en esta clase aplicamos los estilos iniciales a la sección planes.
    ```css
    .main-plans-container {
        width: 100%;
        min-width: 320px;
        padding-bottom: 70px;
        text-align: center;
    }
    .plans--title {
        width: 90%;
        min-width: 288px;
        height: auto;
        margin: 0 auto;
        margin-bottom: 50px;
    }
    .plans--title h2 {
        padding-top: 50px;
        font-size: 2.4rem;
        font-weight: bold;
        line-height: 2.6rem;
        color: var(--warm-black);
    }
    .plans--title p {
        padding-top: 30px;
        font-size: 1.4rem;
        font-weight: 500;
        line-height: 1.8rem;
        color: #757575;
    }
    ```

4. En la [Clase 24: Aplicando estilos a las tarjetas de la sección de planes](https://platzi.com/clases/2030-mobile-first/32324-aplicando-estilos-a-las-tarjetas-de-la-seccion-de-/), en esta clase aplicamos los estilos a las tarjetas de esta sección.
    ```html
    <section class="plans-container--slider">
        <article class="plans-container--cards">
            <p class="recommended">Recomendado</p>
            <div class="plan-info-container">
                <h3 class="plan-card--title">Pago Anual<h3>
                <p class="plan-card--price"><sup>$</sup> 99</p>
                <p class="plan-card--saving">*Ahorras $129 comparado al plan mensual.</p>
                <button class="plan-card-ca">Escoger este <span>i</span></button>
            </div>
        </article>
    </section>
    ```

    ```css
    .plans-container--cards {
        position: relative;
        width: 70%;
        min-width: 230px;
        max-width: 300px;
        height: 250px;
        margin: 50px auto 0;
        padding: 0 15px;
        background-color: var(--just-white);
        box-shadow: 0px 4px 8px rgba(89, 73, 30, 0.16);
        border-radius: 15px;
    }
    ```

    ***Nota: `<button class="plan-card-ca">` ca es call to action.***

5. En la [Clase 25: Detallando estilos en tarjetas de planes](https://platzi.com/clases/2030-mobile-first/32325-detallando-estilos-en-tarjetas-de-planes/), en esta clase aplicamos los estilos al contenido de las tarjetas de esta sección.
    ```css
    .plans-container--cards {
        position: relative;
        width: 70%;
        min-width: 230px;
        max-width: 300px;
        height: 250px;
        margin: 50px auto 0;
        padding: 0 15px;
        background-color: var(--just-white);
        box-shadow: 0px 4px 8px rgba(89, 73, 30, 0.16);
        border-radius: 15px;
    }
    .recommended {
        position: absolute;
        width: 120px;
        height: 31px;
        top: -15px;
        left: calc(50% - 60px);
        padding: 6px;
        font-size: 1.2rem;
        font-weight: bold;
        background-color: var(--bitcoin-orange);
        border-radius: 8px;
        color: var(--just-white);
    }
    .plan-card--title {
        padding-top: 30px;
        font-size: 1.4rem;
        font-weight: 500;
        line-height: 1.8rem;
        color: var(--black);
    }
    .plan-card--price {
        padding: 5px 0;
        font-size: 5.2rem;
        font-weight: bold;
        line-height: 5.3rem;
        color: var(--black);
    }
    .plan-card--price sup {
        font-size: 1.2rem;
        font-weight: 500;
        vertical-align: 25px;
    }
    .plan-card--saving{
        font-size: 1.2rem;
        color: #757575;
    }
    ```

6. En la [Clase 26: Aplicando estilos al botón de call to action](https://platzi.com/clases/2030-mobile-first/32326-aplicando-estilos-al-boton-de-call-to-action/), en esta clase aplicamos los estilos al button dentro de la card.
    ```css
    .plan-card-ca {
        width: 150px;
        height: 48px;
        margin-top: 20px;
        background-color: var(--off-white);
        border: 2px solid var(--bitcoin-orange);
        border-radius: 4px;
        font-family: 'DM Sans', sans-serif;
        font-size: 1.4rem;
        font-weight: bold;
        line-height: 1.8rem;
        color: var(--black);
    }
    .plan-card-ca span {
        display: inline-block;
        width: 20px;
        height: 20px;
        background-image: url("./assets/icons/arrow-right.svg");
        vertical-align: text-bottom;
    }
    ```

    ***Nota: La propiedad vertical-align de CSS especifica el alineado vertical de un elemento en línea o una celda de una tabla. `text-bottom` Alinea la parte inferior del elemento con la parte inferior de la fuente del elemento principal.***

7. En la [Clase 27: Scroll horizontal con CSS](https://platzi.com/clases/2030-mobile-first/32327-scroll-horizontal-con-css/), en esta clase realizamos el slider para poder ver las siguientes tarjetas de forma horizontal.
    ```css
    .plans-container--slider {
        display: flex;
        gap: 10px;
        height: 316px;
        overflow-x: scroll;
        overscroll-behavior-x: contain;
        scroll-snap-type: x proximity;
    }
    .plans-container--cards {
        position: relative;
        scroll-snap-align: center;
        width: 70%;
        min-width: 230px;
        max-width: 300px;
        height: 250px;
        margin: 50px auto 0;
        padding: 0 15px;
        background-color: var(--just-white);
        box-shadow: 0px 4px 8px rgba(89, 73, 30, 0.16);
        border-radius: 15px;
    }

    ```

    Nota: 
    1. En elemento padre (.plans-container--slider)
    - ***overflow-x: scroll;*** Establece lo que se muestra cuando el contenido desborda los bordes izquierdo y derecho de un elemento a nivel de bloque. Esto puede ser nada, una barra de desplazamiento o el contenido de desbordamiento.overflow-x.
    - ***overscroll-behavior-x: contain;*** Establece el comportamiento del navegador cuando se alcanza el límite horizontal de un área de desplazamiento.
    - ***scroll-snap-type: x proximity;*** Establece cuán estrictamente se aplican los puntos de ajuste en el contenedor de desplazamiento en caso de que haya uno. 
    X = El contenedor de desplazamiento se ajusta a las posiciones de ajuste solo en su eje horizontal. Proximity = La ventana gráfica de este contenedor de desplazamiento puede descansar en un punto de ajuste si no se desplaza actualmente teniendo en cuenta los parámetros de desplazamiento del agente de usuario. Si se agrega, mueve, elimina o cambia el tamaño del contenido, el desplazamiento de desplazamiento se puede ajustar para mantener el descanso en ese punto de ajuste.
    2. En elemento hijo (.plans-container--cards)
    - ***scroll-snap-align: center;*** La alineación central del área de ajuste de desplazamiento de este cuadro, dentro del puerto de ajuste del contenedor de desplazamiento, es una posición de ajuste en este eje, nos ajusta el elemento al centro.

## Dia 5

## Footer

1. En la [Clase 28: Footer](https://platzi.com/clases/2030-mobile-first/32328-footer/), en esta clase comenzamos la maquetación del footer.


2. antes de iniciar la maquetación del footer arreglamos el ancho de la tarjeta que parecia más ancha que el mockup.

3. Comenzamos la maquetación del footer en HTML:
    ```html <footer>
    <footer>
        <section class="left">
            <ul>
                <li><a href="#">Linkedin</a></li>
                <li><a href="#">Crunchbase</a></li>
                <li><a href="#">Hackernews</a></li>
            </ul>
        </section>
        <section class="right">
            <img src="./assets/imgs/copyright-batata.svg" alt="logo de batatabit 2020" />
        </section>
    </footer>
    ```
4. Ahora aplicamos los estilos en CSS:
    ```css
    footer {
        display: flex;
        width: 100%;
        min-width: 320px;
        height: 150px;
        background-color: var(--bitcoin-orange);
    }
    footer section {
        display: flex;
        width: 50%;
        justify-content: center;
        align-items: center;
    }
    footer .left ul {
        font-size: 1.4rem;
        font-weight: 500;
        line-height: 1.8rem;
        list-style: none;
    }
    .left li {
        margin: 10px 0;
    }
    .left a {
        text-decoration: none;
        color: var(--just-white);
    }
    ```


5. En la [Clase 29: Aplicando media queries](https://platzi.com/clases/2030-mobile-first/32329-aplicando-media-queries/), comenzamos a agregar los estilos por medio de media queries, que nos permitirán ver nuestro diseño en laptop y otros dispositivos.

6. Creamos una carpeta "CSS" para allí agregar los archivos de los estilos segun el tamaño del dispositivo. Creamos el primer archivo "tablet.css".

7. Ahora en nuestro archivo "index.html", agregamos las nuevas paginas de estilos por medio de `<link>`, posicionandolos despues del link que nos llama style.css.
`<link rel="stylesheet" href="./css/tablet.css" media="(min-width: 930px)">`
***Nota: Con la regla de min-width le estamos diciendo al navegador que descarge esos estilos de la hoja de estilos "tablet.css" tan pronto llegue a ese ancho de pantalla de 930px.***

8. Comenzamos a trabajar los estilos en el archivo "tablet.css" para adaptar nuestros estilos a tamaño de tablet.
    ```css
    .main--tables-container {
        display: flex;
        width: 930px;
        margin: 0 auto;
    }
    .product-cards--container {
        display: flex;
        flex-wrap: wrap;
        width: 930px;
        margin: 0 auto;
    }
    ```

    ***Nota: Siempre por buenas prácticas debemos comenzar un proyecto "mobile first" por que como podemos darnos cuenta, los estilos que tuvimos que añadir fueron muy pocos, en cambio cuando realizamos primero el diseño para desktop hay muchas más variables que no tuvimos en cuenta y así se ingrementan nuestros estilos.***

## Medicion de Producto final - LightHouse

1. En la [Clase 30: Análisis con Lighthouse](https://platzi.com/clases/2030-mobile-first/32330-analisis-con-lighthouse/), utilizamos la herramienta lightHouse para medir accesibilidad, buenas practicas, performance, progresive web app, y demas cosas que nos permiten ver que cosas podemos mejorar en nuestro producto.

    ***Nota: Como desarrollador hay que medir lo que se hace, por que no se puede mejorar lo que no se mide.***

2. Para encontrar lightHouse, vamos a nuestro navegador, abrimos la consola y en la flechita de siguiente en encontramos lightHouse, esta herramienta ya hace parte de las herramientas del navegador de google Chrome.

3. Una vez adentro de "LightHouse" hay varias cosas que podemos medir:
    - Performance: Es la velocidad, cuanto tiempo se tarda en renderizar el proyecto.
    - Best practices
    - Accessibility

    Realizamos estas pruebas para mobile y para desktop.

    ***Nota: Un puntaje mayor a 60% es bueno pero se puede mejorar, ademas no hay que obsesionarse con estos puntajes, hay cosas en cuanto a performance que influyen como la velocidad de nuestra conexion a internet.***

4. Por último y para terminar el proyecto arreglaremos algunos estilos y crearemos scroll donde se necesita.

5. Primero realizamos el scroll horizontal de la sección exchange, para esto decidí modificar en el html los contenedores de las tarjetas, quedando así:
    ```html
    <section class="main--tables-container">
        <div class="main-currency-table">
            <div id="currency--table" class="currency--table">
                <p class="currency-table--title">Monedas</p>
                <div class="currency-table--container">
                    <table>
                        <tr>
                            <td class="table__top-left">Bitcoin</td>
                            <td class="table__top-right table__right">$ 1.96 <span class="down"></span></td>
                        </tr>
                        <tr>
                            <td>Ethereum</td>
                            <td class="table__right">$ 0.07 <span class="up"></span></td>
                        </tr>
                        <tr>
                            <td>Ripple</td>
                            <td class="table__right">$ 2.15 <span class="down"></span></td>
                        </tr>
                        <tr>
                            <td class="table__bottom-left">Stellar</td>
                            <td class="table__bottom-right table__right">$ 4.96 <span class="down"></span></td>
                        </tr>
                    </table>
                </div>
                <div class="currency-table--date">
                    <p><b>Actualizado:</b> 19 Julio 23:45</p>
                </div>
            </div>
            <div class="right-icon-container">
                <a href="#commission--table">
                    <img src="./assets/icons/dropdown-right.svg" alt="drop right icon">
                </a>
            </div>
        </div>

        <div class="main-commissions-table">
            <div class="left-icon-container">
                <a href="#currency--table">
                    <img src="./assets/icons/dropdown-left.svg" alt="drop left icon">
                </a>
            </div>
            <div id="commission--table" class="commission--table">
                <p class="commissions-table--title">Comisiones</p>
                <div class="commissions-table--container">
                    <table>
                        <tr>
                            <td class="table__top-left">Bitrade</td>
                             <td class="table__top-right table__right">$ 1.96</td>
                        </tr>
                        <tr>
                            <td>Bitpreco</td>
                            <td class="table__right">$ 13.07</td>
                        </tr>
                        <tr>
                            <td>Novadax</td>
                            <td class="table__right">$ 13.15</td>
                        </tr>
                        <tr>
                            <td class="table__bottom-left">Coinext</td>
                            <td class="table__bottom-right table__right">$ 14.96</td>
                        </tr>
                    </table>
                </div>
                <div class="commissions-table--date">
                    <p><b>Actualizado:</b> 19 Julio 23:45</p>
                </div>
            </div>
        </div>
    </section>            
    ```

6. Ahora vamos a arreglar los estilo que se necesiten en el archivo "styles.css":
    ```css
    /* Estilos modificados para mejorar las vistas de los sliders */
    .main--tables-container {
        display: flex;
        gap: 50px;
        overflow-x: scroll;
        overscroll-behavior-x: contain;
        scroll-snap-type: x proximity;
    }
    .main-currency-table, .main-commissions-table {
        display: flex;
        scroll-snap-align: center;
        /* width: 70%; */
        /* min-width: 235px; */
        /* max-width: 500px; */
        height: 360px;
        margin: 0 auto;
        font-family: 'Inter', sans-serif;
    }
    /* Estilos añadidos para sliders faltantes */
    .currency--table{
        padding-left: 10px;
    }
    .commission--table {
        padding-right: 20px;
    }
    .right-icon-container, .left-icon-container {
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 30px;
    }
    ```

7. Ahora realizaremos los arreglos en los estilos que se necesiten para que se vean bien en tablet y desktop, en el archivo "tablet.css":
    ```css
    /*? Estilos añadidos para sliders faltantes */
    .main--tables-container, .plans-container--slider {
        overflow: hidden;
    }
    .right-icon-container, .left-icon-container {
    display: none;
    }
    /*? Estilos añadidos para footer */
    footer .left {
        width: 70%;
    }
    footer .left ul {
        display: flex;
        gap: 100px;
    }
    ```

8. Despues de terminada toda la aplicación corremos nuevamente el test de "LightHouse":

    ***Para Mobile***
    - Performance: 75%
    - Accessibility: 96%
    - Best Pactice: 100%
    
    ***Para Desktop***
    - Performance: 99%
    - Accessibility: 96%
    - Best Pactice: 100%
