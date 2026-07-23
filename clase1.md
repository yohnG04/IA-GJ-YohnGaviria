# Actividad de Clase: Analizando Agentes de IA con Hugging Face Spaces

## Objetivo

Explorar aplicaciones reales de Inteligencia Artificial en **Hugging
Face Spaces** y analizarlas desde la perspectiva de los **agentes
racionales**.

Al finalizar la actividad, los estudiantes deberán ser capaces de:

-   Identificar los componentes **PEAS** de un agente.
-   Clasificar las propiedades del entorno.
-   Proponer qué tipo de programa de agente podría implementarse detrás
    del sistema.
-   Justificar sus respuestas.

------------------------------------------------------------------------

## Instrucciones

1.  Ingresen a **https://huggingface.co/spaces**.
2.  Exploren diferentes Spaces.
3.  Seleccionen uno que les parezca interesante.
4.  Interactúen con el sistema durante algunos minutos.
5.  Completen la siguiente ficha de análisis.

------------------------------------------------------------------------

# Ficha de análisis

## 1. Nombre del Space

**Nombre:** 🎨 Z-Image-Turbo

**Enlace:** https://huggingface.co/spaces/mrfakename/Z-Image-Turbo

------------------------------------------------------------------------

## 2. ¿Qué hace el agente?

Es un sistema de inteligencia artificial que genera imagenes a partir de 
una descripción brindada por el usuario. Puedes modificar el tamaño de la
imagen por pixeles y el numero de pasos de inferencia.

------------------------------------------------------------------------

## 3. Análisis PEAS

  Elemento          Respuesta
  ----------------- ----------------------------------------------------
  **Performance**   ¿Qué significa que el agente haga bien su trabajo?
  Genera imagenes a partir del texto ingresado con rapidez y coherencia.
  **Environment**   ¿Con qué interactúa el agente?
  El agente interactua con el usuario, con la interfaz web, el modelo de IA.
  **Actuators**     ¿Qué acciones produce?
  Genera las imagenes, muestra el progreso de generacion y responde a los 
  cambios que haya hecho el usuario, sea en tamaño o en el numero de pasos 
  de inferencia.
  **Sensors**       ¿Qué información recibe como entrada?
  Recibe el prompt, numero de pasos de inferencia y cambios en el tamaño 
  ingresados por el usuario.

------------------------------------------------------------------------

## 4. Clasificación del entorno

Complete la siguiente tabla y justifique brevemente cada respuesta.

  Propiedad      Clasificación     Justificación
  -------------- ----------------- ---------------
  Observable     Total              Solo conoce lo que el usuario le proporciona
                                    pero no conoce completamente la intencion del usuario.
  Determinista   No                 Porque produce imagenes diferentes cuando cambia de semilla 
                                    y hay procesos aleatorios.        
  Episódico      Sí                 Cada solicitud es independiente de las anteriores.          
  Estático       Sí                 Mientras se procesa una imagen el entorno no cambia.
  Discreto       No                 Las imagenes estan en espacios continuos (pixeles, colores).
  Conocido       Sí                 Las acciones estan definidas por el modelo.

------------------------------------------------------------------------

## 5. ¿Qué tipo de programa de agente creen que es?

Agente basado en objetivos porque el objetivo del sistema es generar una imagen que represente
de la mejor manera lo que el usuario ingresó. Analiza el texto y da el resultado orientado a cumplir el objetivo.

> **Importante:** No existe una única respuesta correcta. Lo importante
> es justificar la elección a partir del comportamiento observado.

------------------------------------------------------------------------

# Discusión en clase

Después de las presentaciones, discutiremos preguntas como:

-   ¿Dos Spaces diferentes pueden compartir el mismo tipo de entorno?
-   ¿Es posible saber con certeza qué tipo de agente implementa un Space
    únicamente observándolo?
-   ¿Qué diferencia existe entre el comportamiento observable de un
    agente y su implementación interna?

------------------------------------------------------------------------

# Reto adicional

Encuentre un Space que pueda clasificarse como:

1.  **Totalmente observable, determinista y episódico.**
2.  **Parcialmente observable, estocástico y secuencial.**

Justifique su respuesta.

------------------------------------------------------------------------

# Rúbrica (10 puntos)

| Criterio | Puntos |
|-----------|:------:|
| Descripción correcta del Space | 2 |
| Identificación de PEAS | 3 |
| Clasificación del entorno | 3 |
| Justificación del tipo de agente | 2 |
| **Total** | **10** |

------------------------------------------------------------------------


