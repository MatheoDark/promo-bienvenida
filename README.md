<!-- prettier-ignore -->
# 🎁 promo-bienvenida

<p align="center">
	<img src="media/Logo.jpeg" alt="Logo" width="160" style="border-radius:12px; box-shadow: 0 8px 30px rgba(0,0,0,0.6);" />
</p>

Landing promocional con estilo moderno, animaciones y CTAs optimizados para campañas de afiliados (1win, Stake y Coolbet).

<p align="center">
	<a href="https://wlcoolbet.adsrv.eacdn.com/C.ashx?btag=a_3299b_124c_&affid=935&siteid=3299&adid=124&c="><img alt="APUESTA GRATIS $15.000" src="https://img.shields.io/badge/⚽-APUESTA%20GRATIS%20%2415.000-brightgreen?style=for-the-badge" /></a>
	&nbsp;
	<a href="https://github.com/MatheoDark/promo-bienvenida"><img alt="Repo" src="https://img.shields.io/badge/Repo-MatheoDark-blue?style=for-the-badge" /></a>
</p>

## Estructura del repositorio

```
promo-bienvenida/
├── index.html      # Landing completa (HTML + CSS + JS en un solo archivo)
├── sitemap.xml     # Sitemap para SEO
├── CNAME           # Dominio personalizado de GitHub Pages
└── media/
    ├── Logo.jpeg                   # Logo 1win
    ├── stake-full.tLL7usOz.svg     # Logo Stake
    └── coolbet/                    # Marca y banners de Coolbet
        ├── coolbet-logo.png        # Logo oficial (usado en loader, sección y footer)
        └── coolbet-fiesta-*.jpg    # Banners Mundial 2026 (hero, franja, vertical, torre...)
```

## Enlaces de afiliado activos

| Plataforma | Producto | Enlace |
|---|---|---|
| **Coolbet** ⭐ principal | Sportsbook CL (adid 124) | `https://wlcoolbet.adsrv.eacdn.com/C.ashx?btag=a_3299b_124c_&affid=935&siteid=3299&adid=124&c=` |
| **Coolbet** ⭐ principal | Casino CL (adid 125) | `https://wlcoolbet.adsrv.eacdn.com/C.ashx?btag=a_3299b_125c_&affid=935&siteid=3299&adid=125&c=` |
| 1win | Registro (código `WINCLP`) — opción 2 | `https://1wjsit.life/?open=register&p=3w9p` |
| Stake | Referido — opción 3 | `https://stake.com/?c=3UsGeLgH` |

Además, la sección Coolbet incluye 3 banners oficiales servidos por iframe (adid 253 · 728x90, adid 255 · 320x160, adid 264 · 300x250) desde `wlcoolbet.adsrv.eacdn.com/I.ashx`.

> **Nota anti-adblock** (no deshacer estas decisiones):
> 1. Los nombres de las imágenes locales evitan patrones de tamaño de banner (`728x90`, `300x250`...) que EasyList filtra por nombre de archivo.
> 2. Los enlaces de Coolbet **no van en el HTML**: EasyList oculta cualquier elemento con `href` hacia `adsrv.eacdn.com`. Se usan `<a href="#" data-cb="sb|ca">` y la URL se construye en JavaScript al hacer click (función `cbUrl` en index.html).
> 3. Si un bloqueador colapsa los iframes oficiales, un script los reemplaza por banners locales con el mismo enlace de registro.

## ¿Qué incluye la landing?

La página funciona con **pestañas por plataforma** (navbar fija con hash routing). Cada pestaña tiene URL propia para compartir en campañas:

| Pestaña | Link directo | Contenido |
|---|---|---|
| 🐻 Coolbet ⭐ (por defecto) | `/#coolbet` | Oferta Mundial 2026, CTAs deportes/casino, banners oficiales, FAQ propio |
| 🎁 1win | `/#1win` | Bono +500%, countdown, juegos, ganadores, niveles, FAQ, testimonios |
| 🎲 Stake | `/#stake` | Referido directo + características (crypto, originals) |
| ⚽ Mundial 2026 | `/#mundial` | Cuenta regresiva real a la Gran Final (19-jul-2026), banners verticales |

Además: diseño responsivo tema neón, CTA fijo de móvil hacia Coolbet, y selector de idioma manual (español por defecto).

## Despliegue

- GitHub Pages: push a la rama `main` (dominio configurado vía `CNAME`).
- Netlify / Vercel: conecta el repo y despliega automáticamente.

## Contribuir

1. Haz fork y crea una rama: `feature/tu-cambio`.
2. Realiza cambios y abre un PR describiendo la intención.

## Avisos legales

- Contenido promocional/afiliado: verifica leyes locales y plataformas.
- Solo para mayores de 18 años. Juega responsablemente.

---
_Hecho por MatheoDark — último cambio: integración Coolbet Mundial 2026_
