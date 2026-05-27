 Informe de Laboratorio 5  
## Simulación y Monitoreo de Variables Cardiovasculares y Hemodinámicas

**Universidad Militar Nueva Granada**  
**Facultad:** Ingeniería  
**Programa:** Ingeniería Biomédica  
**Asignatura:** Instrumentación Biomédica y Biosensores  
**Semestre:** VII  

---

## Integrantes

- María Paula Fernández  
- Nombre del integrante 2  
- Nombre del integrante 3  

**Docente:** Nombre del docente  
**Fecha:** Día / Mes / Año  

---

## 1. Introducción

El monitoreo de variables fisiológicas es una actividad fundamental dentro del entorno clínico, ya que permite observar el estado del paciente en tiempo real y detectar condiciones que puedan representar riesgo. Entre las variables más comunes monitoreadas se encuentran la frecuencia cardíaca, conocida como **HR** o **BPM**, y la saturación periférica de oxígeno, conocida como **SpO₂**.

Los monitores de signos vitales permiten visualizar estas variables y generar alarmas cuando los valores se encuentran por fuera de rangos fisiológicos esperados. Para verificar que estos equipos funcionen correctamente, se utilizan simuladores biomédicos capaces de recrear señales fisiológicas bajo condiciones normales y anormales.

En esta práctica se empleó el simulador de parámetros hemodinámicos **Pronk OxSim OX-1** junto con el monitor de signos vitales **Mindray uMEC 100**, con el fin de evaluar la respuesta del monitor ante diferentes escenarios simulados, tales como bradicardia, hipoxia, baja perfusión y taquicardia. Además, se analizaron los errores entre los valores simulados y los valores medidos por el monitor.

---

## 2. Objetivos

### 2.1 Objetivo general

Operar el simulador **Pronk OxSim OX-1** y el monitor de signos vitales **uMEC 100** para realizar pruebas funcionales de monitoreo cardiovascular y hemodinámico.

### 2.2 Objetivos específicos

- Identificar los modos de operación del simulador de parámetros hemodinámicos Pronk OxSim OX-1.
- Verificar los límites de medición del monitor de signos vitales uMEC 100 mediante simulación de variables hemodinámicas.
- Interpretar variaciones en parámetros hemodinámicos asociadas a estados fisiológicos y patológicos.
- Evaluar el desempeño funcional del monitor frente a valores simulados.
- Calcular errores absolutos y porcentuales entre los valores simulados y los valores medidos por el monitor.
- Analizar la repetibilidad de las mediciones mediante promedio, desviación estándar e incertidumbre tipo A.

---

## 3. Marco teórico

### 3.1 Monitoreo de signos vitales

El monitoreo de signos vitales permite evaluar el estado fisiológico de un paciente mediante la medición de variables como frecuencia cardíaca, presión arterial, saturación de oxígeno, frecuencia respiratoria y temperatura. En esta práctica se hizo énfasis en la frecuencia cardíaca, la saturación periférica de oxígeno y la frecuencia respiratoria.

### 3.2 Frecuencia cardíaca

La frecuencia cardíaca corresponde al número de latidos del corazón por minuto y se expresa en **BPM**. En adultos, una frecuencia cardíaca normal en reposo suele encontrarse aproximadamente entre 60 y 100 BPM.

Valores por debajo de este rango pueden asociarse con **bradicardia**, mientras que valores por encima pueden asociarse con **taquicardia**.

### 3.3 Saturación periférica de oxígeno

La saturación periférica de oxígeno, **SpO₂**, indica el porcentaje de hemoglobina saturada con oxígeno en sangre periférica. En condiciones normales, un valor esperado suele estar entre 95 % y 100 %. Valores bajos pueden indicar hipoxemia o alteraciones en la oxigenación.

### 3.4 Pulsioximetría

La pulsioximetría es una técnica no invasiva que permite medir la saturación de oxígeno y la frecuencia cardíaca. Su funcionamiento se basa en la absorción diferencial de luz roja e infrarroja por parte de la hemoglobina oxigenada y desoxigenada.

### 3.5 Señal fotopletismográfica

La señal fotopletismográfica representa los cambios volumétricos de sangre en el tejido durante cada ciclo cardíaco. Esta señal permite estimar la frecuencia cardíaca y calcular la saturación de oxígeno. Su forma puede verse afectada por movimiento, mala perfusión, baja amplitud de pulso, ruido o mala colocación del sensor.

### 3.6 Simulador Pronk OxSim OX-1

El **Pronk OxSim OX-1** es un simulador de parámetros hemodinámicos utilizado para verificar el funcionamiento de monitores de signos vitales y sensores de pulsioximetría. Permite simular diferentes valores de frecuencia cardíaca y saturación de oxígeno, así como condiciones fisiológicas y patológicas.

### 3.7 Monitor de signos vitales uMEC 100

El **uMEC 100** es un monitor de signos vitales utilizado para visualizar variables fisiológicas del paciente. En esta práctica se empleó para registrar frecuencia cardíaca, saturación de oxígeno y frecuencia respiratoria frente a señales simuladas.

---

## 4. Materiales, equipos e instrumentos

### 4.1 Equipo bajo prueba

| Característica | Información |
|---|---|
| Equipo | Monitor de signos vitales |
| Marca | Mindray |
| Modelo | uMEC 100 |
| Serie | FT4-4C015042 |
| Activo | 210000001-5767 |
| Fecha de verificación | 30.04.2026 |

### 4.2 Instrumentos utilizados

| Equipo | Marca | Modelo | Serie | Fecha de calibración |
|---|---|---|---|---|
| SimCube NIBP Simulator | Pronk Technologies | SC-5 | 16433 | 01.04.2026 |
| Simulador de pulsioximetría | Pronk Technologies | OX-1 | Maleta Pequeña 1 | 01.04.2026 |

### 4.3 Condiciones ambientales

| Magnitud | Valor registrado | Unidad |
|---|---:|---|
| Temperatura ambiente | 22,7 | °C |
| Humedad relativa | 49,0 | % |
| Registro adicional | 22,5 | °C |

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

Se realizó una revisión bibliográfica sobre el monitor de signos vitales **uMEC 100** y el simulador **Pronk OxSim OX-1**. Se consultaron manuales técnicos, información del fabricante y recursos académicos relacionados con monitores de signos vitales y simuladores de pulsioximetría.

#### a. ¿Cómo colocar el uMEC 100 en modo monitor?

El procedimiento debe verificarse en el manual técnico del equipo uMEC 100. Generalmente, el modo monitor corresponde a la configuración estándar de visualización continua de signos vitales, donde se observan variables como frecuencia cardíaca, SpO₂ y señales asociadas al paciente.

**Respuesta completada con manual:**  
Completar aquí el procedimiento exacto según el manual del uMEC 100.

#### b. ¿Qué parámetros fisiológicos pueden simularse con el Pronk OxSim OX-1?

El simulador Pronk OxSim OX-1 permite simular parámetros relacionados con pulsioximetría, principalmente:

- Frecuencia cardíaca.
- Saturación periférica de oxígeno.
- Condiciones de baja perfusión.
- Variaciones asociadas a estados fisiológicos o patológicos simulados.

#### c. ¿Cuáles son las tolerancias o errores máximos permitidos para cada parámetro?

Las tolerancias o errores máximos permitidos dependen del fabricante, el manual técnico del monitor y las normas aplicables a equipos de monitoreo biomédico. En esta práctica se evaluó el error de indicación como la diferencia entre el promedio medido y el valor de referencia simulado.

---

### 6.2 Parte B: Verificación de mediciones

La verificación consistió en comparar las indicaciones del monitor frente a señales simuladas de frecuencia cardíaca, saturación de oxígeno y frecuencia respiratoria. Las lecturas se registraron cada 10 segundos, con cinco observaciones por punto cuando la serie fue legible y completa.

No se aplicaron correcciones ni ajustes al equipo bajo prueba.

---

## Paso 1: Construcción de tabla de alarmas

Se diseñó una tabla para registrar el límite configurado, el valor simulado, la activación de alarma y el tiempo de respuesta.

> **Nota:** En los resultados metrológicos disponibles se registraron principalmente indicaciones del equipo, promedios, desviación estándar, error e incertidumbre tipo A. La activación de alarmas debe completarse con la evidencia visual o sonora tomada durante la práctica.

| Prueba | Límite configurado | Valor simulado | ¿Alarma activa? | Tiempo de respuesta |
|---|---|---:|---|---:|
| SpO₂ baja | 90 % | 85 % | No registrado | No registrado |
| SpO₂ alta | 97 % | 100 % | No registrado | No registrado |
| Frecuencia cardíaca alta | Completar | 140 BPM | No registrado | No registrado |

---

## Paso 2: Encendido del uMEC 100

Se encendió el monitor de signos vitales **uMEC 100** y se seleccionó el modo de monitoreo.

---

## Paso 3: Conexión del sensor

Se conectó la pinza de pulsioximetría del monitor uMEC 100 al simulador **Pronk OxSim OX-1**.

---

## Paso 4: Simulación de paciente bradicárdico

Se configuró el simulador OxSim para simular una condición de bradicardia con frecuencia cardíaca de 40 BPM y SpO₂ de 95 %.

| Variable | Valor simulado | Indicaciones del equipo cada 10 s | n | Promedio | s | Error | uA |
|---|---:|---|---:|---:|---:|---:|---:|
| Frecuencia cardíaca | 40,0 BPM | 40,0; 40,0; 40,0; 40,0; 40,0 | 5 | 40,0 BPM | 0,00 BPM | 0,00 BPM | 0,00 BPM |
| SpO₂ | 95,0 % | 95,0; 95,0; 95,0; 95,0; 95,0 | 5 | 95,0 % | 0,00 % | 0,00 % | 0,00 % |

**Interpretación:**  
El monitor registró valores iguales al valor simulado, por lo que no se presentó error de indicación en este punto.

---

## Paso 5: Registro de onda fotopletismográfica

Se observó la forma de onda fotopletismográfica visualizada en el monitor uMEC 100.

**Observación:**  
Completar con la descripción visual de la onda observada: amplitud, estabilidad, regularidad y presencia o ausencia de ruido.

**Imagen o captura:**  
Insertar aquí imagen de la onda.

---

## Paso 6: Configuración de alarma de SpO₂ baja

Se configuró el límite inferior de alarma de SpO₂ en:

```text
90 %
```

---

## Paso 7: Simulación de hipoxia

Se configuró el simulador con los siguientes valores:

| Variable | Valor simulado |
|---|---:|
| Frecuencia cardíaca | 80 BPM |
| SpO₂ | 85 % |

Después de 5 segundos se verificó la activación de alarma visual o sonora.

### Resultados de medición

| Variable | Valor simulado | Indicaciones del equipo cada 10 s | n | Promedio | s | Error | uA |
|---|---:|---|---:|---:|---:|---:|---:|
| Frecuencia cardíaca | 80,0 BPM | 80,0; 80,0; 80,0; 80,0; 80,0 | 5 | 80,0 BPM | 0,00 BPM | 0,00 BPM | 0,00 BPM |
| SpO₂ | 85,0 % | 85,0; 85,0; 85,0; 85,0; 85,0 | 5 | 85,0 % | 0,00 % | 0,00 % | 0,00 % |

**Resultado de alarma:**  
La alarma se activó: No registrado en certificado  
Tiempo de respuesta: No registrado  

**Interpretación:**  
El monitor registró correctamente los valores simulados de frecuencia cardíaca y saturación de oxígeno. El error de indicación fue de 0,00 para ambas variables.

---

## Paso 8: Configuración de alarma de SpO₂ alta

Se configuró el límite superior de alarma de SpO₂ en:

```text
97 %
```

---

## Paso 9: Simulación de SpO₂ alta en modo baja perfusión

Se configuró el simulador para simular una condición de SpO₂ alta bajo anotación de **low perfusion**.

| Variable | Valor simulado |
|---|---:|
| SpO₂ | 100 % |
| Modo | Low Perfusion |

### Resultado de medición

| Variable | Valor simulado | Indicaciones del equipo cada 10 s | n | Promedio | s | Error | uA |
|---|---:|---|---:|---:|---:|---:|---:|
| SpO₂ | 100,0 % | 100,0; 100,0; 100,0; 100,0; 100,0 | 5 | 100,0 % | 0,00 % | 0,00 % | 0,00 % |

**¿La onda fotopletismográfica se distorsiona?**  
No registrado en el certificado.  

**Descripción:**  
Completar según la observación visual tomada durante la práctica. Metrológicamente, el valor de SpO₂ se mantuvo estable en 100,0 %, sin dispersión en las cinco lecturas registradas.

---

## Paso 10: Simulación de taquicardia

Se configuró el simulador para generar una frecuencia cardíaca elevada.

| Variable | Valor simulado |
|---|---:|
| Frecuencia cardíaca | 140 BPM |
| SpO₂ | 98 % |

### Resultados de medición

| Variable | Valor simulado | Indicaciones del equipo cada 10 s | n | Promedio | s | Error | uA |
|---|---:|---|---:|---:|---:|---:|---:|
| Frecuencia cardíaca | 140,0 BPM | 140,0; 140,0; 140,0; 140,0; 140,0 | 5 | 140,0 BPM | 0,00 BPM | 0,00 BPM | 0,00 BPM |
| SpO₂ | 98,0 % | 98,0; 98,0; 98,0; 98,0; 98,0 | 5 | 98,0 % | 0,00 % | 0,00 % | 0,00 % |

**¿Se activó la alarma de frecuencia cardíaca elevada?**  
No registrado en certificado.  

**Tiempo de respuesta:**  
No registrado.  

**Interpretación:**  
El monitor registró correctamente la frecuencia cardíaca de 140 BPM y la SpO₂ de 98 %. No se presentó error de indicación ni dispersión en las lecturas.

---

# 7. Cálculo de errores

Para comparar los valores simulados con los valores medidos por el monitor, se calcularon el error absoluto, el error porcentual, la desviación estándar experimental y la incertidumbre típica tipo A.

## 7.1 Error absoluto

```text
Error absoluto = |Valor medido - Valor simulado|
```

## 7.2 Error porcentual

```text
Error porcentual = (Error absoluto / Valor simulado) × 100
```

## 7.3 Promedio aritmético

```text
Promedio = suma de las indicaciones / número de indicaciones
```

## 7.4 Incertidumbre tipo A

```text
uA = s / √n
```

Donde:

- `s` corresponde a la desviación estándar experimental.
- `n` corresponde al número de mediciones.
- `uA` corresponde a la incertidumbre típica de la media.

---

# 8. Resultados

## 8.1 Resultados de frecuencia cardíaca / BPM

| Punto / condición | Valor simulado o referencia | Indicaciones del equipo cada 10 s | n | Promedio | s | Error | uA |
|---|---:|---|---:|---:|---:|---:|---:|
| Punto 1 - asociado a SpO₂ 85 % | 80,0 BPM | 80,0; 80,0; 80,0; 80,0; 80,0 | 5 | 80,0 BPM | 0,00 BPM | 0,00 BPM | 0,00 BPM |
| Punto 2 - asociado a SpO₂ 95 % | 40,0 BPM | 40,0; 40,0; 40,0; 40,0; 40,0 | 5 | 40,0 BPM | 0,00 BPM | 0,00 BPM | 0,00 BPM |
| Punto 3 - asociado a SpO₂ 98 % | 80,0 BPM | 80,0; 80,0; 80,0; 80,0; 80,0 | 5 | 80,0 BPM | 0,00 BPM | 0,00 BPM | 0,00 BPM |
| Punto 4 - asociado a SpO₂ 98 % | 140,0 BPM | 140,0; 140,0; 140,0; 140,0; 140,0 | 5 | 140,0 BPM | 0,00 BPM | 0,00 BPM | 0,00 BPM |
| Punto 5 - asociado a SpO₂ 100 % | 80,0 BPM | 80,0; 80,0; 80,0; 80,0; 80,0 | 5 | 80,0 BPM | 0,00 BPM | 0,00 BPM | 0,00 BPM |
| Punto 6 - registro simultáneo con RPM | 70,0 BPM | 70,0; 70,0; 70,0; 70,0; 70,0 | 5 | 70,0 BPM | 0,00 BPM | 0,00 BPM | 0,00 BPM |
| Punto 7 - registro simultáneo con RPM | 95,0 BPM | 95,0; 95,0; 95,0; 95,0; 95,0 | 5 | 95,0 BPM | 0,00 BPM | 0,00 BPM | 0,00 BPM |
| Punto 8 - registro simultáneo con RPM | 70,0 BPM | 70,0; 70,0; 70,0; 70,0; 70,0 | 5 | 70,0 BPM | 0,00 BPM | 0,00 BPM | 0,00 BPM |
| Punto 9 - condición de apnea | No disponible | 69,0; 69,0; 69,0; 75,0; 69,0 | 5 | 70,2 BPM | 2,68 BPM | N/D | 1,20 BPM |

---

## 8.2 Resultados de saturación de oxígeno / SpO₂

| Punto / condición | Valor simulado o referencia | Indicaciones del equipo cada 10 s | n | Promedio | s | Error | uA |
|---|---:|---|---:|---:|---:|---:|---:|
| Punto 1 | 85,0 % | 85,0; 85,0; 85,0; 85,0; 85,0 | 5 | 85,0 % | 0,00 % | 0,00 % | 0,00 % |
| Punto 2 | 95,0 % | 95,0; 95,0; 95,0; 95,0; 95,0 | 5 | 95,0 % | 0,00 % | 0,00 % | 0,00 % |
| Punto 3 - con BPM 80 | 98,0 % | 98,0; 98,0; 98,0; 98,0; 98,0 | 5 | 98,0 % | 0,00 % | 0,00 % | 0,00 % |
| Punto 4 - con BPM 140 | 98,0 % | 98,0; 98,0; 98,0; 98,0; 98,0 | 5 | 98,0 % | 0,00 % | 0,00 % | 0,00 % |
| Punto 5 - anotación low perf | 100,0 % | 100,0; 100,0; 100,0; 100,0; 100,0 | 5 | 100,0 % | 0,00 % | 0,00 % | 0,00 % |

---

## 8.3 Resultados de frecuencia respiratoria / RPM

| Punto / condición | Valor simulado o referencia | Indicaciones del equipo cada 10 s | n | Promedio | s | Error | uA |
|---|---:|---|---:|---:|---:|---:|---:|
| Punto 1 - serie 20/10 registrada | No disponible | 20,0; 20,0; 10,0; 10,0; 10,0 | 5 | 14,0 RPM | 5,48 RPM | N/D | 2,45 RPM |
| Punto 2 | 40,0 RPM | 40,0; 40,0; 40,0; 40,0; 40,0 | 5 | 40,0 RPM | 0,00 RPM | 0,00 RPM | 0,00 RPM |
| Punto 3 | 10,0 RPM | 10,0; 10,0; 10,0; 20,0; 10,0 | 5 | 12,0 RPM | 4,47 RPM | 2,00 RPM | 2,00 RPM |
| Punto 4 - apnea | 0,0 RPM | 0,0; 0,0; 0,0; 0,0; 0,0 | 5 | 0,0 RPM | 0,00 RPM | 0,00 RPM | 0,00 RPM |

---

## 8.4 Resultados de alarmas

| Condición simulada | Límite configurado | Valor simulado | Alarma esperada | Alarma observada | Tiempo de respuesta |
|---|---|---:|---|---|---:|
| SpO₂ baja | 90 % | 85 % | Sí | No registrado | No registrado |
| SpO₂ alta | 97 % | 100 % | Sí | No registrado | No registrado |
| Taquicardia | Completar | 140 BPM | Sí | No registrado | No registrado |

---

## 8.5 Resultados visuales

Insertar imágenes o capturas de:

- Conexión del sensor de SpO₂ al simulador.
- Pantalla del monitor uMEC 100.
- Onda fotopletismográfica en condición normal.
- Onda fotopletismográfica en baja perfusión.
- Alarmas visuales o sonoras activadas.

---

# 9. Análisis de resultados

Los resultados obtenidos permiten evaluar el desempeño del monitor **Mindray uMEC 100** frente a señales simuladas por el **Pronk OxSim OX-1** y el **SimCube NIBP Simulator SC-5**.

En las mediciones de **frecuencia cardíaca**, la mayoría de puntos evaluados presentaron error de indicación igual a **0,00 BPM**, lo cual evidencia una alta concordancia entre el valor simulado y el valor mostrado por el monitor. Los puntos de 40 BPM, 80 BPM, 95 BPM y 140 BPM se mantuvieron constantes durante las cinco observaciones registradas cada 10 segundos.

En la condición asociada a **apnea**, no se contó con un valor de referencia disponible para la frecuencia cardíaca. Sin embargo, las lecturas registradas fueron 69,0; 69,0; 69,0; 75,0 y 69,0 BPM, con un promedio de **70,2 BPM**, desviación estándar de **2,68 BPM** e incertidumbre tipo A de **1,20 BPM**. Esta condición presentó mayor dispersión que los demás puntos de BPM.

En las mediciones de **SpO₂**, todos los puntos evaluados presentaron error de **0,00 %**, incluyendo los valores de 85 %, 95 %, 98 % y 100 %. Esto indica que el monitor reprodujo correctamente las condiciones simuladas por el equipo de pulsioximetría.

En el caso de la condición de **low perfusion**, el valor simulado fue de 100 % de SpO₂ y el monitor registró cinco lecturas iguales de 100,0 %. Aunque el dato metrológico fue estable, la distorsión de la onda fotopletismográfica debe confirmarse con la observación visual realizada durante la práctica.

En la evaluación de **frecuencia respiratoria**, se observaron diferencias en algunos puntos. En el punto de 40 RPM y en la condición de apnea de 0 RPM, el error fue de 0,00 RPM. Sin embargo, en el punto de referencia de 10 RPM, el monitor registró un promedio de 12,0 RPM, con error de **2,00 RPM**, desviación estándar de **4,47 RPM** e incertidumbre tipo A de **2,00 RPM**. Esto muestra que la medición respiratoria presentó mayor variabilidad que la frecuencia cardíaca y la SpO₂.

En general, el monitor presentó un desempeño adecuado para frecuencia cardíaca y saturación de oxígeno en los puntos evaluados, con errores nulos y alta repetibilidad. La mayor variabilidad se observó en frecuencia respiratoria y en la condición de apnea asociada al registro de BPM.

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
- El monitor Mindray uMEC 100 presentó alta concordancia con los valores simulados de frecuencia cardíaca y SpO₂.
- En frecuencia cardíaca, los puntos evaluados de 40 BPM, 80 BPM, 95 BPM y 140 BPM presentaron error de indicación de 0,00 BPM.
- En saturación de oxígeno, los puntos de 85 %, 95 %, 98 % y 100 % presentaron error de 0,00 %, lo que indica buena respuesta del sistema de pulsioximetría.
- La condición de baja perfusión mostró estabilidad metrológica en SpO₂, aunque la distorsión de la señal fotopletismográfica debe analizarse mediante evidencia visual.
- La frecuencia respiratoria presentó mayor variabilidad en algunos puntos, especialmente en la serie 20/10 y en el punto de referencia de 10 RPM.
- El cálculo de promedio, desviación estándar, error e incertidumbre tipo A permitió evaluar la repetibilidad de las indicaciones del monitor.
- La práctica refuerza la importancia de verificar periódicamente el funcionamiento de equipos biomédicos para garantizar seguridad, confiabilidad y desempeño clínico adecuado.

---

# 12. Limitaciones

- Los resultados aplican únicamente al monitor identificado y a los puntos evaluados.
- No se calculó incertidumbre tipo B porque no se contaba con información externa suficiente, como certificados completos de calibración, resolución del monitor o incertidumbre declarada de los patrones.
- La activación de alarmas visuales o sonoras no quedó registrada en el certificado metrológico y debe completarse con evidencia experimental.
- La calidad de la señal puede verse afectada por la conexión del sensor, baja perfusión o configuración del simulador.
- Las simulaciones no reemplazan completamente las condiciones fisiológicas reales de un paciente.

---

# 13. Bibliografía

1. Instituto de Salud Pública de Chile. *Guía para la Clasificación de Dispositivos Médicos según Riesgo*.  
2. Instituto Nacional de Vigilancia de Medicamentos y Alimentos, INVIMA. *ABC de Dispositivos Médicos - Guía Reguladora*.  
3. Medical IT. *Metrología Biomédica - OxSim*.  
4. Manual técnico del monitor de signos vitales uMEC 100.  
5. Manual técnico del simulador Pronk OxSim OX-1.  
6. Certificado de verificación metrológica del monitor de signos vitales Mindray uMEC 100.

---

# 14. Anexos

## Anexo A. Registro fotográfico

Insertar aquí imágenes del montaje experimental.

## Anexo B. Capturas de onda fotopletismográfica

Insertar aquí capturas de la onda observada en el monitor.

## Anexo C. Evidencia de alarmas

Insertar aquí imágenes o registros de activación de alarmas.

## Anexo D. Cálculos

Insertar aquí cálculos detallados de error absoluto, error porcentual e incertidumbre tipo A.
