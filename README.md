# Trabalho-do-Bill-04-04
grupo: Amyr, João Paulo, Gabriel Felipe, Alan/
     Da ponto ai bill :)

<?php
function bubbleSort($array) {
    $n = count($array);
    for ($i = 0; $i < $n - 1; $i++) {
        for ($j = 0; $j < $n - $i - 1; $j++) {
            if ($array[$j] > $array[$j + 1]) {
                // Troca os elementos se estiverem fora de ordem
                $temp = $array[$j];
                $array[$j] = $array[$j + 1];
                $array[$j + 1] = $temp;
            }
        }
    }
    return $array;
}

$array = [8, 6, 3, 0, 5];
echo "Array antes da ordenação:\n";
print_r($array);

echo "\nArray após a ordenação:\n";
$resultado = bubbleSort($array);
print_r($resultado);
?>
