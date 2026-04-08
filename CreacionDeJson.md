CREACION Y CORRECCION DE ARCHIVOS JSON EN DATABRICKS

1.- El codigo de creacion lo dejo en el repositorio de Entrega
Archivos JSON

06.-MetricasAnaliticas_event_december_daily.json
08.-EndPoint_event_daily_stats.json

Al crear los archivos json en databricks se crea una carpeta en el cual se puede descargar, antes de ejecutar para guardar el formato json, se le puede agregar el directorio
ejemplo: '/Volumes/testdatabricks/default/datatest/NombreArchivoJson'

Al descargar el archivo.json, se muestra con la siguiente estructura, ejemplo:

{
    "date":"2025-12-01",
    "total_users":59,
    "total_searches":39,
    "total_purchases":31,
    "total_purchased_amount":18674
}
{
    "date":"2025-12-02",
    "total_users":60,
    "total_searches":27,
    "total_purchases":39,
    "total_purchased_amount":20380
}

Una vez teniendo el archivo.json, se le da clic derecho y abrir con bloc de notas

y se hace la correcion, se le agrega corchete al inicio y se le agrega corchete al final, ademas de agregar una coma al final de cada llave que cierra
Ejemplo de correcion:
[
    {
        "date":"2025-12-01",
        "total_users":59,
        "total_searches":39,
        "total_purchases":31,
        "total_purchased_amount":18674
    }
    ,{
        "date":"2025-12-02",
        "total_users":60,
        "total_searches":27,
        "total_purchases":39,
        "total_purchased_amount":20380
    }
]

Una vez terminada la correcion se puede utilizar en el main del endpoint
