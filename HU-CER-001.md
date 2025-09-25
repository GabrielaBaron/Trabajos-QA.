# Historia de Usuario  

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

Define el contexto y la necesidad del usuario: **quién lo solicita, qué quiere lograr y para qué lo necesita**.  

- **COMO (ROL):** [Perfil o rol del usuario]  
  *Ejemplo: Estudiante activo de la institución.*  

- **QUIERO (OBJETIVO):** [Acción o funcionalidad que desea realizar]  
  *Ejemplo: Descargar mis certificados académicos desde el portal.*  

- **PARA (BENEFICIO):** [Razón o valor que obtiene]  
  *Ejemplo: Tener un soporte oficial de mis estudios sin necesidad de acercarme físicamente.*  

---

## 1. Control de Versiones del Documento  

| Versión   | Descripción                                 | Autor | Fecha de Versión |
|-----------|---------------------------------------------|-------|------------------|
| 1.0.0.0   | Construcción de la HU                       |       |                  |
| 0.1.0.0   | Revisión por parte del área de calidad      |       |                  |
| 0.0.1.0   | Ajustes de acuerdo con observaciones        |       |                  |
| 0.0.0.1   | Revisión inicial por parte del área calidad |       |                  |

---

## 2. Referencias Externas  

| No. | Nombre del Anexo              | Archivo                 | Descripción                       |
|-----|-------------------------------|-------------------------|-----------------------------------|
| 1   | Fuentes de información        | Certificados 360        | Información general de certificados |
| 2   | Fuentes de información (XML)  | Certificados 360.xml    | Tipos de Certificados              |

---

## 3. Especificación de las Historias de Usuario  

### 3.1 Historias de Usuario Asociadas  
HU-XXX – [Nombre de la HU relacionada].  

### 3.2 Precondiciones  
- [Precondición 1]  
- [Precondición 2]  

### 3.3 Flujo Normal de Trabajo  

| Paso | Actor  | Acción | Respuesta del Sistema |
|------|--------|--------|-----------------------|
| 1    | Usuario| [Ejemplo: Ingresa a la plataforma] | [Ejemplo: El sistema muestra opciones de acceso] |

### 3.4 Flujos Alternos  

**FA-01 – [Nombre del flujo alterno]**  
| Paso | Actor | Acción | Respuesta del Sistema |  

---

## 3.5 Excepciones  

**EX-01 – [Descripción de la excepción]**  
| Paso | Actor | Acción | Respuesta del Sistema |  

---

## 3.6 Campos  

| Nombre del Campo      | Tipo de Campo    | Obligatorio | Longitud | Observaciones |
|------------------------|------------------|-------------|----------|---------------|
| Tipo de documento      | Lista selección  | Sí          | NA       | Tipos: CC, CE, TI, PAS, PPT |
| Número de documento    | Numérico         | Sí          | 12       | Entrada obligatoria |
| Nombres y Apellidos    | Texto            | Sí          | NA       | Salida automática del sistema |
| Programa académico     | Lista selección  | Sí          | NA       | Selección de programas cursados |
| Tipo de certificado    | Lista selección  | Sí          | NA       | Opciones disponibles según avance |
| Periodo                | Lista selección  | Sí          | NA       | Periodo académico a consultar |
| Valor del certificado  | Alfanumérico     | Sí          | NA       | Informativo |
| Generar certificado    | Botón acción     | Sí          | NA       | Genera vista previa |
| Descargar certificado  | Botón acción     | Sí          | NA       | Descarga en PDF |

---

## 4. Reglas de Negocio  

- **RN-01:** Acceso autorizado por rol (solo administrativos activos).  
- **RN-02:** Acceso mediante autenticación institucional.  
- **RN-03:** Validación automática de identidad.  
- **RN-04:** Validación de campos obligatorios.  
- **RN-05:** Generación de certificado sujeta a formulario completo.  
- **RN-06:** Vista previa obligatoria antes de descarga.  
- **RN-07:** Descarga en PDF habilitada.  
- **RN-08:** Inclusión obligatoria de código QR.  
- **RN-09:** Verificación de validez por QR o enlace.  
- **RN-10:** Prevención de suplantación.  

---

## 5. Criterios de Aceptación  

1. El sistema permite acceso solo a usuarios administrativos activos.  
2. Al iniciar sesión, el usuario ve el módulo "Certificados".  
3. Al ingresar tipo y número de documento, el sistema autocompleta el nombre.  
4. Campos obligatorios muestran mensaje de error si no se diligencian.  
5. El sistema genera una vista previa antes de la descarga.  
6. El usuario puede descargar el certificado en PDF.  
7. El certificado incluye un código QR único.  
8. La validación por QR o enlace muestra “Certificado Válido” y detalles del documento.  
9. El sistema permite volver a CUN360 desde la validación.  

---
