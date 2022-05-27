
# Ejecutar script desde cmd usando un archivo.
Cuando se tiene un archivo .sql y se debe ejecutar mediante el cmd o consola:
* Si el comando no se ejecuta correctamente, se debe abrir la consola en modo administrador.
  ```sh
  sqlcmd -S myServer\instanceName -i C:\myScript.sql
  ```
  




