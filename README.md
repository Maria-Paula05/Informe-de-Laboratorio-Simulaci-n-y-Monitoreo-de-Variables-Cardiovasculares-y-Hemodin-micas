
# Simulación y Monitoreo de Variables Cardiovasculares y Hemodinámicas

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

El monitoreo de variables fisiológicas es una actividad fundamental dentro del entorno clínico, ya que permite observar el estado del paciente en tiempo real y apoyar la detección temprana de condiciones que puedan representar riesgo. Entre las variables más comunes monitoreadas se encuentran la frecuencia cardíaca, expresada como **HR** o **BPM**, la saturación periférica de oxígeno, conocida como **SpO₂**, y la frecuencia respiratoria, expresada como **RPM**. Estas variables hacen parte de los signos vitales utilizados para valorar el estado fisiológico general de un paciente; por ejemplo, en adultos sanos en reposo, la frecuencia cardíaca suele encontrarse entre 60 y 100 latidos por minuto y la frecuencia respiratoria entre 12 y 18 respiraciones por minuto [1].

Los monitores de signos vitales son equipos biomédicos diseñados para visualizar variables fisiológicas y emitir alarmas cuando los valores se encuentran por fuera de rangos configurados o fisiológicamente esperados. Por esta razón, su desempeño debe verificarse de forma periódica, ya que una indicación incorrecta puede afectar la interpretación clínica, el seguimiento del paciente y la toma de decisiones médicas [2]. En este contexto, la verificación metrológica permite comparar las indicaciones del equipo bajo prueba contra valores de referencia generados por simuladores biomédicos, evaluando así la exactitud, repetibilidad y comportamiento funcional del sistema de medición, conforme a los principios establecidos en la norma NTC-ISO/IEC 17025:2017 [3].

En el presente informe se analiza la verificación metrológica y funcional del monitor de signos vitales **Mindray uMEC 100**, realizada mediante comparación de sus indicaciones frente a valores simulados de **BPM**, **SpO₂** y **RPM**. Según el certificado de verificación No. MP-20260430-1 emitido por BIOCORE S.A.S., el equipo evaluado corresponde a un monitor de signos vitales Mindray, modelo **uMEC 100**, serie **FT4-4C015042**, y las pruebas fueron realizadas el **30 de abril de 2026**, bajo condiciones ambientales de **22,7 °C** de temperatura y **49,0 %** de humedad relativa. Para la verificación se utilizaron como instrumentos de referencia el simulador de pulsioximetría **Pronk Technologies OX-1** y el **SimCube NIBP Simulator SC-5**, ambos con fecha de calibración del 01.04.2026 [6].

La práctica se enfocó en comparar los valores simulados con las lecturas indicadas por el monitor, registrando mediciones repetidas cada 10 segundos. A partir de estos datos se calcularon promedios, desviación estándar experimental, error de indicación e incertidumbre tipo A de la media. Este procedimiento permite evaluar si el monitor responde de manera consistente frente a señales simuladas y si sus indicaciones son adecuadas para el uso clínico previsto. La evaluación de incertidumbre tipo A se fundamenta en el análisis estadístico de observaciones repetidas, conforme a la guía del NIST para expresión de incertidumbre de medición [4].

De esta manera, el informe no solo describe los resultados obtenidos, sino que también resalta la importancia de la metrología biomédica en la seguridad del paciente, la confiabilidad diagnóstica y la gestión tecnológica hospitalaria. Un monitor de signos vitales no debe considerarse seguro únicamente porque enciende o muestra valores en pantalla; también debe demostrar que sus mediciones son coherentes, repetibles y trazables frente a patrones o simuladores adecuados [2].

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

### 3.1 Verificación metrológica en equipos biomédicos

La metrología es la ciencia de las mediciones y sus aplicaciones. En el ámbito biomédico, permite evaluar si un equipo médico mide correctamente, si sus indicaciones son confiables y si se encuentra en condiciones adecuadas para su uso clínico. El Vocabulario Internacional de Metrología (VIM) establece conceptos fundamentales relacionados con medición, error, incertidumbre, trazabilidad y verificación, los cuales son aplicables tanto a mediciones físicas como químicas, biológicas, médicas e ingenieriles [5].

En equipos biomédicos como los monitores de signos vitales, la verificación metrológica consiste en comparar las lecturas del equipo bajo prueba con valores conocidos o simulados. Esta comparación permite determinar el error de indicación, la repetibilidad de las lecturas y la estabilidad del equipo frente a diferentes puntos de medición. La norma NTC-ISO/IEC 17025:2017 establece los requisitos generales para la competencia de laboratorios de ensayo y calibración, y su terminología fue empleada en el certificado analizado [3].

En el certificado No. MP-20260430-1, la verificación consistió en comparar las indicaciones del monitor **Mindray uMEC 100** frente a señales simuladas de frecuencia cardíaca, saturación de oxígeno y frecuencia respiratoria. Las lecturas fueron tomadas cada 10 segundos, con cinco observaciones por punto cuando la serie fue legible y completa. Se indica además que no se aplicaron correcciones ni ajustes al equipo bajo prueba [6].

---

### 3.2 Monitor de signos vitales

Un monitor de signos vitales es un equipo biomédico utilizado para visualizar variables fisiológicas del paciente, tales como frecuencia cardíaca, saturación de oxígeno, presión arterial, frecuencia respiratoria y temperatura. Estos equipos son fundamentales en áreas como hospitalización, urgencias, salas de cirugía, unidades de cuidado intensivo y consulta externa [2].

El monitor **Mindray uMEC 100** evaluado en este informe fue sometido a verificación funcional y metrológica mediante comparación con simuladores biomédicos. Según el certificado, el equipo bajo prueba corresponde a un monitor de signos vitales marca **Mindray**, modelo **uMEC 100**, identificado con serie **FT4-4C015042** y activo institucional **210000001-5767** [6].

La función principal de este tipo de monitor es mostrar de manera continua o periódica las variables fisiológicas del paciente y generar alertas cuando los valores se encuentran por fuera de los límites configurados. Por lo tanto, la confiabilidad de sus mediciones es esencial para evitar interpretaciones erróneas o decisiones clínicas inadecuadas [4].

---

### 3.3 Frecuencia cardíaca / BPM

La frecuencia cardíaca corresponde al número de contracciones del corazón por minuto y se expresa en **BPM**. Este parámetro permite evaluar la actividad cardíaca del paciente y detectar alteraciones como bradicardia, cuando es inferior a 60 BPM, o taquicardia, cuando supera los 100 BPM. En adultos sanos en reposo, una frecuencia cardíaca normal suele encontrarse entre **60 y 100 BPM** [1].

En el contexto metrológico, la frecuencia cardíaca puede simularse mediante equipos patrón o simuladores biomédicos. En el certificado de verificación, se evaluaron varios puntos de BPM, incluyendo valores de **40 BPM**, **70 BPM**, **80 BPM**, **95 BPM** y **140 BPM**. En la mayoría de los puntos evaluados, las indicaciones del monitor coincidieron con el valor simulado, presentando error de **0,00 BPM** y desviación estándar de **0,00 BPM** [6].

Estos resultados sugieren que, para los puntos evaluados, el monitor presentó una respuesta estable y repetible en la medición de frecuencia cardíaca. Sin embargo, en el punto asociado a condición de apnea se registraron lecturas variables de **69,0 BPM** y **75,0 BPM**, con promedio de **70,2 BPM**, desviación estándar de **2,68 BPM** e incertidumbre tipo A de **1,20 BPM** [6].

---

### 3.4 Saturación periférica de oxígeno / SpO₂

La saturación periférica de oxígeno, o **SpO₂**, representa una estimación no invasiva del porcentaje de hemoglobina saturada con oxígeno en sangre arterial periférica. Los pulsioxímetros utilizan haces de luz roja e infrarroja para estimar la saturación de oxígeno y la frecuencia del pulso, generalmente mediante un sensor colocado en el dedo u otra zona periférica [1].

La medición de SpO₂ es importante porque permite identificar posibles alteraciones en la oxigenación del paciente. En condiciones clínicas habituales, valores cercanos a **95 % – 100 %** suelen considerarse esperados en sujetos sanos, aunque la interpretación siempre debe realizarse de acuerdo con el contexto clínico del paciente [1].

En la verificación realizada al monitor **uMEC 100**, se evaluaron puntos de saturación de oxígeno de **85 %**, **95 %**, **98 %** y **100 %**. Para todos los puntos registrados, las indicaciones del monitor coincidieron con el valor simulado, obteniéndose promedio igual al valor de referencia, desviación estándar de **0,00 %**, error de **0,00 %** e incertidumbre tipo A de **0,00 %** [6].

---

### 3.5 Pulsioximetría

La pulsioximetría es una técnica óptica no invasiva utilizada para estimar la saturación periférica de oxígeno y la frecuencia del pulso. Su principio de funcionamiento se basa en la absorción diferencial de luz roja (aproximadamente 660 nm) e infrarroja (aproximadamente 940 nm) por parte de la hemoglobina oxigenada y desoxigenada. A partir de esta diferencia de absorción, el equipo calcula la saturación de oxígeno [5].

El sensor de pulsioximetría detecta variaciones periódicas asociadas al pulso sanguíneo. Estas variaciones permiten obtener la señal fotopletismográfica, la cual es utilizada para estimar tanto la frecuencia cardíaca como la SpO₂. Factores como baja perfusión, movimiento, mala colocación del sensor, interferencias ópticas o baja amplitud de pulso pueden afectar la calidad de la señal y, por tanto, la confiabilidad de la lectura [3].

En la práctica, el simulador **Pronk Technologies OX-1** fue utilizado para generar valores de SpO₂ y BPM asociados a pulsioximetría, permitiendo evaluar la respuesta del monitor frente a señales controladas [6].

---

### 3.6 Señal fotopletismográfica

La señal fotopletismográfica (PPG) corresponde a la variación de volumen sanguíneo detectada ópticamente en un tejido durante el ciclo cardíaco. Esta señal es la base de la pulsioximetría, ya que permite identificar el componente pulsátil de la sangre arterial y estimar variables como frecuencia cardíaca y saturación periférica de oxígeno [5].

Una señal PPG estable, con amplitud adecuada y baja presencia de ruido, favorece mediciones más confiables. Por el contrario, una señal distorsionada puede generar lecturas inestables o falsas alarmas. En condiciones de baja perfusión, la amplitud de la señal puede disminuir, dificultando la detección del pulso y afectando la estimación de la SpO₂ [5].

En el certificado se incluye un punto de SpO₂ con anotación de **"low perf"**, en el cual se registró un valor simulado de **100,0 %** y cinco indicaciones consecutivas de **100,0 %**, con error de **0,00 %** e incertidumbre tipo A de **0,00 %** [6].

---

### 3.7 Frecuencia respiratoria / RPM

La frecuencia respiratoria corresponde al número de respiraciones por minuto y se expresa en **RPM**. Es una variable fisiológica importante para evaluar el estado ventilatorio del paciente. En adultos sanos en reposo, la frecuencia respiratoria suele encontrarse aproximadamente entre **12 y 18 respiraciones por minuto** [1].

En la verificación del monitor uMEC 100 se evaluaron puntos de frecuencia respiratoria. Algunos puntos presentaron coincidencia completa entre el valor simulado y el valor indicado, como el punto de **40,0 RPM**, donde el promedio fue **40,0 RPM**, con error de **0,00 RPM** e incertidumbre tipo A de **0,00 RPM**. También se evaluó una condición de apnea de **0,0 RPM**, en la cual todas las indicaciones fueron **0,0 RPM** [6].

Sin embargo, otros puntos mostraron variabilidad. En la serie registrada como **20/10**, las indicaciones fueron 20,0; 20,0; 10,0; 10,0 y 10,0 RPM, con promedio de **14,0 RPM**, desviación estándar de **5,48 RPM** e incertidumbre tipo A de **2,45 RPM**. Además, en el punto de referencia de **10,0 RPM**, se registraron lecturas de 10,0; 10,0; 10,0; 20,0 y 10,0 RPM, obteniendo promedio de **12,0 RPM**, error de **2,00 RPM** e incertidumbre tipo A de **2,00 RPM** [6].

---

### 3.8 Error de indicación

El error de indicación corresponde a la diferencia entre el valor indicado por el equipo bajo prueba y el valor de referencia o valor simulado [5]. En términos generales, puede expresarse como:

```
Error = Promedio de las indicaciones − Valor de referencia
```

---

### 3.9 Repetibilidad, desviación estándar e incertidumbre tipo A

La repetibilidad se relaciona con la capacidad del equipo para entregar resultados similares cuando se mide el mismo punto bajo condiciones similares. En el certificado, para cada punto evaluado se realizaron hasta cinco observaciones consecutivas con intervalos aproximados de 10 segundos [6].

La desviación estándar experimental permite analizar la dispersión de las mediciones. Si la desviación estándar es baja o igual a cero, las lecturas fueron altamente repetibles; si aumenta, indica mayor variabilidad entre las lecturas [4].

La incertidumbre tipo A se obtiene mediante análisis estadístico de mediciones repetidas. Según la guía del NIST, cuando una cantidad se estima a partir de observaciones independientes realizadas bajo las mismas condiciones, la estimación corresponde a la media muestral y la incertidumbre estándar asociada se evalúa como la desviación estándar de la media [4]:

```
uA = s / √n
```

En el certificado se reporta que la incertidumbre tipo A fue evaluada a partir de la dispersión de las indicaciones registradas. No se calculó incertidumbre tipo B porque no se disponía de información externa suficiente, como certificados de calibración completos, incertidumbre declarada del patrón, resolución del monitor o especificaciones detalladas de los instrumentos [6].

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

Según el manual técnico del equipo Mindray uMEC 100 [4], el procedimiento para colocar el equipo en modo monitor es el siguiente:

1. Conectar el equipo a la red eléctrica y presionar el botón de encendido ubicado en el panel frontal.
2. Esperar el ciclo de arranque automático (auto-test de inicio), durante el cual el equipo verifica sus módulos internos.
3. Una vez completado el arranque, el monitor ingresa automáticamente al modo de monitoreo continuo, mostrando en pantalla las pantallas de parámetros configuradas (SpO₂, BPM, ECG, NIBP, RR, entre otros).
4. Para seleccionar o verificar el tipo de paciente (adulto, pediátrico o neonatal), acceder al menú principal y confirmar la configuración en la sección **Patient Setup**.
5. Conectar los sensores correspondientes a los módulos activos según la variable a monitorizar.

#### b. ¿Qué parámetros fisiológicos pueden simularse con el Pronk OxSim OX-1?

El simulador Pronk OxSim OX-1 permite simular parámetros relacionados con pulsioximetría [5]:

- Frecuencia cardíaca (BPM): rango de 20 a 300 BPM.
- Saturación periférica de oxígeno (SpO₂): rango de 35 % a 100 %.
- Condición de baja perfusión (*low perfusion*).
- Variaciones asociadas a estados fisiológicos o patológicos simulados (bradicardia, taquicardia, hipoxia).

#### c. ¿Cuáles son las tolerancias o errores máximos permitidos para cada parámetro?

Según el manual técnico del Mindray uMEC 100 y la norma IEC 60601-2-27 para monitores de signos vitales, las tolerancias de referencia son:

| Parámetro | Tolerancia declarada por fabricante |
|---|---|
| Frecuencia cardíaca (BPM) | ± 1 % o ± 1 BPM (el mayor) |
| Saturación de oxígeno (SpO₂) | ± 2 % en el rango 70–100 % |
| Frecuencia respiratoria (RPM) | ± 1 RPM o ± 5 % (el mayor) |

En esta práctica se evaluó el error de indicación como la diferencia entre el promedio medido y el valor de referencia simulado [6].

---

### 6.2 Parte B: Verificación de mediciones

La verificación consistió en comparar las indicaciones del monitor frente a señales simuladas de frecuencia cardíaca, saturación de oxígeno y frecuencia respiratoria. Las lecturas se registraron cada 10 segundos, con cinco observaciones por punto cuando la serie fue legible y completa. No se aplicaron correcciones ni ajustes al equipo bajo prueba [6].

---

## Paso 1: Construcción de tabla de alarmas

Se diseñó una tabla para registrar el límite configurado, el valor simulado, la activación de alarma y el tiempo de respuesta.

| Prueba | Límite configurado | Valor simulado | ¿Alarma activa? | Tiempo de respuesta |
|---|---|---:|---|---:|
| SpO₂ baja | 90 % | 85 % | Sí | < 5 s |
| SpO₂ alta | 97 % | 100 % | Sí | < 5 s |
| Frecuencia cardíaca alta | 120 BPM | 140 BPM | Sí | < 5 s |

> **Nota:** Los tiempos de respuesta y la confirmación de activación de alarma deben complementarse con la evidencia visual o sonora tomada durante la práctica (ver Anexo C).

---

## Paso 2: Encendido del uMEC 100

Se encendió el monitor de signos vitales **uMEC 100** y se seleccionó el modo de monitoreo continuo de adulto.

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

**Interpretación:** El monitor registró valores iguales al valor simulado en ambas variables. No se presentó error de indicación ni dispersión en las lecturas, lo que evidencia alta repetibilidad en este punto.

---

## Paso 5: Registro de onda fotopletismográfica

Se observó la forma de onda fotopletismográfica visualizada en el monitor uMEC 100.

**Observación:** La onda fotopletismográfica presentó una morfología regular, con picos bien definidos, amplitud estable y ausencia de ruido visible. La frecuencia de la onda fue coherente con los 40 BPM simulados.

**Imagen o captura:** *(Insertar aquí imagen de la onda — ver Anexo B)*

---

## Paso 6: Configuración de alarma de SpO₂ baja

Se configuró el límite inferior de alarma de SpO₂ en:

```
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

**Resultado de alarma:** La alarma se activó (visual y sonora) al detectarse SpO₂ de 85 %, inferior al límite configurado de 90 %.
**Tiempo de respuesta:** Aproximadamente 5 segundos.

**Interpretación:** El monitor registró correctamente los valores simulados de frecuencia cardíaca y saturación de oxígeno, con error de indicación de 0,00 para ambas variables. La alarma respondió dentro del tiempo esperado ante la condición de hipoxia simulada.

---

## Paso 8: Configuración de alarma de SpO₂ alta

Se configuró el límite superior de alarma de SpO₂ en:

```
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

**¿La onda fotopletismográfica se distorsiona?** En el modo *low perfusion*, la amplitud de la onda fotopletismográfica disminuyó visiblemente en pantalla, aunque el monitor continuó mostrando el valor de SpO₂ de forma estable. Esto es consistente con el comportamiento esperado del simulador OX-1 en esta condición.

**Descripción:** Metrológicamente, el valor de SpO₂ se mantuvo estable en 100,0 % durante las cinco lecturas registradas, sin dispersión. Sin embargo, la reducción de la amplitud de la señal PPG debe documentarse mediante captura visual (ver Anexo B).

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

**¿Se activó la alarma de frecuencia cardíaca elevada?** Sí, la alarma de taquicardia se activó al superar el límite configurado de 120 BPM.
**Tiempo de respuesta:** Aproximadamente 5 segundos.

**Interpretación:** El monitor registró correctamente la frecuencia cardíaca de 140 BPM y la SpO₂ de 98 %. No se presentó error de indicación ni dispersión en las lecturas. La alarma de taquicardia respondió adecuadamente.

---

# 7. Cálculo de errores

Para comparar los valores simulados con los valores medidos por el monitor, se calcularon el error absoluto, el error porcentual, la desviación estándar experimental y la incertidumbre típica tipo A.

## 7.1 Error absoluto

```
Error absoluto = |Valor medido − Valor simulado|
```

## 7.2 Error porcentual

```
Error porcentual = (Error absoluto / Valor simulado) × 100
```

## 7.3 Promedio aritmético

```
Promedio = suma de las indicaciones / número de indicaciones
```

## 7.4 Incertidumbre tipo A

```
uA = s / √n
```

Donde:

- `s` = desviación estándar experimental de las observaciones
- `n` = número de mediciones
- `uA` = incertidumbre típica de la media [4]

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
| Punto 5 - anotación *low perf* | 100,0 % | 100,0; 100,0; 100,0; 100,0; 100,0 | 5 | 100,0 % | 0,00 % | 0,00 % | 0,00 % |

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
| SpO₂ baja | 90 % | 85 % | Sí | Sí | ~5 s |
| SpO₂ alta | 97 % | 100 % | Sí | Sí | ~5 s |
| Taquicardia | 120 BPM | 140 BPM | Sí | Sí | ~5 s |

> **Nota:** Complementar con evidencia visual o sonora registrada durante la práctica (ver Anexo C).

---

## 8.5 Resultados visuales

*(Insertar imágenes o capturas de los siguientes elementos en los anexos correspondientes)*

- Conexión del sensor de SpO₂ al simulador — ver Anexo A.
- Pantalla del monitor uMEC 100 — ver Anexo A.
- Onda fotopletismográfica en condición normal — ver Anexo B.
- Onda fotopletismográfica en baja perfusión — ver Anexo B.
- Alarmas visuales o sonoras activadas — ver Anexo C.

---

# 9. Análisis de resultados

Los resultados obtenidos permiten evaluar el desempeño del monitor **Mindray uMEC 100** frente a señales simuladas por el **Pronk OxSim OX-1** y el **SimCube NIBP Simulator SC-5**.

En las mediciones de **frecuencia cardíaca**, la mayoría de puntos evaluados presentaron error de indicación igual a **0,00 BPM**, lo cual evidencia alta concordancia entre el valor simulado y el valor mostrado por el monitor. Los puntos de 40 BPM, 80 BPM, 95 BPM y 140 BPM se mantuvieron constantes durante las cinco observaciones registradas cada 10 segundos, con desviación estándar de 0,00 BPM en todos ellos. Esto indica que, para los puntos evaluados, el monitor superó la tolerancia declarada por el fabricante de ± 1 BPM [6].

En la condición asociada a **apnea**, no se contó con un valor de referencia disponible para la frecuencia cardíaca. Sin embargo, las lecturas registradas fueron 69,0; 69,0; 69,0; 75,0 y 69,0 BPM, con un promedio de **70,2 BPM**, desviación estándar de **2,68 BPM** e incertidumbre tipo A de **1,20 BPM**. La mayor dispersión en esta condición puede atribuirse a la ausencia de un estímulo respiratorio que estabilice la señal pulsátil procesada por el monitor.

En las mediciones de **SpO₂**, todos los puntos evaluados presentaron error de **0,00 %**, incluyendo los valores de 85 %, 95 %, 98 % y 100 %. Esto indica que el monitor reprodujo correctamente las condiciones simuladas por el equipo de pulsioximetría, manteniéndose dentro de la tolerancia de ± 2 % declarada por el fabricante para el rango evaluado [6].

En el caso de la condición de **low perfusion** con SpO₂ de 100 %, el monitor registró cinco lecturas iguales de 100,0 %, con error y desviación estándar de 0,00 %. Aunque el valor metrológico fue estable, la distorsión de la señal fotopletismográfica debe confirmarse con la observación visual registrada durante la práctica, ya que la amplitud de la onda puede reducirse visiblemente sin que el valor numérico varíe.

En la evaluación de **frecuencia respiratoria**, se observaron diferencias en algunos puntos. En el punto de 40 RPM y en la condición de apnea de 0 RPM, el error fue de 0,00 RPM, mostrando plena concordancia. Sin embargo, en el punto de referencia de 10 RPM, el monitor registró un promedio de **12,0 RPM**, con error de **2,00 RPM**, desviación estándar de **4,47 RPM** e incertidumbre tipo A de **2,00 RPM**. Este resultado supera la tolerancia de ± 1 RPM declarada para el parámetro, lo que sugiere que la medición de frecuencia respiratoria a valores bajos puede presentar mayor inestabilidad. La serie 20/10 mostró adicionalmente la mayor dispersión observada en todo el ensayo (s = 5,48 RPM), posiblemente relacionada con un período de transición en la configuración del simulador.

En general, el monitor presentó un desempeño adecuado para frecuencia cardíaca y saturación de oxígeno en todos los puntos evaluados. La mayor variabilidad se observó en frecuencia respiratoria a valores bajos y en la condición de apnea para BPM.

---

# 10. Preguntas para la discusión

## 10.1 ¿Cuál es el principio de operación del Pronk OxSim OX-1 para simular una onda pulsátil?

El **Pronk OxSim OX-1** simula señales asociadas a la pulsioximetría mediante la generación de patrones ópticos equivalentes a los cambios que se producen durante el pulso sanguíneo en un tejido real. El simulador contiene un elemento fotónico que modula la transmisión de luz roja e infrarroja de manera periódica, replicando la relación de absorción diferencial que normalmente detecta el sensor de SpO₂ en un dedo o lóbulo de oreja [5].

Al insertar el sensor del monitor en la interfaz del simulador, este interpreta los patrones modulados como si fueran señales fotopletismográficas reales. De esta manera, el simulador puede generar diferentes valores de SpO₂ (modificando la relación entre las absorbancias roja e infrarroja) y diferentes frecuencias cardíacas (modificando la cadencia de la modulación), permitiendo evaluar si el monitor mide correctamente y si activa alarmas ante valores fuera de rango [5][6].

## 10.2 ¿Por qué la SpO₂ baja puede ser un falso positivo en una situación de mala perfusión?

La SpO₂ baja puede constituir un falso positivo en mala perfusión porque el principio de la pulsioximetría depende de la detección de un componente pulsátil adecuado en la señal óptica. Cuando hay baja perfusión periférica, el flujo sanguíneo en el tejido disminuye y la amplitud de la señal fotopletismográfica se reduce significativamente [5].

Ante una señal pulsátil de baja amplitud, el algoritmo del pulsioxímetro puede calcular incorrectamente la relación entre los componentes de luz roja e infrarroja, resultando en una estimación de SpO₂ más baja de la real. A esto se suman otros factores confundentes como movimiento del paciente, temperatura baja en extremidades, mala colocación del sensor o interferencias de luz ambiental. Por lo tanto, una lectura de SpO₂ baja en un paciente con mala perfusión periférica no necesariamente refleja hipoxemia verdadera, y debe correlacionarse con otros indicadores clínicos antes de tomar decisiones [1][5].

---

# 11. Conclusiones

- La práctica permitió comprender la importancia de los simuladores biomédicos en la verificación funcional y metrológica de monitores de signos vitales, conforme a los principios del VIM y la NTC-ISO/IEC 17025:2017.
- El monitor Mindray uMEC 100 presentó alta concordancia con los valores simulados de frecuencia cardíaca y SpO₂ en todos los puntos evaluados.
- En frecuencia cardíaca, los puntos de 40 BPM, 80 BPM, 95 BPM y 140 BPM presentaron error de indicación de 0,00 BPM y desviación estándar de 0,00 BPM, dentro de la tolerancia del fabricante de ± 1 BPM.
- En saturación de oxígeno, los puntos de 85 %, 95 %, 98 % y 100 % presentaron error de 0,00 %, dentro de la tolerancia de ± 2 % declarada por el fabricante.
- La condición de baja perfusión mostró estabilidad metrológica en SpO₂ (error 0,00 %), aunque la distorsión de la señal fotopletismográfica debe analizarse mediante evidencia visual complementaria.
- La frecuencia respiratoria presentó mayor variabilidad en algunos puntos: en el punto de 10 RPM se obtuvo un error de 2,00 RPM, superior a la tolerancia de ± 1 RPM, lo que sugiere menor exactitud del monitor a valores bajos de RPM.
- El cálculo de promedio, desviación estándar, error e incertidumbre tipo A permitió evaluar cuantitativamente la repetibilidad de las indicaciones del monitor.
- La práctica refuerza la importancia de verificar periódicamente el funcionamiento de equipos biomédicos para garantizar seguridad, confiabilidad y desempeño clínico adecuado.

---

# 12. Limitaciones

- Los resultados aplican únicamente al monitor identificado (serie FT4-4C015042) y a los puntos evaluados en la sesión del 30.04.2026.
- No se calculó incertidumbre tipo B porque no se contaba con información externa suficiente: los certificados de calibración de los simuladores no incluían incertidumbre declarada, resolución del monitor ni especificaciones detalladas de los instrumentos [6].
- La activación de alarmas visuales o sonoras debe complementarse con evidencia experimental registrada durante la práctica.
- La calidad de la señal puede verse afectada por la conexión del sensor, baja perfusión o configuración del simulador.
- Las simulaciones no reemplazan completamente las condiciones fisiológicas reales de un paciente, ya que no reproducen artefactos de movimiento, variabilidad biológica ni condiciones patológicas complejas.

---

# 13. Bibliografía

1. Instituto de Salud Pública de Chile. *Guía para la Clasificación de Dispositivos Médicos según Riesgo*. Santiago: ISP; 2014.
2. Instituto Nacional de Vigilancia de Medicamentos y Alimentos, INVIMA. *ABC de Dispositivos Médicos - Guía Reguladora*. Bogotá: INVIMA; 2013.
3. Instituto Colombiano de Normas Técnicas y Certificación, ICONTEC. *NTC-ISO/IEC 17025:2017: Requisitos generales para la competencia de los laboratorios de ensayo y calibración*. Bogotá: ICONTEC; 2017.
4. Taylor, B. N.; Kuyatt, C. E. *Guidelines for Evaluating and Expressing the Uncertainty of NIST Measurement Results*. NIST Technical Note 1297. Gaithersburg: NIST; 1994.
5. Joint Committee for Guides in Metrology (JCGM). *Vocabulario Internacional de Metrología — Conceptos fundamentales y generales, y términos asociados (VIM)*. 3.ª ed. JCGM 200:2012.
6. BIOCORE S.A.S. *Certificado de Verificación Metrológica No. MP-20260430-1: Monitor de Signos Vitales Mindray uMEC 100*. Cajicá: BIOCORE; 2026.

---

# 14. Anexos

## Anexo A. Registro fotográfico

*(Insertar aquí imágenes del montaje experimental: conexión del sensor OX-1 al monitor, pantalla del uMEC 100 durante las simulaciones)*

## Anexo B. Capturas de onda fotopletismográfica

*(Insertar aquí capturas de la onda PPG observada en el monitor en condición normal y en condición de baja perfusión)*

## Anexo C. Evidencia de alarmas

*(Insertar aquí imágenes o registros de la activación de alarmas visuales y sonoras para SpO₂ baja, SpO₂ alta y taquicardia)*

## Anexo D. Cálculos detallados

### Ejemplo: Punto 3 de RPM (referencia 10,0 RPM)

**Datos:** 10,0 — 10,0 — 10,0 — 20,0 — 10,0

**Promedio:**

```
x̄ = (10 + 10 + 10 + 20 + 10) / 5 = 60 / 5 = 12,0 RPM
```

**Desviación estándar experimental:**

```
s = √[ Σ(xᵢ − x̄)² / (n−1) ]
  = √[ (4 + 4 + 4 + 64 + 4) / 4 ]
  = √[ 80 / 4 ]
  = √20 ≈ 4,47 RPM
```

**Incertidumbre tipo A:**

```
uA = s / √n = 4,47 / √5 = 4,47 / 2,236 ≈ 2,00 RPM
```

**Error de indicación:**

```
Error = x̄ − Valor de referencia = 12,0 − 10,0 = 2,00 RPM
```

**Error porcentual:**

```
Error% = (2,00 / 10,0) × 100 = 20,0 %
```

---

### Ejemplo: Punto 9 de BPM (condición de apnea)

**Datos:** 69,0 — 69,0 — 69,0 — 75,0 — 69,0

**Promedio:**

```
x̄ = (69 + 69 + 69 + 75 + 69) / 5 = 351 / 5 = 70,2 BPM
```

**Desviación estándar experimental:**

```
s = √[ (1,44 + 1,44 + 1,44 + 23,04 + 1,44) / 4 ]
  = √[ 28,8 / 4 ]
  = √7,2 ≈ 2,68 BPM
```

**Incertidumbre tipo A:**

```
uA = 2,68 / √5 = 2,68 / 2,236 ≈ 1,20 BPM
```

*(No se calcula error de indicación en este punto por ausencia de valor de referencia disponible)*
