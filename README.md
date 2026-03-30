# Repo para EIEC - DevOps - UNIR

Este repositorio nos servirá para demostrar el uso de Git en la asignatura de EIEC y muchas cosas mas.

---

Los comandos del Makefile funcionarán en Linux y MacOS. En caso de usar Windows, necesitarás adaptarlos o ejecutarlos en una máquina virtual Linux.

## Ejecución

# Directamente utilizando python
python3 main.py <filename> <dup>
  filename: **ruta** al fichero que contiene la lista de palabras, una por línea
  dup: **yes|no**, yes para eliminar palabras duplicadas, no para mantener la lista

# Segun Sistema Operativo y línea de comandos será necesario cambiar el Makefile:

  # En Windows deberá instalarse chocolatey para depués instalarse make antes de poder usarlo
  
  # Cambiar el Makefile para ejecutar make run desde PowerShell en Windows:
  Cambiar `pwd` por "$(CURDIR):/opt/app".

  # Cambiar el Makefile para ejecutar make run desde bash en Linux:
  Cambiar "$(CURDIR):/opt/app" por `pwd`.

# Utilizando docker con palabras por defecto 
  make run

# Utilizando docker pasando el fichero y el parametro para eliminar o no duplicados
make run file=words.txt dup=yes




