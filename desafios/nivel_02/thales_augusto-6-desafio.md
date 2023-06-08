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

###Também quis confirmar pra ver se realmente foi conectado:

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