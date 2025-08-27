[evidence.md](https://github.com/user-attachments/files/22001739/evidence.md)
# Evidencias & Narrativa

Añade capturas a `/assets` y reférencialas aquí.

1. **Política MFA (Cabeza 1):** `assets/ca-mfa-all-users.png`
2. **Invitada fuera de MX bloqueada (Cabeza 2):** `assets/ca-guest-mx-block.png`
3. **Asignaciones RBAC (Cabeza 3):** `assets/rbac-assignments.png`
4. **Auth Strength Ultra (Cabeza 4):** `assets/auth-strength-ultra.png`
5. **Sign-in logs:** `assets/signin-logs.png`

6. ## 🟨 Evidencia – Cabeza 2: Bloqueo por Ubicación (Fuera de México)

La política de acceso condicional configurada en esta cabeza restringe el inicio de sesión de usuarios cuando la ubicación detectada está fuera de México.  
Esto asegura que únicamente los accesos desde la región designada (MX) sean permitidos como parte del perímetro de confianza.

📎 **Placeholder de captura**:  
![Bloqueo fuera de México](assets/ca-guest-mx-block.png)

> Nota: la imagen será reemplazada posteriormente con la evidencia gráfica tomada desde el portal de Azure AD.
>
> ## 🟩 Evidencia – Cabeza 3: MFA Obligatorio

Se implementó una política de **Multi-Factor Authentication (MFA)** para todos los usuarios, reforzando la seguridad frente a accesos no autorizados.

📎 **Placeholder de captura**:  
![Política MFA](assets/ca-mfa-all-users.png)

---

## 🟦 Evidencia – Cabeza 4: Nivel Ultra de Autenticación

Se creó el nivel **Cerberus Nivel Ultra**, que exige:
- **Passwordless MFA** (Windows Hello, FIDO2, Authenticator sin contraseña).  
- **MFA resistente a phishing** con credenciales seguras.  

📎 **Placeholder de captura**:  
![Nivel Ultra](assets/auth-strength-ultra.png)
