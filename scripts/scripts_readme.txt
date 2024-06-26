#Documento que contiene el script para realizar la filogenia de HSP70 en Trypanosoma cruzi 

1. Datos 
# Secuencias en formato FASTA extraídas desde NCBI 
# Secuencias ya alineadas sacadas de NCBI
# Guardar el archivo formato FASTA

2. Árbol Filogenético
# Mover los datos de las secuencias a la carpeta data
mv sequence.txt /c/Users/usuario/OneDrive/Escritorio/BIOINFORMÁTICA/ProyectoFinalBio24/data 
# Ejecutar IQTREE 
./iqtree2.exe -h
# Construcción del árbol 
# Ejecutar IQ-TREE con el archivo de alineamiento
./iqtree2.exe -s "$ALIGNMENT_FILE" -m MFP -bb 1000 -alrt 1000
# Verificar los archivos generados
echo "Archivos generados"

3. Archivos 
# Archivos generados importantes
Secuencias
Secuencias alineadas
tree
tree: foto del árbol 

4. Visualización del árbol 
# Usar FigTree:
Subir al FigTree mediante File y Open Trypanosoma_cruzi_iqtree.treefile
Podra visualizar en la plataforma de FigTree el arbol generado de las 24 conjuntos de secuencias extraidos y alineados de NCBI.
