PASOS PARA CORRER SOLUCION

Ejecutar la solucion mediante fastapi de manera local

1. Se debe de tener instalado PyCharm 2026.1
2. En caso de no tenerlo se descarga https://www.jetbrains.com/es-es/pycharm/download/?section=windows .exe para windows
3. Una vez instalado se abre la interfaz y se crea el proyecto
4. Se abre una terminal dentro del proyecto creado y se instalan
5. pip install fastapi
6. pip install "uvicorn[standard]"
7. pip freeze > requirements.txt
8. Una vez realizado estas instalaciones se crea archivo main.py
9. El codigo lo dejo anexado en el repositorio NombreMain: 09.-EndPoint_main_event_daily_stats.txt se abre el txt se copea el codigo y se pega en main.py
10. En la carpeta .venv del proyecto se arrastra el archivo 08.-EndPoint_event_daily_stats.json para poder leer los datos, se encuentra en el repositorio
11. Para ejecutar la solucion en la terminal abierta anterior mente se ejecuta
12. uvicorn main:app --reload
13. Una vez ejecutado muestra una url en la terminal con un puerto ejemplo http://127.0.0.1:8000
14. Se pega la url en el navegador, y para visualizar el endpoint se le agrega /docs en la url http://127.0.0.1:8000/docs
15. Una vez abierto el endpoint, se puede ver Get y el nombre
16. Se puede ejecutar de dos maneras
17. Directamente en la interfaz dando clic en Try it out o poniendo la url agregndo el nombre del endpoint /Buscar http://127.0.0.1:8000/Buscar
18. El parametro que recibe es ua fecha, el cual esper el formato YYYY-MM-DD
19. En la interfaz se agrega el parametro ejemplo 2025-12-01 y se le da en ejecutar
20. En la url se le agrega el parametro despues del nombre del endpoint http://127.0.0.1:8000/Buscar/2025-12-01

DEPENDENCIAS
1. PyCharm 2026.1
2. Archivo json 08.-EndPoint_event_daily_stats.json
3. Azure Databricks

DESICIONES TECNICAS
1. Ninguna desicion importante, solo que lo trabaje en azure databricks, todo el codigo lo subire en este repositorio

QUE HARIAS SI TUVIERA MAS TIEMPO
1. Implemetarlo copletamente en la nube (azure, aws, google cloud), aunque se me dificulto un poco por la presion ya que las pruebas sulen ser un poco diferente al trabajo cotidiano (hablo de mi persona) porque no se me comparte el resultado esa es la mayor dificultad que tengo.
