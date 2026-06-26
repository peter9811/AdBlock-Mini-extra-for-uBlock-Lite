# 🧩 AdBlock Mini – Lista de filtros extra para uBlock Origin

> **Complemento ligero** para bloquear anuncios, rastreadores y telemetría que no siempre cubren las listas estándar.

## 📌 ¿Para quién es esto?

- **Para usuarios de uBlock Origin (MV2)** en Firefox, Brave, o Chromium antiguo – puedes suscribirte a esta lista externa.
- **Para usuarios de uBlock Lite (MV3)** – esta lista **no se puede añadir directamente**, pero puedes usar el modo de filtrado **"Complete"** en sitios problemáticos, o cambiar a uBlock Origin si tu navegador lo permite.
- **Para usuarios de AdGuard, AdBlock Plus** – compatible con el formato estándar de filtros.

## 🚀 Cómo suscribirse

Copia y pega este enlace en la configuración de tu bloqueador:

```
https://raw.githubusercontent.com/peter9811/AdBlock-Mini-extra-for-uBlock-Lite/main/minifilters.txt
```

### Pasos en uBlock Origin:

1. Abre el panel de uBlock Origin (clic en el icono → ⚙️).
1. Ve a la pestaña **"Listas de filtros"**.
1. Baja hasta **"Importar..."**.
1. Pega la URL y haz clic en **"Aplicar cambios"**.
1. La lista se actualizará automáticamente cada 7 días.

## 📦 Categorías cubiertas

| Categoría                       | Ejemplos                                                            |
| ------------------------------- | ------------------------------------------------------------------- |
| Google / DoubleClick            | `pagead2.googlesyndication.com`, `googleads.g.doubleclick.net`      |
| Amazon                          | `amazon-adsystem.com`, `device-metrics-us.amazon.com`               |
| Microsoft / Bing                | `bat.bing.com`, `settings-win.data.microsoft.com`                   |
| Redes sociales                  | Facebook, Twitter/X, LinkedIn, Instagram, TikTok, Pinterest, Reddit |
| Ad Networks / SSPs              | Criteo, Taboola, Outbrain, MGID, AppNexus, PubMatic, OpenX, etc.    |
| Analítica / Rastreo             | Google Analytics, Hotjar, Mixpanel, Amplitude, Segment, FullStory   |
| Identidad / Data Brokers        | BlueKai, Tapad, ID5, TheTradeDesk                                   |
| Atribución móvil                | AppsFlyer, Adjust, Branch, Kochava, Singular                        |
| Monitoreo de errores            | Sentry, Bugsnag, New Relic, DataDog                                 |
| Minería de criptos              | CoinImp, Webminepool, Minero.cc                |
| Popups / Popunders              | PopAds, PopCash, ExoClick, TrafficJunky                             |
| Fabricantes (telemetría)        | Apple, Huawei, Samsung, Xiaomi, Oppo, Realme, LG                    |
| Smart TVs / Streaming           | Roku, Vizio, LG TV                                                  |
| Gestión de consentimiento (CMP) | OneTrust, Cookiebot, TrustArc, Usercentrics                         |
| Afiliados / Referidos           | Impact, Skimlinks, Viglink, Awin                                    |
| Marketing / Email               | Mailchimp, HubSpot, Marketo, Intercom, Braze, OneSignal, Klaviyo    |
| Anuncios en vídeo               | JW Player, FreeWheel, Connatix, Brightcove, Tremor                  |

## 🛡️ Reglas de excepción (Allowlist)

La lista incluye excepciones para evitar romper sitios populares:

- `@@||www.facebook.com/ajax/ads/` – permite algunos componentes internos de Facebook necesarios.
- `@@||accounts.google.com/adwords/` – permite acceso a servicios de Google Ads.
- `@@||connect.facebook.net^$script` – permite el SDK de Facebook.
- `@@||platform.twitter.com^$script` – permite widgets de Twitter.

Si encuentras un falso positivo, **abra un issue** o envía un pull request.

## 🤝 Contribuir

1. Haz un **fork** del repositorio.
1. Edita `minifilters.txt` (sigue la sintaxis de AdBlock Plus).
1. Envía un **pull request** con tus cambios.
1. Si no estás seguro, abre un **issue** describiendo el dominio o regla problemática.

## 📝 Licencia

MIT © 2026 – Libre para usar, modificar y distribuir.

## 🙏 Agradecimientos

- A la comunidad de EasyList y EasyPrivacy por las referencias.
- A los mantenedores de uBlock Origin por su increíble herramienta.
