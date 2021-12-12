echo "Segunda parte de la tarea"
cd ..
cd Saavedra2013
echo "se pretende  imprimir el numero de columnas y filas para cada red"
echo " creamos un  bucle con el for "
echo "con el bucle tenemos que definir donde queremos trabajar in../Saavedra2013/*.txt acabamos con  * para escoger todos los archivos que terminen con .txt luego acabamos la orden con un punto y coma y con el do  especificamos  que archivos en especifico queremos imprimir por ello usamos el cat para imprimirlos"
echo "número de filas"
for M in ../Saavedra2013/*.txt; do cat $M | wc -l; done
echo "Número de columnas"
for B in ../Saavedra2013/*.txt; do head -n 1 $B | tr -d "\n" | wc -c; done
