# Historia de Usuario (Plantilla en Borrador)  

**Proceso:** Gestión de Apoyo Documental  
**Área:** Fábrica de Software  
**Código:** FS-VSD-001  
**Versión:** 1.0.0.0  

---

## Nombre de la HU  

**HU – [MÓDULO] – [CONSECUTIVO] – [NOMBRE DE LA FUNCIONALIDAD]**  

- **HU:** Indica que es una *Historia de Usuario*.  
- **[MÓDULO]:** Corresponde al módulo del sistema (Ejemplo: CER = Certificados).  
- **[CONSECUTIVO]:** Número asignado de forma consecutiva (Ejemplo: 001).  
- **[NOMBRE DE LA FUNCIONALIDAD]:** Nombre descriptivo de la funcionalidad.  

---

## Escenario de la HU  

Formato estándar para definir: **quién lo solicita, qué quiere lograr y para qué lo necesita**.  

- **COMO (ROL):** [Perfil o rol del usuario]  
- **QUIERO (OBJETIVO):** [Acción o funcionalidad que desea realizar]  
- **PARA (BENEFICIO):** [Razón o valor que obtiene]  

---

## 1. Control de Versiones del Documento  

| Versión   | Descripción del Cambio                   | Autor       | Fecha de Versión |
|-----------|-------------------------------------------|-------------|------------------|
| 1.0.0.0   | Creación inicial de la HU                 | [Nombre]    | [dd/mm/aaaa]     |
| 0.1.0.0   | Actualización de criterios de aceptación  | [Nombre]    | [dd/mm/aaaa]     |

---

## 2. Referencias Externas  

| No. | Nombre del Anexo          | Archivo                    | Descripción                              |
|-----|---------------------------|----------------------------|------------------------------------------|
| 1   | [Ejemplo: Mockup pantalla certificados] | Mockup_Certificados_v1.png | Imagen de la interfaz para descargar certificados |

---

## 3. Especificación de las Historias de Usuario  

### 3.1 Historias de Usuario Asociadas  
HU-XXX – [Nombre de la HU relacionada].  

### 3.2 Precondiciones  
- [Precondición 1]  
- [Precondición 2]  

### 3.3 Flujo Normal de Trabajo  

| Paso | Actor | Acción | Respuesta del Sistema |
|------|-------|--------|-----------------------|
| 1    | Usuario | Ingresa a la plataforma CUN 360 | El sistema muestra opciones de ingreso |

### 3.4 Flujos Alternos  

**FA-01 – [Título descriptivo del flujo alterno]**  

| Paso | Actor | Acción | Respuesta del Sistema |  
|------|-------|--------|-----------------------|  

---

## 3.5 Excepciones  

**EX-01 – [Título descriptivo de la excepción]**  

| Paso | Actor | Acción | Respuesta del Sistema |  
|------|-------|--------|-----------------------|  

---

## 3.6 Campos  

| Nombre del Campo        | Tipo de Campo      | Obligatorio | Longitud | Observaciones |
|--------------------------|--------------------|-------------|----------|---------------|
| Tipo de documento        | Lista desplegable  | Sí          | NA       | Campo de Entrada |
| Número de documento      | Numérico           | Sí          | 12       | Campo de Entrada |
| Nombres y Apellidos      | Texto              | Sí          | NA       | Campo de Salida |

---

## 3.7 Mockups  

Representaciones gráficas de la interfaz (pantallas, formularios, módulos).  
*Ejemplo: Mockup en Figma de la pantalla “Descargar Certificados”*.  

---

## 4. Reglas de Negocio  

- **RN01 – [Título descriptivo]:** [Explicación detallada].  
- **Ejemplo: RN01 – Acceso autorizado por rol:** Solo usuarios con rol administrativo activo pueden acceder al módulo.  

---

## 5. Criterios de Aceptación  

1. El sistema debe permitir el acceso solo a funcionarios administrativos activos con cuenta institucional.  
2. Al iniciar sesión, se debe mostrar el módulo "Certificados".  
3. Si no se diligencian campos obligatorios, se debe mostrar el mensaje “Este campo es requerido”.  
4. El sistema debe permitir generar y descargar certificados en PDF.  

---
