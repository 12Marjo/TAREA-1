# TAREA-1
Primero se crea una carpeta en nuestro escritorio
Creando primero un usuario se logra crear un nuevo repositorio en github.com
Luego de ello copiamos el code del repositorio y lo abrimos con un click izquierdo seleccionando git bash here
Primera tarea
Cd nos permite abrir carpetas por lo que en orden jerárquico y en MI CASO abrí primero documentos (asegurándome con la tecla TAP de estar en lo correcto) luego abro la carpeta de CSB y sucesivamente hasta llegar a la carpeta de Saavedra2013
El cat nos permite ser más exactos para imprimir el contenido de los archivos, le ponemos head -n 1 para ver la primera fila a continuación borramos los espacios entre filas y el espacio final
Si solo usamos head veríamos las primeras 10 filas por lo tanto condicionamos a ver desde la primera fila
cd Documents/CSB-master/unix/data/Saavedra2013
cat ../Saavedra2013/n10.txt | wc –l
head -n 1 ../Saavedra2013/n10.txt | tr -d " " | tr -d "\n" | wc -c
"Segunda parte de la tarea"
cd ..
cd Saavedra2013
Se pretende imprimir el numero de columnas y filas para cada red
Primero se crea un bucle con el for
Con el bucle tenemos que definir donde queremos trabajar in../Saavedra2013/.txt acabamos con * para escoger todos los archivos que terminen con .txt luego acabamos la orden con un punto y coma y con el do especificamos que archivos en especifico queremos imprimir por ello usamos el cat para imprimirlos
"Número de filas"
for M in ../Saavedra2013/.txt; do cat $M | wc -l; done
"Número de columnas"
for B in ../Saavedra2013/*.txt; do head -n 1 $B | tr -d "\n" | wc -c; done
