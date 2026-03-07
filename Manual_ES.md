# FUSION IV - Documentación Completa

> ⚠️ **AVISO LEGAL**: Este repositorio contiene únicamente documentación de usuario. No se incluye código fuente, algoritmos, lógica backend ni mecanismos de licencia. Cualquier intento de ingeniería inversa del producto está prohibido.

![Version](https://img.shields.io/badge/version-Beta-blue)
![Platform](https://img.shields.io/badge/platform-Garmin%20Connect%20IQ-green)
![API](https://img.shields.io/badge/API-5.0.0%2B-orange)

---

## Tabla de Contenidos

1. [Descripción General](#descripción-general)
2. [Características Principales](#características-principales)
3. [Interfaz de Usuario](#interfaz-de-usuario)
4. [Configuración](#configuración)
   - [Configuración del Sistema](#configuración-del-sistema)
   - [Configuración de Pantalla](#configuración-de-pantalla)
   - [Campos de Datos](#campos-de-datos)
   - [Personalización de Colores](#personalización-de-colores)
   - [Clima](#clima)
5. [Tipos de Datos Disponibles](#tipos-de-datos-disponibles)
6. [Glosario](#glosario)
7. [Apéndices](#apéndices)

7. [Instalación](#instalación)
8. [Soporte y Asistencia](#soporte-y-asistencia)

---

![FUSION IV Banner](docs/images/Banner.jpg)

---

## Descripción General

**FUSION IV** es una esfera de reloj altamente personalizable para relojes Garmin Connect IQ. Diseñado para proporcionar una experiencia de usuario óptima, combina diseño moderno y riqueza funcional con una amplia personalización de todos los elementos en pantalla.


### Características Clave

- ✨ **Interfaz Altamente Personalizable**: 28 colores configurables independientemente
- 📊 **Múltiples Campos de Datos**: 18 zonas de datos configurables
- 🌦️ **Integración del Clima**: Compatible con Garmin Weather y OpenWeatherMap
- ⚡ **Optimización de Batería**: Modos inteligentes de ahorro de energía
- 🌍 **Soporte Multilingüe**: 19 idiomas disponibles
- 🎯 **Metas y Seguimiento**: Barras de progreso para tus objetivos
- 🌙 **Modo Nocturno**: Protección de pantalla configurable

---



## Características Principales

### 1. Visualización de la Hora

- Formato 12h o 24h
- Visualización de segundos (3 modos)
- Cero inicial opcional para las horas
- Soporte AM/PM en formato 12h
- Configuración de colores independiente (horas, minutos, segundos, separadores)

### 2. Campos de Datos Circulares

Cuatro campos de datos circulares posicionados a las 9h, 11h, 1h y 3h alrededor de la esfera del reloj:

- Visualización de valores
- Título personalizable
- Visualización de unidades
- Múltiples modos de visualización
- Colores independientes

### 3. Campos de Datos Clásicos

Seis campos de datos periféricos:

- 3 campos superiores (izquierda, centro, derecha)
- 3 campos inferiores (izquierda, centro, derecha)
- Iconos de colores
- Valores de texto

### 4. Campos de Texto

- Campo de texto superior
- Campo de texto inferior
- Personalización completa del contenido
- Varios modos de visualización

### 5. Indicadores de Información

Cinco indicadores visuales:

1. **Bluetooth**: Estado de conexión del teléfono
2. **Info 2**: Superior izquierda
3. **Info 3**: Superior derecha
4. **Info 4**: Lado izquierdo de la fecha
5. **Info 5**: Lado derecho de la fecha

### 6. Barra de Objetivos

- Visualización gráfica del progreso
- Múltiples tipos de objetivos
- Texto e icono configurables
- Colores personalizables (vacío/lleno/texto)

### 7. Fecha

- 7 formatos de visualización
- Día de la semana
- Soporte de formato internacional
- Color personalizable

### 8. Clima

- **Fuentes**: Garmin Weather y/o OpenWeatherMap
- **Datos Disponibles**:
  - Temperatura actual, sensación térmica, min/max
  - Descripción del clima e icono
  - Humedad
  - Velocidad y dirección del viento
  - Presión atmosférica (OWM)
  - Cobertura de nubes (OWM)
  - Visibilidad (OWM)
  - Probabilidad de precipitación (GW)

---

## Interfaz de Usuario

### Estructura de la Pantalla

![Watch Face Layout](docs/images/Display_Overview_2.png)

*Diseño de visualización de FUSION IV mostrando todas las zonas configurables*

### Modos de Visualización

#### Modo de Visualización Completa
![Full Display](docs/images/Display_1.png)

#### Modo Siempre Activo
![Always Active](docs/images/Layout_Always_Active.png)

#### Modo Protector de Pantalla
![Screen Saver](docs/images/Layout_Screen_Saver.png)

#### AOD (Always On Display)
![AOD Mode](docs/images/Display_AOD.png)

### Leyenda
- **Time**: Visualización de la hora
- **Date**: Visualización de la fecha
- **Circ**: Campos circulares
- **TL/TC/TR**: Campos superiores (Izquierda/Centro/Derecha)
- **BL/BC/BR**: Campos inferiores (Izquierda/Centro/Derecha)
- **I2/I3/I4/I5**: Indicadores de información
- **Goal Bar**: Barra de progreso de objetivos

---

## Configuración

### Configuración del Sistema

#### Frecuencia de Actualización de Datos
Controla la frecuencia de actualización de datos:

- **Full Refresh**: Actualización completa cada segundo (consumo máximo)
- **High Refresh Rate**: Actualización alta
- **Medium Refresh Rate**: Actualización media (recomendado)
- **Low Refresh Rate**: Actualización baja (ahorro de batería)

#### Ahorro de Energía

**Screen Saver Delay**: Tiempo en minutos antes de la activación del protector de pantalla (-1 para desactivar)

**Screen Off Delay**: Tiempo en minutos antes de que la pantalla se apague (-1 para desactivar)

#### Widget

**Launch Widget On Press Hold**: Iniciar widget en pulsación larga (solo pantalla táctil)

---

### Configuración de Pantalla

#### Formato de Hora

**Use Military Format**: 
- `true`: Formato de 24 horas
- `false`: Formato de 12 horas (AM/PM)

**Hours Leading 0**: 
- `true`: Mostrar cero inicial (01, 02, 03...)
- `false`: Sin cero inicial (1, 2, 3...)

**Seconds Display Mode**:
1. **Hidden**: Segundos ocultos
2. **Normal**: Visualización normal de segundos
3. **Always On**: Siempre mostrados (solo no AMOLED)

#### Formato de Fecha

7 modos de visualización disponibles:

1. `[DOW dd Month]`: Lun 15 enero
2. `[DOW dd/mm]`: Lun 15/01
3. `[dd/mm/yyyy]`: 15/01/2026
4. `[DOW Month dd]`: Lun enero 15
5. `[Month dd DOW]`: enero 15 Lun
6. `[DOW mm/dd]`: Lun 01/15
7. `[yyyy/mm/dd]`: 2026/01/15

---

### Campos de Datos

#### Configuración para Cada Campo

Para cada campo de datos, puedes configurar:

1. **Tipo de Datos**: Elegir entre más de 73 tipos (ver sección de Tipos de Datos)
2. **Título Personalizado**: Texto libre para reemplazar el título predeterminado
3. **Modo de Visualización**: Cómo mostrar los datos

#### Modos de Visualización

##### Campos Circulares (9h, 11h, 1h, 3h)

0. **Value**: Solo valor
1. **Title + Value**: Título encima del valor
2. **Value + Unit**: Valor con unidad
3. **Value + Title**: Valor con título debajo
4. **Title + Value + Unit**: Título, valor, unidad

##### Campos de Texto (Superior/Inferior)

0. **Value**: Solo valor
1. **Title + Value**: Título y valor
2. **Value + Unit**: Valor con unidad
3. **Value + Title**: Valor con título
4. **Title + Value + Unit**: Título, valor, unidad

##### Barra de Objetivos

- **Display Goal Bar Icon**: Mostrar icono
- **Display Goal Bar Text**: Mostrar texto
- **Goal Bar Text Display Mode**: Modo de visualización de texto:
  - 0. **Value**: Solo valor
  - 5. **Title**: Solo título
  - 6. **Goal**: Visualización de objetivo
  - 7. **Value / Goal**: Valor sobre objetivo
  - 8. **Percents Of Goal**: Porcentaje de objetivo
  - 9. **Remaining**: Restante para alcanzar el objetivo
- **Goal Range**: Rango personalizado (min/max) - vacío para usar objetivo del sistema

---

### Personalización de Colores

FUSION IV ofrece **28 colores personalizables**:

#### Colores Base

| ID | Elemento | Descripción |
|----|---------|-------------|
| 0 | Background Color | Color de fondo de la esfera del reloj |
| 1 | Circular Arcs Color | Color de los arcos circulares |
| 2 | Circular Fields Sep Color | Color de los separadores de campos circulares |

#### Colores de Campos Circulares

| ID | Elemento |
|----|---------|
| 3 | Circular Fields Value Color |
| 4 | Circular Fields Title/Unit Color |

#### Colores de la Hora

| ID | Elemento |
|----|---------|
| 5 | Time Hours Color |
| 6 | Time Sep Color (separador) |
| 7 | Time Minutes Color |
| 8 | Time Seconds & AM/PM Color |

#### Colores de Fecha

| ID | Elemento |
|----|---------|
| 9 | Date Color |

#### Colores de Texto

| ID | Elemento |
|----|---------|
| 10 | Top Text Color |
| 11 | Bottom Text Color |

#### Colores de Indicadores

| ID | Elemento |
|----|---------|
| 12 | Info Off Color |
| 13 | Info 1 On Color (Bluetooth) |
| 14 | Info 2 On Color (Superior Izquierda) |
| 15 | Info 3 On Color (Superior Derecha) |
| 16 | Info 4 Color (Lado Izquierdo de Fecha) |
| 17 | Info 5 Color (Lado Derecho de Fecha) |

#### Colores de Campos Clásicos

| ID | Elemento |
|----|---------|
| 18 | Classic Fields X6 Text Color |
| 19 | Top Left Field Icon Color |
| 20 | Top Center Field Icon Color |
| 21 | Top Right Field Icon Color |
| 22 | Bottom Left Field Icon Color |
| 23 | Bottom Center Field Icon Color |
| 24 | Bottom Right Field Icon Color |

#### Colores de Barra de Objetivos

| ID | Elemento |
|----|---------|
| 25 | Goal Bar Off Color |
| 26 | Goal Bar On Color |
| 27 | Goal Bar Text Color |

### Paleta de Colores Predefinidos

La esfera del reloj ofrece **67 colores predefinidos** organizados por familia.

➡️ **[Ver lista completa de colores](https://pay.b65dev.com/portfolio/faqs#faq-colors)**

### Opciones Especiales de Color

**Use Battery Adaptative Color**: Adapta automáticamente el color según el nivel de batería

**Use Weather Colored Icons**: Colorea los iconos meteorológicos según las condiciones

**Custom Colors**: Define hasta 3 colores personalizados mediante código hexadecimal (formato: `0xffffff` o `ffffff`)

---

### Clima

#### Configuración del Proveedor

**Weather Provider**: Selección del servicio meteorológico

1. **Garmin Weather (GW)**: Servicio nativo de Garmin
2. **OpenWeatherMap (OWM)**: Servicio externo que requiere clave API
3. **Garmin Weather + OpenWeatherMap**: Prioridad Garmin, complemento OWM
4. **OpenWeatherMap + Garmin Weather**: Prioridad OWM, complemento Garmin

#### OpenWeatherMap

**Weather Key**: Clave API de OpenWeatherMap (máximo 32 caracteres)

Para obtener una clave API:
1. Crea una cuenta en [openweathermap.org](https://openweathermap.org)
2. Genera una clave API gratuita
3. Copia la clave en la configuración

**Weather Call**: Muestra la hora de la última llamada API (solo lectura)

---

### Unidades de Medida

#### Altitud
- Metros (m)
- Pies (ft)

#### Distancia
- Kilómetros (km)
- Millas (mi)
- Millas Náuticas Internacionales (nm)

#### Temperatura
- Celsius (°C)
- Fahrenheit (°F)
- Kelvin (°K)

**Temperature Offset**: Corrección del sensor de temperatura (valor numérico)

#### Presión
- Hectopascal (hPa)
- Milímetros de Mercurio 0°C (mmHg)
- Pulgada de Mercurio 0°C (inHg)

#### Peso
- Kilogramos (kg)
- Libras (lbs)

#### Velocidad del Viento
- Metros / Segundos (m/s)
- Kilómetros / Horas (km/h)
- Millas / Horas (mi/h)
- Nudos (kn)
- Escala Beaufort (bf)

#### Dirección del Viento
- **Degrees Direction**: Visualización en grados (000-360)
- **Cardinal Direction**: Visualización cardinal (N, NE, E, SE, S, SW, W, NW)

---

### Configuración Avanzada

#### Textos Personalizados

**Custom Text 1 Value**: Texto libre para visualización personalizada  
**Custom Text 2 Value**: Segundo texto libre

#### Cuenta Regresiva

**Countdown Target Day**: Fecha objetivo de la cuenta regresiva  
**Countdown Target Hour**: Hora objetivo (formato HH:mm:ss, ej.: 14:30:00)

#### Zonas Horarias

Configuración de 4 zonas horarias adicionales:

- **Time Zone 2**: Formato UTC (ej.: +02:00 o -05:30)
- **Time Zone 3**: Formato UTC
- **Time Zone 4**: Formato UTC
- **Time Zone 5**: Formato UTC

Formato: HH:mm con signo + o - (ej.: `+02:00`, `-05:30`)

#### Conjuntos de Iconos

**Icons Set**:
- **Filled Icons**: Iconos sólidos
- **Outlined Icons**: Iconos con contorno

#### Proporciones de Fuente

Ajusta los tamaños de fuente independientemente (75% a 150%):

- **Date Font Ratio**: Tamaño de fecha (75-130%)
- **Text Font Ratio**: Tamaño de texto (75-130%)
- **Circular Fields Font Ratio**: Tamaño de campos circulares (75-130%)
- **Classic Fields Font Ratio**: Tamaño de campos clásicos (75-130%)
- **Goal Bar Font Ratio**: Tamaño de texto de barra de objetivos (75-150%)

---

## Tipos de Datos Disponibles

FUSION IV soporta **más de 73 tipos de datos diferentes**. Aquí está la lista completa:

### Actividad Física

| Tipo | Descripción |
|------|-------------|
| Active Minutes : Daily | Minutos activos diarios |
| Active Minutes : Weekly | Minutos activos semanales |
| Calories : Daily Burned | Calorías quemadas diarias |
| Calories : Daily Burned Active | Calorías activas quemadas |
| Steps Daily | Conteo de pasos diarios |
| Distance : Daily | Distancia de hoy |
| Distance : Weekly | Distancia de esta semana |
| Floors Climbed : Daily | Pisos subidos hoy |

### Distancias Específicas

| Tipo | Descripción |
|------|-------------|
| Bike Distance : Week | Distancia en bicicleta de la semana |
| Bike Distance : 30 Days | Distancia en bicicleta de 30 días |
| Bike Distance : Current Month | Distancia en bicicleta del mes actual |
| Run Distance : Week | Distancia de carrera de la semana |
| Run Distance : 30 Days | Distancia de carrera de 30 días |
| Run Distance : Current Month | Distancia de carrera del mes actual |
| Pushes | Número de empujones (si está disponible) |
| Pushes Distance Daily | Distancia diaria de empujones |

### Salud y Bienestar

| Tipo | Descripción |
|------|-------------|
| Heart Rate | Frecuencia cardíaca actual |
| Heart Rate Min/Max (4 Hours) | FC min/max durante 4 horas |
| Body Battery | Nivel de batería corporal |
| Stress Level | Nivel de estrés |
| Respiration Rate | Frecuencia respiratoria |
| Oxygen Saturation | Saturación de oxígeno (SpO2) |
| Recovery Time | Tiempo de recuperación (hh:mm) |
| Weight | Peso en kg |

### Rendimiento Deportivo

| Tipo | Descripción |
|------|-------------|
| VO2 Max Cycling | VO2 Max en ciclismo |
| VO2 Max Running | VO2 Max en carrera |
| Race Predictor 5K | Predicción de tiempo 5K |
| Race Predictor 10K | Predicción de tiempo 10K |
| Race Predictor Half Marathon | Predicción de medio maratón |
| Race Predictor Marathon | Predicción de maratón |
| Training Status | Estado de entrenamiento |

### Sistema y Batería

| Tipo | Descripción |
|------|-------------|
| Battery In Days | Vida de batería en días |
| Battery In Percents | Nivel de batería en % |
| Solar Intensity | Intensidad solar |
| Phone Connected | Teléfono conectado |
| Alarms Count | Número de alarmas |
| Notifications Count | Número de notificaciones |
| Move Alert Level | Nivel de alerta de movimiento |
| Do Not Disturb Enabled | No molestar activado |

### Entorno

| Tipo | Descripción |
|------|-------------|
| Altitude | Altitud actual |
| Pressure From Sensor | Presión atmosférica |
| Temperature From Sensor | Temperatura del sensor |

### Clima (Garmin Weather)

| Tipo | Descripción |
|------|-------------|
| Weather Description | Descripción del clima |
| Weather Temperature | Temperatura meteorológica |
| Weather Temperature : Feel | Sensación térmica |
| Weather Temperature : Min / Max | Temperaturas min/max (solo GW) |
| Weather Humidity | Humedad |
| Weather Precipitation Probability | Probabilidad de precipitación (GW) |
| Weather Wind Speed/Direction | Velocidad y dirección del viento |
| Weather GW Update Time | Hora de actualización de Garmin Weather |

### Clima (OpenWeatherMap)

| Tipo | Descripción |
|------|-------------|
| Weather Station | Estación meteorológica (OWM) |
| Weather Clouds Cover | Cobertura de nubes (OWM) |
| Weather Pressure | Presión (OWM) |
| Weather Visibility | Visibilidad (OWM) |
| Weather OWM Update Time | Hora de actualización de OpenWeatherMap |

### Sol y Luna

| Tipo | Descripción |
|------|-------------|
| Sun Event : Daily Sunrise | Amanecer |
| Sun Event : Daily Sunset | Atardecer |
| Sun Event : Next Sun Event | Próximo evento solar |
| Sun Event : Civil Dawn | Amanecer civil |
| Sun Event : Civil Dusk | Anochecer civil |
| Moon Age | Edad de la luna |
| Moon Illumination | Iluminación de la luna |
| Moon Phase | Fase lunar |

### Fecha y Hora

| Tipo | Descripción |
|------|-------------|
| Date | Fecha actual |
| Day Of The Year | Día del año |
| Week Of The Year | Semana del año |
| Time Zone 2 | Zona horaria 2 |
| Time Zone 3 | Zona horaria 3 |
| Time Zone 4 | Zona horaria 4 |
| Time Zone 5 | Zona horaria 5 |
| Countdown | Cuenta regresiva |

### Personalización

| Tipo | Descripción |
|------|-------------|
| Custom Text | Texto personalizado 1 |
| Custom Text 2 | Texto personalizado 2 |
| Hidden Field | Campo oculto |

### Depuración

| Tipo | Descripción |
|------|-------------|
| Debug Data | Datos de depuración |

---

## Licencia y Activación

### Clave de Licencia

**License Key**: Campo para ingresar tu clave de licencia (máximo 15 caracteres)

La esfera del reloj FUSION IV puede funcionar en modo gratuito con algunas limitaciones. Una licencia desbloquea todas las características premium.

### Obtención de una Licencia

Para obtener una clave de licencia:
1. Visita el sitio web del desarrollador
2. Sigue las instrucciones de compra/activación
3. Ingresa la clave en la configuración de la esfera del reloj

### Información de Versión

**Release**: Muestra la versión actual de la esfera del reloj (solo lectura)

---

## Glosario

- **AMOLED**: Tipo de pantalla de diodos orgánicos emisores de luz de matriz activa
- **API**: Interfaz de Programación de Aplicaciones
- **Connect IQ**: Plataforma de Garmin para aplicaciones de terceros
- **GW**: Garmin Weather (servicio meteorológico de Garmin)
- **OWM**: OpenWeatherMap (servicio meteorológico externo)
- **SpO2**: Saturación de oxígeno en sangre
- **VO2 Max**: Consumo máximo de oxígeno
- **UTC**: Tiempo Universal Coordinado

---

## Apéndices

### Formatos de Parámetros

#### Colores Personalizados
Formato hexadecimal: `0xRRGGBB` o `RRGGBB`
- RR = Rojo (00-FF)
- GG = Verde (00-FF)
- BB = Azul (00-FF)

Ejemplo: `0xFF0000` = Rojo puro

#### Zonas Horarias
Formato: `±HH:mm`
- Signo + para Este, - para Oeste
- HH = Horas (00-14)
- mm = Minutos (00 o 30)

Ejemplos:
- `+01:00` = UTC+1 (París)
- `-05:00` = UTC-5 (Nueva York)
- `+05:30` = UTC+5:30 (India)

#### Hora de Cuenta Regresiva
Formato: `HH:mm:ss`
- HH = Horas (00-23)
- mm = Minutos (00-59)
- ss = Segundos (00-59)

Ejemplo: `14:30:00` = 2:30 PM

### Códigos de Fase Lunar

Las fases lunares están numeradas del 0 al 7:
- 0: Luna Nueva
- 1: Creciente
- 2: Cuarto Creciente
- 3: Gibosa Creciente
- 4: Luna Llena
- 5: Gibosa Menguante
- 6: Cuarto Menguante
- 7: Menguante

---

**Última actualización**: 2 de enero de 2026  
**Versión del documento**: 1.0  
**Autor**: Bastos65

---

*Este documento se proporciona "tal cual" sin garantía de ningún tipo. El desarrollador se reserva el derecho de modificar las características y la documentación sin previo aviso.*
