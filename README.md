# 🛡️ Proyecto Cerberus
Nada entra. Nada escapa. Todo está vigilado.

Proyecto de prácticas de seguridad en **Microsoft Entra ID (Azure AD)** enfocado en el uso de **Acceso Condicional, roles administrativos, MFA avanzado y Zero Trust**.

---

## 🎥 Vídeo explicativo
👉 [Ver video de presentación](./video-cerberus.mp4)

---

## 🖼️ Banner / Imagen Principal
![Proyecto Cerberus](./proyecto-cerberus.png)

---

## 📌 Objetivos del Proyecto
- Implementar un sistema de seguridad multinivel inspirado en la metáfora de **Cerberus con 4 cabezas**.  
- Aplicar parámetros reales de **Acceso Condicional, MFA avanzado y roles administrativos**.  
- Documentar un flujo de seguridad corporativa como ejemplo práctico de **IAM (Identity & Access Management)**.  

> [!IMPORTANT]  
> Este proyecto es un laboratorio **educativo** para practicar conceptos de seguridad.  
> No debe aplicarse directamente en entornos de producción sin las debidas validaciones.

---

## 🔑 Configuración en 4 Cabezas

### 🟥 Cabeza 1 – Usuarios y Roles
- Asignación de roles diferenciados en la cuenta de facturación:  
  - **Propietario**: control total.  
  - **Colaborador**: administración parcial.  
  - **Lector**: acceso de lectura.  

> [!WARNING]  
> Nunca te asignes restricciones que puedan bloquear tu propia cuenta de administrador.  
> Siempre prueba las políticas con un **usuario de prueba** antes de aplicarlas a toda la organización.

---

### 🟨 Cabeza 2 – Bloqueo por Ubicación
- Directiva para restringir accesos fuera de **México**.  
- Configuración de ubicación confiable (ej. *México*).  
- Usuarios fuera de esta zona **no pueden autenticarse**.  

> [!TIP]  
> Define al menos **dos ubicaciones seguras** (ejemplo: oficina y ciudad principal).  
> Así evitas perder acceso si tu IP cambia inesperadamente.

---

### 🟩 Cabeza 3 – MFA Obligatorio
- Aplicación de **MFA** como requisito para acceder a recursos.  
- Implementación con:  
  - Microsoft Authenticator  
  - Códigos de verificación temporales  

> [!IMPORTANT]  
> El **MFA no es opcional**, reduce más del **90% de los ataques de robo de credenciales**.

> [!NOTE]  
> En este laboratorio se usó **Microsoft Authenticator**,  
> pero puedes combinarlo con otros factores compatibles.

---

### 🟦 Cabeza 4 – Niveles de Autenticación
- Creación del nivel **Cerberus Nivel Ultra**:  
  - MFA sin contraseña (Windows Hello, FIDO2, Authenticator sin contraseña).  
  - MFA resistente al phishing.  
- Aplicado a usuarios críticos para máxima protección.  

> [!TIP]  
> Aplica este nivel **solo a cuentas críticas** (administradores, finanzas, seguridad).  
> Así balanceas seguridad sin afectar a todos los usuarios.

---

## 📊 Resultados
- Seguridad **escalada en capas**.  
- Control granular por rol, ubicación, factor de autenticación e intensidad.  
- Ejemplo práctico de cómo **Zero Trust** se aplica en entornos reales.  

> [!NOTE]  
> Este laboratorio fue diseñado como ejemplo **educativo**.  
> Puede extenderse con más directivas, informes o integraciones.

---

## 🗂️ Estructura del Repositorio
