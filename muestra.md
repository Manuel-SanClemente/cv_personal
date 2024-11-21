//Kotlin

[Repositorio]<https://github.com/Manuel-SanClemente/e-8>
[Pagina](https://manuel-sanclemente.github.io/e-8/)


````
fun main() {
    // se introduce la entrada (recuerda, un string es más o menos un Array de Char)
    var entrada= readln()
    while (entrada != "FIN") {

        // se establecen contadores
        var N:Double =0.0
        var R:Double =0.0
        var B:Double =0.0
        var C:Double =0.0
        var S:Double =0.0

        // Se recorre la lista y se cuentan las apariciones de cada letra
        // Ten en cuenta esto: la variable "i" es la que recorre cada caracter de la entrada
        // Si esta equivale una de las posibilidades de abajo, esta suma los contadores
        for (i in entrada) {
            when (i) {
                'N' -> N++
                'R' -> R++
                'B' -> B++
                'S' -> S++
                'C' -> C++
                ' ' -> continue  // Ignorar espacios
            }
        }

        // con las letras contadas, se multiplican los contadores por sus cantidades (mira el comentario de abajo)
        var Nx:Double=N*1.0
        var Rx:Double=R*4.0
        var Bx:Double=B*2
        var Cx:Double=C*0.50
        var Sx:Double=S*0.25

        // se suman todas las cantidades
        var resultado=Nx+Rx+Bx+Cx+Sx

        // se comparan los resultados
        if (resultado==4.0) { println("CORRECTO") }
        else if (resultado<4.0) { println("DEFECTO") }
        else { println("EXCESO") }

        entrada= readln()
    }
}
````

//HTML

````
<html>

<head>
    <meta charset="UTF-8">
    <title>Vegetables</title>
    <link rel="icon" href="img/favicon.ico">
    <style>
        body{
            margin: 0%;
            display: flex;
            flex-direction: column;
            justify-content: space-around;
            align-items: center;
        }

        header img,
        footer img {
            width: 100%;
        }

        main ul {
            display: flex;
            flex-wrap: wrap;
            margin: 10 auto;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 5px;
            list-style: none;
            gap: 20px;
        }

        main ul li {
            background-color: #E0E6A6;
            border: 3px solid #D8DF8F;
            border-radius: 20px;
            padding: 10px;
        }

        main ul li p {
            font-size: 2.5vh;
            color: #008528;
        }

        main ul li img {
            height:20vh;
            border: 3px solid #008528;
            border-radius: 20px;
        }
    </style>
</head>

<body>

    <header>
        <img src="img/banner1.png" alt="">
    </header>
    <main>
        <ul>
            <li><img src="img/potato.png">
                <p>Potato</p>
            </li>
            <li><img src="img/garlic.png">
                <p>Garlic</p>
            </li>
            <li><img src="img/chili-pepper.png">
                <p>Chili pepper</p>
            </li>
            <li><img src="img/bell-pepper2.png">
                <p>Bell pepper</p>
            </li>
            <li><img src="img/mushroom.png">
                <p>Mushroom</p>
            </li>
            <li><img src="img/eggplant2.png">
                <p>Eggplant</p>
            </li>
            <li><img src="img/carrot.png">
                <p>Carrot</p>
            </li>
            <li><img src="img/tomato.png">
                <p>Tomato</p>
            </li>
            <li><img src="img/cucumber.png">
                <p>Cucumber</p>
            </li>
        </ul>
    </main>
    <footer>
        <img src="img/banner2.png" alt="">
    </footer>

</body>

</html>
````
