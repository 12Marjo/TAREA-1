echo "Tarea 1"
cd ..
cd Saavedra2013
echo "Le ponemos head -n 1 para ver la primera fila a continuación borramos los espacios entre filas y el espacio final"
echo "Si solo usamos head veriamos las primeras 10 filas por lo tanto condicionamos a ver desde la primera fila" 
echo "usando cd../../ volvemos al directorio raíz"
echo "cuando usamos wc-l contamos solo las líneas del archivo"
echo "usamos cat para imprimir el contenido de los archivos sin embargo es más especifico"
head -n 1 ../Saavedra2013/n10.txt | tr -d " " | tr -d "\n" | wc -c

