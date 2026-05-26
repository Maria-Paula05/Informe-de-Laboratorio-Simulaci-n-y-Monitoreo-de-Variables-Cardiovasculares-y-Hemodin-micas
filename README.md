# Informe de Laboratorio Simulación y Monitoreo de Variables Cardiovasculares y Hemodinámicas

**Universidad Militar Nueva Granada**  
**Programa:** Ingeniería Biomédica  
**Asignatura:** Instrumentación Biomédica y Biosensores  
**Laboratorio:** Simulación y Monitoreo de Variables Cardiovasculares y Hemodinámicas  

**Integrantes:**  
- María Paula Fernández Jiménez 
- Juan Pablo Díaz Rocha
- Jhonathan Guevara 

**Docente:**  
Erick Javier Arguello 

---

## 1. Introducción

El monitoreo de variables fisiológicas es una actividad fundamental dentro del entorno clínico, ya que permite observar el estado del paciente en tiempo real y detectar condiciones que puedan representar riesgo. Entre las variables más comunes monitoreadas se encuentran la frecuencia cardíaca, conocida como HR, y la saturación periférica de oxígeno, conocida como SpO₂.

Los monitores de signos vitales permiten visualizar estas variables y generar alarmas cuando los valores se encuentran por fuera de rangos fisiológicos esperados. Sin embargo, para verificar que estos equipos funcionen correctamente, es necesario utilizar simuladores biomédicos capaces de recrear señales fisiológicas bajo condiciones normales y anormales.

En esta práctica se empleó el simulador de parámetros hemodinámicos **Pronk OxSim OX-1** junto con el monitor de signos vitales **uMEC 100**, con el fin de evaluar la respuesta del monitor ante diferentes escenarios simulados, tales como bradicardia, hipoxia, baja perfusión y taquicardia. Además, se verificó la activación de alarmas y se analizaron los errores entre los valores simulados y los valores medidos por el monitor.

---

## 2. Objetivos

### 2.1 Objetivo general

Operar el simulador Pronk OxSim OX-1 y el monitor de signos vitales uMEC 100 para realizar pruebas funcionales de monitoreo cardiovascular y hemodinámico.

### 2.2 Objetivos específicos

- Identificar los modos de operación del simulador de parámetros hemodinámicos Pronk OxSim OX-1.
- Verificar los límites de medición del monitor de signos vitales uMEC 100 mediante la simulación de variables hemodinámicas.
- Interpretar variaciones en parámetros hemodinámicos asociadas a estados fisiológicos y patológicos.
- Evaluar la activación de alarmas visuales y sonoras ante condiciones simuladas.
- Calcular errores absolutos y porcentuales entre los valores simulados y los valores medidos por el monitor.

---

## 3. Marco teórico

### 3.1 Monitoreo de signos vitales

El monitoreo de signos vitales permite evaluar el estado fisiológico de un paciente mediante la medición de variables como frecuencia cardíaca, presión arterial, saturación de oxígeno, frecuencia respiratoria y temperatura. En esta práctica se hizo énfasis en la frecuencia cardíaca y la saturación periférica de oxígeno.

### 3.2 Frecuencia cardíaca

La frecuencia cardíaca corresponde al número de latidos del corazón por minuto y se expresa en latidos por minuto, o bpm. En adultos, una frecuencia cardíaca normal en reposo suele encontrarse aproximadamente entre 60 y 100 bpm.

Valores por debajo de este rango pueden asociarse con bradicardia, mientras que valores por encima pueden asociarse con taquicardia.

### 3.3 Saturación periférica de oxígeno

La saturación periférica de oxígeno, SpO₂, indica el porcentaje de hemoglobina saturada con oxígeno en sangre periférica. En condiciones normales, un valor esperado suele estar entre 95 % y 100 %. Valores bajos pueden indicar hipoxemia o alteraciones en la oxigenación.

### 3.4 Pulsioximetría

La pulsioximetría es una técnica no invasiva que permite medir la saturación de oxígeno y la frecuencia cardíaca. Su funcionamiento se basa en la absorción diferencial de luz roja e infrarroja por parte de la hemoglobina oxigenada y desoxigenada.

El sensor de SpO₂ detecta los cambios de absorción de luz asociados al pulso sanguíneo, generando una señal conocida como señal fotopletismográfica.

### 3.5 Señal fotopletismográfica

La señal fotopletismográfica representa los cambios volumétricos de sangre en el tejido durante cada ciclo cardíaco. Esta señal permite estimar la frecuencia cardíaca y calcular la saturación de oxígeno. Su forma puede verse afectada por movimiento, mala perfusión, baja amplitud de pulso, ruido o mala colocación del sensor.

### 3.6 Simulador Pronk OxSim OX-1

El Pronk OxSim OX-1 es un simulador de parámetros hemodinámicos utilizado para verificar el funcionamiento de monitores de signos vitales y sensores de pulsioximetría. Permite simular diferentes valores de frecuencia cardíaca y saturación de oxígeno, así como condiciones fisiológicas y patológicas.

### 3.7 Monitor de signos vitales uMEC 100

El monitor uMEC 100 es un equipo biomédico utilizado para visualizar variables fisiológicas del paciente. En esta práctica se empleó para registrar la frecuencia cardíaca, la saturación de oxígeno y la forma de onda fotopletismográfica generada a partir del simulador.

---

## 4. Materiales y equipos

| Equipo o material | Cantidad | Descripción |
|---|---:|---|
| Monitor de signos vitales uMEC 100 | 1 | Monitor empleado para visualizar HR, SpO₂ y onda fotopletismográfica |
| Sensor de SpO₂ | 1 | Sensor conectado al monitor uMEC 100 |
| Simulador Pronk OxSim OX-1 | 1 | Simulador de parámetros hemodinámicos |
| Computador con conexión a Internet | 1 | Consulta de manuales y documentación |
| Libreta y lapicero | 1 | Registro de resultados |

---

## 5. Seguridad en el laboratorio

Durante el desarrollo de la práctica se tuvieron en cuenta las siguientes medidas de seguridad:

- No encender ni manipular equipos biomédicos sin presencia o autorización del técnico encargado.
- Usar los elementos de protección personal requeridos, como bata, pantalón largo y cabello recogido.
- Manipular los equipos con cuidado para evitar daños físicos o eléctricos.
- No dejar sesiones abiertas ni archivos guardados en equipos institucionales.
- Verificar conexiones antes de iniciar la simulación.
- Evitar la desconexión brusca de sensores o cables.

---

## 6. Procedimiento

### 6.1 Parte A: Revisión bibliográfica

Se realizó una revisión bibliográfica sobre el monitor de signos vitales uMEC 100 y el simulador Pronk OxSim OX-1. Se consultaron manuales técnicos, información del fabricante y recursos académicos relacionados con el funcionamiento de monitores de signos vitales y simuladores de pulsioximetría.

Se respondieron las siguientes preguntas:

#### a. ¿Cómo colocar el uMEC 100 en modo monitor?

El procedimiento debe verificarse en el manual técnico del equipo uMEC 100. Generalmente, el modo monitor corresponde a la configuración estándar de visualización continua de signos vitales, donde se observan variables como frecuencia cardíaca, SpO₂ y señales asociadas al paciente.

**Respuesta completada con manual:**  
Escribir aquí el procedimiento exacto según el manual del uMEC 100.

#### b. ¿Qué parámetros fisiológicos pueden simularse con el Pronk OxSim OX-1?

El simulador Pronk OxSim OX-1 permite simular parámetros relacionados con pulsioximetría, principalmente:

- Frecuencia cardíaca.
- Saturación periférica de oxígeno.
- Condiciones de baja perfusión.
- Variaciones asociadas a estados fisiológicos o patológicos simulados.

#### c. ¿Cuáles son las tolerancias o errores máximos permitidos para cada parámetro?

Las tolerancias o errores máximos permitidos dependen del fabricante, el manual técnico del monitor y las normas aplicables a equipos de monitoreo biomédico. Para esta práctica, se recomienda consultar los manuales del uMEC 100 y del Pronk OxSim OX-1.

| Parámetro | Tolerancia o EMP según manual | Fuente |
|---|---|---|
| Frecuencia cardíaca | Completar | Manual uMEC 100 |
| SpO₂ | Completar | Manual uMEC 100 |
| Baja perfusión | Completar | Manual Pronk OxSim OX-1 |

---

### 6.2 Parte B: Verificación de alarmas y mediciones

#### Paso 1: Construcción de tabla de alarmas

Se elaboró una tabla para registrar el límite configurado, el valor simulado, la activación de alarma y el tiempo de respuesta.

| Prueba | Límite configurado | Valor simulado | ¿Alarma activa? | Tiempo de respuesta |
|---|---|---:|---|---:|
| SpO₂ baja | 90 % | 85 % | Sí / No | ___ s |
| SpO₂ alta | 97 % | 99 % | Sí / No | ___ s |
| Frecuencia cardíaca alta | Completar | 140 bpm | Sí / No | ___ s |

#### Paso 2: Encendido del uMEC 100

Se encendió el monitor de signos vitales uMEC 100 y se seleccionó el modo de monitoreo.

#### Paso 3: Conexión del sensor

Se conectó la pinza de pulsioximetría del monitor uMEC 100 al simulador Pronk OxSim OX-1.

#### Paso 4: Simulación de paciente bradicárdico

Se configuró el simulador OxSim para simular:

| Variable | Valor simulado |
|---|---:|
| Frecuencia cardíaca | 40 bpm |
| SpO₂ | 95 % |

Luego se registraron los valores observados en el monitor uMEC 100.

| Variable | Valor simulado | Valor medido en monitor | Error absoluto | Error porcentual |
|---|---:|---:|---:|---:|
| Frecuencia cardíaca | 40 bpm | ___ bpm | ___ | ___ % |
| SpO₂ | 95 % | ___ % | ___ | ___ % |

#### Paso 5: Registro de la onda fotopletismográfica

Se observó y registró la forma de onda fotopletismográfica visualizada en el monitor uMEC 100.

**Observación:**  
Describir aquí la forma de onda observada, amplitud, estabilidad, regularidad y presencia de ruido.

**Imagen o captura:**  
Insertar aquí imagen de la onda.

#### Paso 6: Configuración de alarma de SpO₂ baja

Se configuró el límite inferior de alarma de SpO₂ en:

```text
90 %
## Paso 7: Simulación de hipoxia

Se configuró el simulador con los siguientes valores:

| Variable | Valor simulado |
|---|---:|
| Frecuencia cardíaca | 80 bpm |
| SpO₂ | 85 % |

Después de 5 segundos se verificó la activación de alarma visual o sonora.

| Variable | Valor simulado | Valor medido en monitor | Error absoluto | Error porcentual |
|---|---:|---:|---:|---:|
| Frecuencia cardíaca | 80 bpm | ___ bpm | ___ | ___ % |
| SpO₂ | 85 % | ___ % | ___ | ___ % |

**Resultado de alarma:**  
La alarma se activó: Sí / No  
Tiempo de respuesta: ___ segundos

---

## Paso 8: Configuración de alarma de SpO₂ alta

Se configuró el límite superior de alarma de SpO₂ en:

```text
97 %
```

---

## Paso 9: Simulación de SpO₂ alta en modo baja perfusión

Se configuró el simulador para simular:

| Variable | Valor simulado |
|---|---:|
| SpO₂ | 99 % |
| Modo | Low Perfusion |

Después de 5 segundos se verificó la activación de alarma sonora o visual.

| Variable | Valor simulado | Valor medido en monitor | Error absoluto | Error porcentual |
|---|---:|---:|---:|---:|
| SpO₂ | 99 % | ___ % | ___ | ___ % |

**¿La onda fotopletismográfica se distorsiona?**  
Respuesta: Sí / No  

**Descripción:**  
Completar según observación.

---

## Paso 10: Simulación de taquicardia

Con SpO₂ en 95 %, se configuró el simulador para generar:

| Variable | Valor simulado |
|---|---:|
| Frecuencia cardíaca | 140 bpm |
| SpO₂ | 95 % |

Se observó si el monitor activó alarma por frecuencia cardíaca elevada.

| Variable | Valor simulado | Valor medido en monitor | Error absoluto | Error porcentual |
|---|---:|---:|---:|---:|
| Frecuencia cardíaca | 140 bpm | ___ bpm | ___ | ___ % |
| SpO₂ | 95 % | ___ % | ___ | ___ % |

**¿Se activó la alarma de frecuencia cardíaca elevada?**  
Respuesta: Sí / No  

**Tiempo de respuesta:**  
___ segundos

---

# 7. Cálculo de errores

Para comparar los valores simulados con los valores medidos por el monitor, se calcularon el error absoluto y el error porcentual.

## 7.1 Error absoluto

```text
Error absoluto = |Valor medido - Valor simulado|
```

## 7.2 Error porcentual

```text
Error porcentual = (Error absoluto / Valor simulado) × 100
```

## 7.3 Tabla general de errores

| Prueba | Variable | Valor simulado | Valor medido | Error absoluto | Error porcentual |
|---|---|---:|---:|---:|---:|
| Bradicardia | HR | 40 bpm | ___ bpm | ___ | ___ % |
| Bradicardia | SpO₂ | 95 % | ___ % | ___ | ___ % |
| Hipoxia | HR | 80 bpm | ___ bpm | ___ | ___ % |
| Hipoxia | SpO₂ | 85 % | ___ % | ___ | ___ % |
| SpO₂ alta | SpO₂ | 99 % | ___ % | ___ | ___ % |
| Taquicardia | HR | 140 bpm | ___ bpm | ___ | ___ % |
| Taquicardia | SpO₂ | 95 % | ___ % | ___ | ___ % |

---

# 8. Resultados

Durante la práctica se realizaron simulaciones de diferentes condiciones cardiovasculares y hemodinámicas mediante el **Pronk OxSim OX-1**. El monitor **uMEC 100** permitió visualizar la frecuencia cardíaca, la saturación de oxígeno y la señal fotopletismográfica.

Se evaluó la activación de alarmas ante valores fuera de los límites configurados para SpO₂ y frecuencia cardíaca. Además, se registraron los valores medidos por el monitor para calcular el error respecto a los valores simulados.

## 8.1 Resultados de alarmas

| Condición simulada | Límite configurado | Valor simulado | Alarma esperada | Alarma observada | Tiempo de respuesta |
|---|---|---:|---|---|---:|
| SpO₂ baja | 90 % | 85 % | Sí | Sí / No | ___ s |
| SpO₂ alta | 97 % | 99 % | Sí | Sí / No | ___ s |
| Taquicardia | Completar | 140 bpm | Sí | Sí / No | ___ s |

## 8.2 Resultados visuales

Insertar imágenes o capturas de:

- Conexión del sensor de SpO₂ al simulador.
- Pantalla del monitor uMEC 100.
- Onda fotopletismográfica en condición normal.
- Onda en baja perfusión.
- Alarmas visuales o sonoras activadas.

---

# 9. Análisis de resultados

Los resultados obtenidos permiten evaluar el desempeño del monitor **uMEC 100** frente a señales simuladas por el **Pronk OxSim OX-1**.

En la simulación de **bradicardia**, se esperaría que el monitor detectara una frecuencia cardíaca reducida y mostrara una onda fotopletismográfica con pulsos más separados en el tiempo. Si el valor medido por el monitor se aproxima al valor simulado, se puede considerar que la medición de frecuencia cardíaca es confiable dentro de las condiciones de prueba.

En la simulación de **hipoxia**, el valor de SpO₂ se configuró por debajo del límite inferior de alarma. Si el monitor activó alarma sonora o visual, se puede concluir que el sistema de alarmas respondió adecuadamente ante una condición potencialmente crítica.

En la prueba de **SpO₂ alta bajo modo de baja perfusión**, se evaluó la estabilidad de la señal fotopletismográfica. La baja perfusión puede reducir la amplitud de la señal y generar distorsión, lo cual podría afectar la confiabilidad de la medición. Si la onda se observó deformada o inestable, esto puede indicar que el monitor presenta limitaciones en condiciones de baja perfusión.

En la simulación de **taquicardia**, se configuró una frecuencia cardíaca de 140 bpm. En esta condición, se esperaba observar una onda con pulsos más frecuentes y, si el límite superior de frecuencia cardíaca estaba configurado adecuadamente, la activación de una alarma.

Los errores absolutos y porcentuales permiten cuantificar la diferencia entre el valor simulado y el valor medido. Errores bajos indican buena concordancia entre el simulador y el monitor, mientras que errores altos pueden sugerir problemas de configuración, baja calidad de señal, limitaciones del sensor o condiciones simuladas difíciles de interpretar.

---

# 10. Preguntas para la discusión

## 10.1 ¿Cuál es el principio de operación del Pronk OxSim OX-1 para simular una onda pulsátil?

El **Pronk OxSim OX-1** simula señales asociadas a la pulsioximetría mediante la generación de patrones equivalentes a los cambios ópticos que se producen durante el pulso sanguíneo. Estos patrones permiten que el sensor de SpO₂ del monitor interprete una señal similar a la que recibiría en un paciente real.

El simulador reproduce condiciones de frecuencia cardíaca y saturación de oxígeno, permitiendo evaluar si el monitor mide correctamente y si activa alarmas ante valores fuera de rango.

## 10.2 ¿Por qué la SpO₂ baja puede ser un falso positivo en una situación de mala perfusión?

La SpO₂ baja puede ser un falso positivo en mala perfusión porque el sensor de pulsioximetría depende de una señal pulsátil adecuada. Cuando hay baja perfusión, el flujo sanguíneo periférico disminuye y la amplitud de la señal fotopletismográfica se reduce.

Esto puede ocasionar que el monitor interprete erróneamente la señal y reporte una saturación baja, aunque la oxigenación real no necesariamente esté disminuida. También pueden influir factores como movimiento, mala colocación del sensor, temperatura baja en extremidades o ruido en la señal.

---

# 11. Conclusiones

- La práctica permitió comprender la importancia de los simuladores biomédicos en la verificación funcional de monitores de signos vitales.
- El Pronk OxSim OX-1 permitió simular condiciones fisiológicas y patológicas, como bradicardia, hipoxia, baja perfusión y taquicardia.
- El monitor uMEC 100 permitió visualizar variables como frecuencia cardíaca, SpO₂ y la señal fotopletismográfica.
- La verificación de alarmas permitió comprobar la respuesta del monitor ante valores fuera de los límites configurados.
- El cálculo de errores absolutos y porcentuales permitió evaluar la precisión del monitor frente a valores simulados.
- Las condiciones de baja perfusión pueden afectar la calidad de la señal fotopletismográfica y generar posibles falsas alarmas.
- La práctica refuerza la importancia de evaluar periódicamente los equipos biomédicos para garantizar seguridad, confiabilidad y desempeño clínico adecuado.

---

# 12. Limitaciones

- Los resultados dependen de la correcta configuración del simulador y del monitor.
- La calidad de la señal puede verse afectada por la conexión del sensor.
- Algunos procedimientos específicos deben verificarse directamente en los manuales técnicos del uMEC 100 y del Pronk OxSim OX-1.
- Las simulaciones no reemplazan completamente las condiciones fisiológicas reales de un paciente.

---

# 13. Bibliografía

1. Instituto de Salud Pública de Chile. *Guía para la Clasificación de Dispositivos Médicos según Riesgo*.
2. Instituto Nacional de Vigilancia de Medicamentos y Alimentos, INVIMA. *ABC de Dispositivos Médicos - Guía Reguladora*.
3. Medical IT. *Metrología Biomédica - OxSim*.
4. Manual técnico del monitor de signos vitales uMEC 100.
5. Manual técnico del simulador Pronk OxSim OX-1.

---

# 14. Anexos

## Anexo A. Registro fotográfico

Insertar aquí imágenes del montaje experimental.

## Anexo B. Capturas de onda fotopletismográfica

Insertar aquí capturas de la onda observada en el monitor.

## Anexo C. Evidencia de alarmas

Insertar aquí imágenes o registros de activación de alarmas.

## Anexo D. Cálculos

Insertar aquí cálculos detallados de error absoluto y error porcentual.2
