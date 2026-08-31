# AI FrontDesk — sitio público

Descripción del servicio y páginas legales de AI FrontDesk.

Existe por un motivo concreto: **el registro A2P 10DLC de EE. UU. exige que un revisor de la
operadora pueda abrir, sin cuenta, la descripción del opt-in de SMS y los enlaces a privacidad y
términos.** La campaña se rechazó una vez con el error **30909** justamente porque esas URLs no
existían.

| Página | Para qué |
|---|---|
| `sms/index.html` | Divulgación del programa de SMS. **Es la que revisa la operadora.** |
| `privacy/index.html` | Política de privacidad |
| `terms/index.html` | Términos del servicio |

Sitio estático, sin build. Se publica con GitHub Pages desde `main`.

## Si editas `sms/index.html`

Mantén estos cinco elementos o la campaña volverá a caer:

1. cómo da el consentimiento el usuario (aquí: iniciado por el propio cliente, que escribe primero),
2. qué mensajes recibe y con qué frecuencia,
3. el aviso de que pueden aplicarse tarifas,
4. las palabras **STOP** y **HELP**,
5. los enlaces a privacidad y términos.

El mismo texto vive también como rutas `/privacy`, `/terms` y `/sms` en la aplicación
(repo privado `aifrontdesk-ai`). Si cambias uno, cambia el otro.
