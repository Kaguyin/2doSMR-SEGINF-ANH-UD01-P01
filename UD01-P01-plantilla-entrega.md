# Entrega Práctica UD01 · Auditoría y fortificación Clínica Dental Sonrisas

- **Nombre y apellidos del alumno/a: Aitor Nieto Haro**
- **Grupo:** 2º SMR
- **Fecha de realización: 24 Noviembre 2026**

---

### Actividad 1 · Mecanismos y objetivos de la seguridad informática

1. El objetivo de seguridad principal es el de Confidencialidad.
2. Según el elemento: Lógica, ya que se refiere a un error de Software el cual permite el acceso a documentos remotamente a usuarios no permitidos
3. Activa, ya que es una herramienta  la cuál siempre debe de estar activa y no actuar cuando ocurre una entrada irregular a ciertos usuarios los cuales no tienen la entrada permitida** 

| ID | Mecanismo | Objetivo principal (C, I, D, NR) | Física / Lógica | Activa / Pasiva | Justificación |
|:--|:---|:---:|:---:|:---:|:---|
| 1.1 | SAI servidor | D |F| A | Debido a que siempre debe de estar en funcionamiento, y es un elemento de hardware físico|
| 1.2 | Cifrado BitLocker | C| L| A | Debido a que la informacion es confidencial de la empresa, no todo el mundo debe de tener permitido el acceso a la misma, el bitlocker salta para identificar al usuario que va a acceder a la información|
| 1.3 | Cortafuegos perimetral | C|L | A| Para que nadie acceda desde el exterior al sistema servidor en el cual se guardan todos los datos|
| 1.4 | Copias de seguridad NAS | D|L |P | Para crear un respaldo en caso de perdida de todos los archivos |
| 1.5 | Antivirus corporativo | C | L | A| Un sistema de seguridad que permite que nadie que no tenga autorización entre o intente entrar de forma irregular o se ejecuten programas no deseados como Malware en general|

---

### Actividad 2 · Cadena del incidente de seguridad

1. **Activos afectados:**
   - Activo 1: El servidor el cual tenía los datos (se encontraba desactualizado el sistema de seguridad)
   - Activo 2: Los datos de los clientes que fueron robados, el atacante borró los datos de los pacientes del servidor, también guardó una copia en su propio equipo.
2. **Amenaza:** Persona atacante externa Hacker (uso de exploit público)
3. **Vulnerabilidad y clasificación:** Conocida en software instalado ya que existe una version actualizada la cual permite a los atacantes de NO entrar.
4. **Riesgo previo:** La versión se encontraba vieja por lo que encontrabamos fallos de seguridad
5. **Ataque:** Aprovechamiento de software incorrecto
6. **Impacto:**
   - Impacto cuantitativo: El coste de las perdidas que ha supuesto la perdida del contenido
   - Impacto cualitativo: 

---

### Actividad 3 · Plan de contingencia

1. **Clasificación de medidas:**
   - Medida A: Respaldo
   - Medida B: Respaldo
   - Medida C: Recuperación
   - Medida D: De emergencia
   - Medida E: Recuperación
   - Medida F: Respaldo
2. **Diferencia entre plan de respaldo y plan de recuperación:**
 Rspaldo: actúa antes de que se de el incidente para asegurar la NO perdida o filtración del contenido
 Recuperación: Actúa después de la tragédia, entra en vigor una vez necesitamos recuperar lo perdido/filtrado/secuestrado etc...
---

### Actividad 4 · Software malicioso y test de intrusión

#### 4.1. Diagnóstico de malware
- **Caso 1:**
  - Tipo de malware: Troyano 
  - Justificación (archivo anfitrión e intervención usuario): debido a que se necesita la instalación en el equipo para luego actuar, al principio para en programa legítimo ya que se esta haciendo pasar por un .zip, luego se acaba desmostrando que en realidad es un .exe (programa ejecutable) se debe de descargar manualmente para intervenir maliciosamente.
- **Caso 2:**
  - Tipo de malware: Gusano
  - Justificación (archivo anfitrión e intervención usuario): Debido a que la red usada no era segura y se coló aprovechando un fallo no parcheado en el protocolo de compartición de archivos (SMB). No hace falta que el usuario descargué nada en el equipo infectado.
- **Medida preventiva para Caso 2:** La principal sería añadir un cortafuegos para que atacantes no consigan ingresar irregularmente a la misma, por otro lado aprovecharia la situacion para hacer una comprobacion de todos los equipos, actualizar en caso de que no lo esten y usar un sistema verificado de seguridad contra atacantes. 

#### 4.2. Secuenciación de test de intrusión
- Secuencia ordenada cronológicamente (letras):
- Fases correspondientes:
  - Acción: W Fase ...3 
  - Acción : X Fase ...2
  - Acción :  Y Fase ...4
  - Acción :  Z Fase ...1

---

### Actividad 5 · Contraseñas e identificación digital

#### 5.1. Contraseñas
1. **Comparativa de seguridad frente a fuerza bruta:** Seguridad frente nos asegura escribir simbolos numberos y letras para reforzar nuestra contraseña, la resistencia aumenta con la longitud y la variedad de caracteres.

2. **Política de contraseñas (3 reglas):**
   - Regla 1: Cifrado
   - Regla 2: Autenticación de los extremos
   - Regla 3: Control de acceso

#### 5.2. Identificación digital
3. **Mecanismos aplicados:**
   - Trámite A: Documento electrónico que este vincula
identidad verificada y claves, lo emite una autoridad de
certificación

   - Trámite B: Vincula a una persona con el contenido de
un documento, este aporta autoría, integridad
y no repudio
4. **Objetivo de seguridad garantizado y diferencia con usuario/contraseña:**
La principal diferencia es que hay una entidad la cuál debe de corroborar que somos nostros los cuales estamos ejerciendo X acción, como por ejemplo firmar un documento electrónicamente, ya que si solo actua la contraseña de seguridad, si alguien consigue esa contraseña, cualquier persona puede hacerse pasar por nosotros