# Proyecto para Curso Práctico Responsive Design Platzi 👩‍💻 🤖 👀

## Documentación y recursos entregados por Platzi

- Coach: Diego De Granda

- [Wireframes o Mockups en Figma](https://www.figma.com/file/sMmlQaZldfDcLERYYWe6h4/Bata-Bit)

- [Diseño Mobile](https://www.figma.com/proto/sMmlQaZldfDcLERYYWe6h4/Bata-Bit?node-id=44%3A594&scaling=scale-down)



## Paso a paso desarrollo del proyecto🏃‍♀️📝🏃‍♀️

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