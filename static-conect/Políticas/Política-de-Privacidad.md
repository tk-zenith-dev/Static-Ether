# Política de Privacidad de Static Ether

**Última actualización:** 22 de Noviembre de 2026 (Versión 1.1.20)

En **Static Ether**, respetamos profundamente tu privacidad y estamos totalmente comprometidos a proteger tus datos personales y la seguridad de tu dispositivo. Esta Política de Privacidad explica de forma transparente cómo opera la aplicación **Static Ether** y confirma nuestro compromiso inquebrantable de cero recopilación de datos (Zero-Logs).

---

## 1. Operación 100% Local y Cero Recopilación de Datos (No-Logs Policy)

- **Sin Registro de Actividad:** Static Ether **NO recopila, NO almacena y NO transmite** ningún tipo de información personal, historial de navegación, nombres de dominio consultados, consultas DNS, direcciones IP o identificadores de dispositivo.
- **Procesamiento en Dispositivo:** Todo el procesamiento, análisis e inspección profunda de paquetes (DNS, SNI TLS y QUIC) se realiza íntegramente en la memoria RAM local de tu dispositivo a través de un motor nativo C++20 optimizado con cero fugas de memoria.
- **Sin Seguimiento de Terceros:** La aplicación no incluye SDKs de publicidad, ni herramientas de analítica intrusiva o rastreo (como Google Analytics, Firebase Analytics, AdMob o Facebook SDK).

---

## 2. Declaración del Permiso `VpnService` de Android

Static Ether requiere y utiliza el permiso `VpnService` de Android bajo las siguientes condiciones estrictas:

1. **Uso Exclusivo como Bucle Local (Local Loopback TUN):** El servicio crea una interfaz virtual de red en tu dispositivo (`10.255.0.1`) para inspeccionar localmente el tráfico y aplicar las reglas de bloqueo declaradas por el usuario.
2. **Sin Redirección Externa:** La aplicación **NO redirige tu tráfico de internet a ningún servidor VPN remoto, proxy o servidor de terceros**. Todo el tráfico permitido viaja directamente hacia su destino original.
3. **Privacidad de IP:** La aplicación no altera, no oculta ni enmascara tu dirección IP pública ante servidores de internet externos.
4. **Propósito:** El único objetivo del uso de `VpnService` es permitir el filtrado de red de alto rendimiento para neutralizar publicidad abusiva, telemetría y rastreadores sin requerir permisos de superusuario (root).

---

## 3. Seguridad y Cifrado de Datos en Tránsito

- **Actualización de Reglas:** La aplicación realiza solicitudes HTTPS seguras cifradas con protocolo TLS 1.3 hacia el repositorio público oficial en GitHub únicamente para verificar y descargar actualizaciones periódicas de las bases de datos de filtrado (`version.json`, `ads.json` y `telemetry.json`).
- **Sin Información Identificable:** Estas solicitudes de actualización no contienen token de usuario, identificador de dispositivo ni información personal.

---

## 4. Almacenamiento y Protección de Datos en el Dispositivo

- **Operación Continua e Ilimitada:** Static Ether opera de forma 100% continua 24/7 sin temporizadores restrictivos, sin cuotas diarias y sin paywalls.
- **Persistencia Local:** Los únicos datos almacenados en el dispositivo son las bases de datos de reglas compiladas (`active_rules.bin`), perfiles de configuración seleccionados por el usuario y preferencias de tema e idioma en el almacenamiento privado de la app (`/data/data/com.tkzenith.staticether/files/`).

---

## 5. Eliminación de Datos

Dado que **Static Ether no recopila ni almacena ningún dato de usuario en servidores remotos**, no existen datos de usuario guardados en la nube para eliminar. Al desinstalar la aplicación de tu dispositivo, se eliminarán automáticamente todos los archivos de configuración local.

---

## 6. Cambios en esta Política de Privacidad

Nos reservamos el derecho de actualizar esta Política de Privacidad periódicamente. Cualquier cambio significativo será publicado en esta misma página con la fecha de actualización correspondiente.

---

## 7. Contacto y Soporte

Si tienes alguna pregunta o inquietud sobre esta Política de Privacidad o las prácticas de seguridad de Static Ether, puedes ponerte en contacto con nosotros a través de nuestro repositorio oficial de GitHub:

- **Repositorio GitHub:** [https://github.com/tk-zenith-dev/Static-Ether](https://github.com/tk-zenith-dev/Static-Ether)
