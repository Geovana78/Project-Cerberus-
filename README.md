Project Cerberus: Acceso Condicional en Azure AD con roles, ubicaciones y MFA avanzado.
# 🛡️ Project Cerberus  
**Nada entra. Nada escapa. Todo está vigilado.**

Proyecto de prácticas de seguridad en **Microsoft Entra ID (Azure AD)** enfocado en el uso de **Acceso Condicional** para proteger identidades y accesos críticos dentro de una organización.

---

## 📌 Objetivos del Proyecto
- Implementar un sistema de seguridad multinivel inspirado en la metáfora de "Cerberus con 4 cabezas".
- Aplicar configuraciones reales de **Acceso Condicional**, **MFA avanzado** y **roles administrativos**.
- Documentar un flujo de seguridad corporativa como ejemplo práctico de **IAM (Identity & Access Management)**.

---

## 🔑 Configuración en 4 Cabezas

### 🟥 Cabeza 1 – Usuarios y Roles
- Asignación de **roles diferenciados** en la cuenta de facturación:
  - **Propietario**: control total.  
  - **Colaborador**: administración parcial.  
  - **Lector**: acceso de solo lectura.  
- Separación clara de privilegios para prevenir riesgos de escalamiento.

---

### 🟨 Cabeza 2 – Bloqueo por Ubicación
- Directiva para **restringir accesos fuera de México**.  
- Se configuró **ubicación con nombre (México)** como zona confiable.  
- Usuarios fuera de esta ubicación no pueden autenticarse.

---

### 🟩 Cabeza 3 – MFA Obligatorio
- Aplicación de **Multi-Factor Authentication** como requisito para acceder a recursos.  
- Implementación de:
  - **Microsoft Authenticator**.  
  - **Códigos de verificación temporales**.  
- Refuerzo de la postura de seguridad contra accesos no autorizados.

---

### 🟦 Cabeza 4 – Niveles de Autenticación
- Creación del nivel **Cerberus Nivel Ultra**:  
  - **Passwordless MFA** (Windows Hello, FIDO2, Authenticator sin contraseña).  
  - **MFA resistente a phishing** (credenciales seguras).  
- Aplicado a usuarios críticos para máxima protección.

---

## 📊 Resultados
- Seguridad escalonada en capas.  
- Control granular por rol, ubicación, factor de autenticación e intensidad.  
- Ejemplo práctico de cómo **Zero Trust** se aplica en entornos reales.  

---

## 🗂️ Estructura del Repositorio
- `/docs` → Documentación detallada de cada directiva.  
- `/images` → Capturas de referencia del laboratorio.  
- `README.md` → Resumen ejecutivo del proyecto.  

---

## 🚀 Tecnologías
- **Microsoft Entra ID (Azure AD)**  
- **Acceso Condicional**  
- **Microsoft Authenticator**  
- **Passwordless (FIDO2 / Windows Hello)**  

---

## 📌 Autor
**Geovana Martínez Sepúlveda**  
Estudio de caso en **Identity & Access Management (IAM)** con Microsoft Azure.  
