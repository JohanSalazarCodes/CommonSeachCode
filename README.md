# CommonSeachCode
Helps me to find quick code i searched and probably  use in future.


# Uso de archivos embebidos en libreria de clases c#
Cuando se tiene una librería de clases que forma parte de una de las capas de un backend, por ejemplo, siguiendo una estructura:
  * Api.
  * BL  -> Contiene archivos como imagenes.
  * DAL.
Para poder acceder a esos archivos desde el BL para realizar alguna accion sobre estos se puede hacer lo siguiente:
  * Se cambia la propiedad del archivo Build Action = Embedded resource 
  * Codigo:
  ```sh
  var assemblys = Assembly.GetExecutingAssembly();
  var stream = assemblys.GetManifestResourceStream($"ProyectoBL.Folder.Imagen.logo.png");
  ```
  
