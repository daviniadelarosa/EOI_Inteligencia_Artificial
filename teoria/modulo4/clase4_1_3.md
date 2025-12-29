# Ejemplo en Python

Vamos a usar un modelo pre-entrenado específico para español. Utilizaremos la librería pysentimiento (basada en Transformers), que es mucho más precisa para el sarcasmo y las variantes del español que las librerías clásicas como TextBlob.

## 1. El Dataset de Prueba (Copia esto a un txt o excel, es un csv)
Crea un archivo llamado comentarios_pyme.xlsx o txt con una sola columna llamada "Comentario". Incluye estos ejemplos variados para demostrar que la IA no solo lee palabras sueltas:

```csv
Comentario,Resultado Esperado
"El producto es increíble, pero el repartidor fue muy grosero.",NEG/NEU (Detecta el peso de la logística)
"Gracias por ignorar mi correo durante tres días, excelentes profesionales.",NEG (Detecta Sarcasmo)
"No es lo más barato del mercado, pero la calidad compensa cada euro.",POS (Entiende el matiz de valor)
"Me llegó el color equivocado, pero me lo resolvieron en 10 minutos.",POS (Valora la resolución sobre el error)
"Pues nada, otra vez el paquete roto.",NEG (Detección de frustración)
```

## 2. El Script de Python
Este script lee el Excel, analiza el sentimiento, calcula la "probabilidad" (cuanto de segura está la IA del resultado esperado) y guarda un nuevo Excel con los resultados: 

```py
import pandas as pd
from pysentimiento import create_analyzer

# 1. Cargamos el analizador específico para español
# Este modelo está entrenado con lenguaje real (redes sociales)
analyzer = create_analyzer(task="sentiment", lang="es")

def ejecutar_demo(input_file, output_file):
    print("--- Iniciando análisis de sentimiento para la Pyme ---")
    
    # 2. Leer los datos
    df = pd.read_excel(input_file)
    
    # 3. Función para aplicar el modelo
    def obtener_sentimiento(texto):
        # El modelo devuelve: POS (positivo), NEU (neutro), NEG (negativo)
        resultado = analyzer.predict(texto)
        return pd.Series([resultado.output, max(resultado.probas.values())])

    # 4. Aplicar análisis
    df[['Sentimiento', 'Confianza']] = df['Comentario'].apply(obtener_sentimiento)
    
    # 5. Guardar resultados
    df.to_excel(output_file, index=False)
    print(f"--- Análisis finalizado. Resultados guardados en: {output_file} ---")

# Para ejecutarlo:
# ejecutar_demo('comentarios_pyme.xlsx', 'resultado_sentimiento.xlsx')
```

## 3. Puntos clave para tu "Pitch" en la Demo
Veamos el valor que tiene para marketing esto: 

- Más allá de las Palabras Clave: Veamos por ejemplo el sarcasmo ("excelentes profesionales"), la IA entiende el contexto, no solo busca palabras en una lista.

- Escalabilidad: "Si hoy recibes 10 comentarios, los lees tú. Si mañana lanzas una campaña y recibes 1.000, este script te dice en poco tiempo cuáles requieren una respuesta urgente del equipo de atención al cliente".

- Matriz de Confianza: La columna "Confianza" permite filtrar. Solo se deben  revisar manualmente, por ejemplo, aquellos donde la IA tenga una confianza menor al 60%, automatizando el resto con seguridad y/o revisiones menos habituales.

## 4. Ejercicio propuesto
Escribe una queja "disfrazada" de elogio y pásala por el script. Es una buena forma de ver que el script funciona.
