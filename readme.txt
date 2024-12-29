Instrucciones de uso se debe de descargar todo de control panel
la primer grafica de categorias
despues cargar la data de subcategorias y descargar una por una 
cada subcategoria subcategoria son las tablas con porcentaje
(Nota revisar el formato en casillas vacias debe de ser igual al formato descargado)
de lo contrario no funcionara el programa
nota: al cargar level 3 seleccionar semana y crear un diccionario por categoria con su porcentaje 
Para rt explicar subcategorias y cargar ordenes nominativas para todas las cat ‪
nota recordar las categorias que faltan y agregarlas
nota preguntar sobre la clasificacion de las categorias y ver si existe
forma de comparar con un if si la categoria esta y si no esta meterla dentro del
data frame
Nota agregar los iguales por si hay valores wo iguales en todos los ifs
Nota investigar si se puede agregar info al df de categorias faltantes
Hacer prueba de agregar info con este bloque
import pandas as pd

# Crear el DataFrame original
data = {
    "SUB_CATEGORY": ["Discipline", "Early Regret", "Other", "Discipline", "Early Regret", "Other"],
    "Cancel_rate": ["0,37 %", "0,24 %", "0,09 %", "0,34 %", "0,04 %", "0,16 %"],
    "Year": [2024, 2024, 2024, 2024, 2024, 2024],
    "Month": ["December", "December", "December", "December", "December", "December"],
    "Day": [9, 9, 9, 16, 16, 16],
}
df = pd.DataFrame(data)

# Agregar nuevas filas al DataFrame
new_data = {
    "SUB_CATEGORY": ["Discipline", "Early Regret", "Other"],
    "Cancel_rate": ["0,50 %", "0,30 %", "0,20 %"],
    "Year": [2024, 2024, 2024],
    "Month": ["December", "December", "December"],
    "Day": [23, 23, 23],
}

new_df = pd.DataFrame(new_data)

# Concatenar el DataFrame original con las nuevas filas
df = pd.concat([df, new_df], ignore_index=True)

# Mostrar el DataFrame actualizado
print(df)
If categoria en la posicion by day y es igual a la categoria tal entonces agrega la siguiente categoria con valor 0
