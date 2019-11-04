# Código fuente del evento de "Inteligencia Artificial para el reconocimiento facial en Python"

El archivo .html exportado muestra el resultado de toda la ejecución del código para aquellos que busquen echar un vistazo rápido a los conocimiento que presentan, o copiar slots de código para sus proyectos.

Para aquellos que quieran montarlo en su máquina local pueden seguir las instrucciones de los siguientes apartados.

## Cosas a tener en cuenta para ejecutar el proyecto
1. Se debe saber cómo crear entornos virtuales con Conda a partir de un fichero yml
2. OpenCV puede dar problemas a la hora de instalar desde Conda (sobre todo con la integración de la web-cam). Se debe buscar el repositorio que corresponda a nuestro SO, siempre teniendo en cuenta la versión de Python especificada en el fichero yml.

## Cómo lanzar el proyecto
1. Clonar en tu máquina el repositorio
2. Instalar conda (gestor de paquetes cientificos de Python). Con la instalación de Conda vendrá Jupyter también.
3. Instalar con Conda el entorno virtual de Python extraído en el fichero fa-workshop01.yml. Se han detectado algunos issues con algunas versiones de OS. Está extraido de un MacOS. La instalación en otros OS no debería ser problema instalando una a una las dependencias antes de correr el notebook.
4. Establecer Tensorflow como el backend de Keras con el siguiente comando. 

    ```set KERAS_BACKEND=tensorflow``` para Windows
    ```KERAS_BACKEND=tensorflow``` para Limux/MacOS
    
    Para comprobar que todo está configurado correctamente:
        ```python -c "from keras import backend"```


5. Activar el entorno de desarrollo y hacer disponible este entorno virtual para que pueda ser ejecutado desde Jupyter. Se puede encontrar cómo hacerlo en [este enlace](https://help.pythonanywhere.com/pages/IPythonNotebookVirtualenvs/).
6. Descomprimir los dos archivos .zip que se encuentran en el directorio data
7. Ejecutar el siguiente comando desde el directorio raíz del proyecto
    ```jupyter notebook```
8. Seleccionar nuestro entorno virtual para que el kernel de Jupyter ejecute el código usando nuestras librerías.


## Autores

**Carlos Tarquino** 

Udacity attribution as the original creators of this project in their full AI Nanodegree program.

Todo el código es libre de ser distribuido y modificado bajo la licencia Apache v2.0