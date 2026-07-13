# 🕐 Vida Plena · Asesoría Integral GAR

Aplicación web para asesores de **Grupo Asesores RAM (GNP)** que digitaliza la asesoría consultiva *"Asegura una Vida Plena"*: perfilamiento del prospecto, diagnóstico financiero en vivo, sensibilización con **El Reloj del Patrimonio** y resumen ejecutivo en PDF con llamada a la acción.

## ✨ Funciones
- Wizard guiado de 7 pasos con guion de venta integrado
- Cálculo automático: patrimonio actuarial, faltantes de Vida y GMM, capital de retiro, plazos de metas
- Panel de diagnóstico en tiempo real durante la sesión
- Reporte PDF con perfil, brechas, recomendación, presupuesto y CTA (WhatsApp / agenda)
- Cuentas por asesor con panel de administración y registro de actividad
- Respaldo de asesorías en el Google Drive de cada asesor (OAuth)

## 🚀 Uso
Abre la app publicada (GitHub Pages) o el archivo `index.html` directamente en Chrome/Edge.

Primer acceso del administrador: usuario `admin` · contraseña `GAR2026` → **cámbiala de inmediato en Ajustes** y crea las cuentas de tus asesores en *Equipo y uso*.

## 🔒 Datos
Todo se guarda **localmente en el navegador de cada asesor** (localStorage) y, si se conecta, en su propio Google Drive. Este repositorio no almacena ni transmite información de prospectos.

> ⚠️ El acceso por usuario/contraseña es organizativo, no un sistema de seguridad de servidor: no publiques datos sensibles dentro del código ni subas asesorías (archivos JSON) al repositorio.

## ☁️ Google Drive
1. En [Google Cloud Console](https://console.cloud.google.com) crea un proyecto y habilita **Google Drive API**.
2. Pantalla de consentimiento OAuth → tipo *Externo* → agrega los correos de los asesores como usuarios de prueba.
3. Credenciales → *ID de cliente OAuth* → *Aplicación web* → en **Orígenes de JavaScript autorizados** agrega la URL de tu GitHub Pages (ej. `https://tuusuario.github.io`).
4. Pega el Client ID en la app: *Ajustes → Google Drive* (solo visible para admin).

## 🛠️ Stack
HTML + CSS + JavaScript vanilla en un solo archivo. Sin dependencias, sin build, sin servidor.

---
© Grupo Asesores RAM · Herramienta interna de asesoría. Documento de diagnóstico; no constituye cotización formal.
