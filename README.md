# 🛡️ Proyecto Cerberus  
Nada entra. Nada escapa. Todo está vigilado.  

![SC-900 Certified](https://img.shields.io/badge/Microsoft%20SC--900-Certified-blue)
![Azure](https://img.shields.io/badge/Microsoft%20Azure-Cloud%20Security-0078D4?logo=microsoftazure)
![IAM](https://img.shields.io/badge/Identity%20%26%20Access%20Management-IAM-orange)
![Zero Trust](https://img.shields.io/badge/Zero%20Trust-Security-green)

Proyecto de prácticas de seguridad en **Microsoft Entra ID (Azure AD)** enfocado en el uso de **Acceso Condicional**, **roles administrativos**, **MFA avanzado** y **Zero Trust**.

---

## 🎥 Vídeo explicativo
[Ver video de presentación](./videos/video-cerberus.mp4)

---

## 🖼️ Banner / Imagen Principal
![Proyecto Cerberus](./imagenes/proyecto-cerberus.png)

---

## 📌 Objetivos del Proyecto
- Implementar un sistema de seguridad multinivel inspirado en la metáfora de **Cerberus con 4 cabezas**.  
- Aplicar parámetros reales de **Acceso Condicional**, **MFA avanzado** y **roles administrativos**.  
- Documentar un flujo de seguridad corporativa como ejemplo práctico de **IAM (Identity & Access Management)**.

> [!IMPORTANT]
> Este proyecto es un **laboratorio educativo** para practicar conceptos de seguridad.  
> No debe aplicarse directamente en entornos de producción sin las debidas validaciones.

---

## 🔑 Configuración en 4 Cabezas

🟥 **Cabeza 1 – Usuarios y Roles**  
- Asignación de **roles RBAC diferenciados en la suscripción de Azure**:
  - **Propietario**: control total.  
  - **Colaborador**: administración parcial.  
  - **Lector**: acceso de solo lectura.  
- Separación clara de privilegios para prevenir riesgos de escalada.

> [!WARNING]
> Nunca te asignes restricciones que puedan bloquear tu propia cuenta de administrador.  
> Siempre prueba las políticas con un usuario de prueba antes de aplicarlas a toda la organización.

---

🟨 **Cabeza 2 – Bloqueo por Ubicación**  
- Directiva para **restringir accesos fuera de México**.  
- Configuración de **ubicación con nombre (México)** como zona confiable.  
- Usuarios fuera de esta ubicación no pueden autenticarse.

> [!TIP]
> Define al menos **dos ubicaciones seguras** (ejemplo: oficina y ciudad principal) para evitar perder acceso si tu IP cambia inesperadamente.

---

🟩 **Cabeza 3 – MFA Obligatorio**  
- Aplicación de **autenticación multifactor (MFA)** como requisito para acceder a recursos.  
- Implementación de:
  - **Microsoft Authenticator**.  
  - **Códigos de verificación temporales**.

> [!IMPORTANT]
> El **MFA no es opcional**: reduce más del **90% de los ataques de robo de credenciales**.

> [!NOTE]
> En este laboratorio se utilizó **Microsoft Authenticator**, pero puedes combinarlo con otros factores de autenticación compatibles.

---

🟦 **Cabeza 4 – Niveles de Autenticación**  
- Creación del nivel **Cerberus Nivel Ultra**:
  - **MFA sin contraseña** (Windows Hello, FIDO2, Authenticator passwordless).
  - **MFA resistente al phishing** (credenciales seguras).
- Aplicado a **usuarios críticos** para máxima protección.

> [!TIP]
> Aplica este nivel solo a **cuentas críticas** (administradores, finanzas, seguridad) para equilibrar protección y experiencia de usuario.

---

## 📊 Resultados
- Seguridad escalada en **capas**.  
- Control granular por **rol**, **ubicación**, **factor de autenticación** e **intensidad**.  
- Ejemplo práctico de cómo **Zero Trust** se aplica en entornos reales.

> [!NOTE]
> Este laboratorio fue diseñado como **ejemplo educativo** y puede extenderse con más directivas, informes o integraciones de seguridad.

---

## 🖥️ Arquitectura Lógica de Cerberus

```text
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐    ┌──────────────────┐
│   CABEZA 1      │    │    CABEZA 2      │    │    CABEZA 3     │    │    CABEZA 4      │
│  Roles RBAC     │ -> │ Named Locations  │ -> │ MFA Obligatorio │ -> │ Authentication   │
│ (Suscripción)   │    │   (Solo México)  │    │                 │    │   Strength       │
└─────────────────┘    └──────────────────┘    └─────────────────┘    └──────────────────┘
         │                       │                        │                       │
         └───────────────────────┼────────────────────────┼───────────────────────┘
                                 ▼
                    ┌─────────────────────────┐
                    │     ACCESO SEGURO       │
                    │    Zero Trust Applied   │
                    └─────────────────────────┘
🗂️ Estructura del Repositorio

/docs
 → Documentación detallada de cada directiva.

/imagenes
 → Capturas de referencia y banner del proyecto.

/videos
 → Video explicativo del proyecto.

README.md
 → Resumen ejecutivo del proyecto.

🚀 Tecnologías

Microsoft Entra ID (Azure AD)

Acceso Condicional

Microsoft Authenticator

Passwordless (FIDO2 / Windows Hello)

📌 Autor

Geovana Martínez Sepúlveda
Estudio de caso en Identity & Access Management (IAM) con Microsoft Azure.

📜 Licencia

Este proyecto está bajo la Licencia MIT.
