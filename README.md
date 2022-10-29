# calculadora
calculadora simples em php e html

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="calculadora" content="width=device-width, initial-scale=1.0">
    <title>CALCULADORA</title>
</head>
<body> 
    <fieldset>
    <h1>
    <stronger> CALCULADORA </stronger>
    </h1>
    <section class="container">
    <form action="calculador.php" class="form" method="POST">
    </br><label for="nome"><strong> 1º valor / </strong></label>
    <label for="nome"><strong> Operação / </strong></label>
    <label for="nome"><strong> 2º valor </strong></label>
    </br>
    </br><input type="number" id="nome" name="num1" size="5" maxlength="5">
    <select name = calcular>
        <option value = "somar"><strong>+</strong></option>
        <option value = "subtrair"><strong>-</strong></option>
        <option value = "multiplicar"><strong>*</strong></option>
        <option value = "dividir"><strong>/</strong></option>
    </select>
    <input type="number" id="nome" name="num2" size="5" maxlength="5">
    </br>
    </br><button type="submit">CALCULAR</button>
    </br>
    </br><label for="nome"><strong>Resultado:</strong></label>
    </br>
    </br><output type="int" id="nome" name="nome" size="5">
    </form>
  </section>
</fieldset>
</body>
</html>

--------------------------------------------------------------------------

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="calculdora" content="width=device-width, initial-scale=1.0">
    <title>CALCULADORA</title>
</head>
<body>
    <?php

    $num1 = 0;
    $num2 = 0;

    $num1 = $_POST ['num1'];
    $num2 = $_POST ['num2'];

    $soma = $num1 + $num2;
    $subtracao = $num1 - $num2;
    $mutipllicacao = $num1 * $num2;
    $divisao = $num1 / $num2;

    ?>
</body>
</html>
