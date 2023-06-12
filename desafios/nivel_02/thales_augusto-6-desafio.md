###Dentro do banco-dados.php:

~~~php

<?php
    $servidor = "localhost";
    $usuario  = "root";
    $senha    = "";
    $banco    = "ex.6";

    try {
        $pdo = new PDO("mysql:host={$servidor};dbname={$banco};port=3306;charset=utf8;",$usuario,$senha);
    } catch (Exception $e) {
        echo "<p>Erro ao tentar conectar</p>";
        echo $e->getMessage();
    }
?>
~~~

###Também quis confirmar pra ver se realmente foi conectado, então fiz um index.php:

~~~php

<?php 
    require "./banco-dados.php";

    $sql = "select frase from mensagem";
    $consulta = $pdo->prepare($sql);
    $consulta->execute();

    $dados = $consulta->fetch(PDO::FETCH_OBJ);

    var_dump($dados);
?>

~~~