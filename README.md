# Segundo Parcial Redes de Computadores

# 1. Simulación de Congestión en Redes de Datos y Evaluación del Comportamiento del Protocolo TCP

## Descripción del problema
En una red de datos, la congestión ocurre cuando los nodos o enlaces dentro de la red no pueden manejar adecuadamente el tráfico de datos, lo que resulta en pérdidas de paquetes, aumento de la latencia y reducción del rendimiento general. El protocolo TCP (Transmission Control Protocol) juega un papel crucial en la gestión de esta congestión, ya que ajusta dinámicamente el flujo de datos mediante mecanismos como el control de congestión, ventanas deslizantes y retransmisiones de paquetes perdidos.

## Objetivo del ejercicio
Simular una red de datos utilizando la herramienta ns-3 para observar y analizar el comportamiento del protocolo TCP bajo condiciones de congestión. El objetivo es identificar cómo TCP maneja la congestión y evalúa su rendimiento en términos de tiempo de respuesta, throughput (rendimiento) y pérdida de paquetes.

## Escenario de simulación
1. Crear una topología de red sencilla que contenga al menos dos nodos de envío (nodos fuente) y dos nodos receptores conectados a través de un enlace central compartido con ancho de banda limitado.
2. Utilizar tráfico TCP desde los nodos fuente a los nodos receptores.
3. Introducir condiciones de congestión controlando el ancho de banda del enlace central y la cantidad de tráfico que los nodos fuente generan, excediendo la capacidad del enlace.
4. Medir el impacto de la congestión en el rendimiento del protocolo TCP, evaluando las métricas clave: throughput, tiempo de latencia, y pérdida de paquetes.

## Puntos clave a evaluar
- Cómo TCP adapta la tasa de envío cuando se detecta congestión (congestión evitada o experimentada).
- Comparación de distintos algoritmos de control de congestión de TCP (Reno, Cubic, etc.) en la misma simulación.
- Impacto en la calidad de servicio (QoS) para los usuarios finales.

## Requisitos
- Utilizar ns-3 para configurar la red y generar los escenarios de congestión.
- Implementar diferentes variantes del protocolo TCP y capturar métricas como la tasa de pérdida de paquetes, tiempo de respuesta y throughput.
- Analizar los resultados mediante gráficos que evidencien el comportamiento de TCP en diferentes situaciones de congestión.

# 2. Evaluación del Concepto de Conmutación de Paquetes utilizando Switches

## Descripción
En las redes de datos, la conmutación de paquetes es el proceso mediante el cual los datos se dividen en pequeños paquetes y se envían de manera independiente a través de la red. Los switches desempeñan un papel clave en la conmutación de paquetes, ya que dirigen estos paquetes de manera eficiente a través de la red hacia su destino final.

En este ejercicio, se simulará una red de switches que conecta varios dispositivos. El objetivo es observar el proceso de conmutación de paquetes y cómo los switches manejan el tráfico en la red, mejorando la eficiencia de la transmisión de datos.

## Objetivo del ejercicio
El propósito de este ejercicio es entender el funcionamiento de los switches en un entorno de conmutación de paquetes y analizar su impacto en la eficiencia del envío de datos dentro de una red.

## Instrucciones
1. Crear una red de datos que incluya al menos tres switches y seis dispositivos finales distribuidos de manera que cada switch interconecte varios dispositivos (simule los nodos como switches).
2. Generar tráfico de red entre los dispositivos finales, simulando múltiples flujos de datos simultáneamente.
3. Evaluar cómo los switches gestionan el tráfico, analizando el enrutamiento de los paquetes entre los dispositivos finales.
4. Simular un escenario de congestión y evaluar cómo los switches manejan este tráfico, analizando métricas como el throughput y el tiempo de latencia.
5. Comparar los resultados de la simulación con el caso de una red de hubs, destacando las ventajas de los switches en la conmutación de paquetes.

## Entregables
- Implementar la simulación utilizando NS-3.
- Generar métricas de rendimiento como el throughput, latencia y pérdida de paquetes.
- Realizar un análisis comparativo del rendimiento de la red cuando se utilizan switches frente a hubs.



# 3.Evaluación del Concepto de VLAN en Redes de Datos

## Descripción
Las VLANs (Virtual Local Area Networks) son una tecnología de red que permite dividir una red física en múltiples redes lógicas independientes. Las VLANs son utilizadas para mejorar la eficiencia, seguridad y administración de una red, separando el tráfico de diferentes grupos de trabajo o departamentos dentro de una misma infraestructura de red física. A través de este ejercicio, se evaluará cómo las VLANs permiten segmentar el tráfico, reducir la congestión y mejorar la seguridad de una red.

## Objetivo del ejercicio
Simular una red que utilice VLANs para segmentar el tráfico entre diferentes grupos de usuarios y evaluar el comportamiento del tráfico en la red, observando los beneficios de la segmentación en términos de seguridad y eficiencia.

## Instrucciones
1. Configurar una red con al menos dos switches y seis dispositivos finales, distribuidos en tres VLANs. Cada VLAN debe representar un departamento o grupo de trabajo diferente (por ejemplo, Administración, Finanzas, y Recursos Humanos).
2. Asignar cada dispositivo final a una VLAN específica, de manera que solo los dispositivos dentro de la misma VLAN puedan comunicarse entre sí.
3. Implementar el uso de un router o switch con enrutamiento entre VLANs para permitir la comunicación entre los dispositivos de las diferentes VLANs.
4. Generar tráfico de red entre dispositivos dentro de la misma VLAN y observar cómo se aísla el tráfico de las otras VLANs.
5. Generar tráfico entre dispositivos de VLANs diferentes a través del enrutamiento entre VLANs y medir el impacto en el rendimiento de la red.

## Puntos clave a evaluar
- La segmentación del tráfico entre las VLANs y cómo esta mejora la seguridad al aislar el tráfico de diferentes grupos.
- El uso de enrutamiento entre VLANs y su impacto en el rendimiento de la red.
- La comparación de una red con VLANs frente a una red sin segmentación, observando la congestión y la seguridad en ambos casos.

## Entregables
- Utilizar Cisco Packet Tracer o GNS3 para configurar y simular las VLANs.
- Generar métricas como throughput, latencia y pérdida de paquetes tanto dentro de las VLANs como entre ellas.
- Analizar los beneficios y limitaciones del uso de VLANs en una red de tamaño mediano.



