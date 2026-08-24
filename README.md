# Mis Finanzas — vista web

Página de solo lectura generada desde la app local. Los datos van cifrados con
AES-256-GCM; la llave se deriva del secreto TOTP con PBKDF2-SHA256.

Sin ese secreto este repositorio es un bloque ilegible. El código de 6 dígitos de
Google Authenticator es el segundo factor, no la llave.

No se edita a mano: se regenera con `python app/exportar_web.py` desde el proyecto.
