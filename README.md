PASOS PARA CORRER SOLUCION

Ejecutar la solucion mediante fastapi de manera local

1. Se debe de tener instalado PyCharm 2026.1
2. En caso de no tenerlo se descarga https://www.jetbrains.com/es-es/pycharm/download/?section=windows .exe para windows
3. Una vez instalado se abre la interfa y se crea el proyecto
4. Se abre una termianl dentro del proyecto creado y se instalan
5. :pip install fastapi
6. :pip install "uvicorn[standard]"
7. :pip freeze > requirements.txt
8. El codigo lo dejo anexado en el repositorio
9. En la carpeta .venv del proyecto se arrastra el archivo event_daily_stats.json para poder leer los datos, se encuentra en el repositorio
10. Para ejecutar la solucioon en la terminal abierta anterior mente se ejecuta
11. :uvicorn main:app --reload
12. Una vez ejecutado muestra una url con un puerto ejemplo http://127.0.0.1:8000
13. Se pega la url en el navegador, y para visualizar el endpoint se le agrega /docs en la url http://127.0.0.1:8000/docs
14. Una vez abierto el endpoint, se puede ver Get y el nombre
15. Se puede ejecutar de dos maneras
16. Directamente en la interfaz dando clic en Try it out o poniendo la url agregndo el nombre del endpoint /Buscar http://127.0.0.1:8000/Buscar
17. El parametro que recibe es ua fecha, el cual esper el formato YYYY-MM-DD
18. En la interfaz se agrega el parametro ejemplo 2025-12-01 y se le da en ejecutar
19. En la url se le agrega el parametro despues del nombre del endpoint http://127.0.0.1:8000/Buscar/2025-12-01

DEPENDENCIAS
1. PyCharm 2026.1
2. Archivo json event_daily_stats.json

DESICIONES TECNICAS
1. Ninguna desicion importante, solo que lo trabaje en azure databricks, todo el codigo lo subire en este repositorio

QUE HARIAS SI TUVIERA MAS TIEMPO
1. Implemetarlo copletamente en la nube (azure, aws, google cloud), aunque se me dificulto un poco por la presion ya que las pruebas sulen ser un poco diferente al trabajo cotidiano (hablo de mi persona) porque no se me coparte el resultado esa es la mayor dificultad que tengo.
