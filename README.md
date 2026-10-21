# Jota Café — landing con carta digital

```
index.html   la página (hero con los 3 platos girando + carta + visítanos)
img/         pancakes, café, tostada (webp recortados) y logo
```

## Publicarla en Cloudflare Pages

Cloudflare → **Workers & Pages → Create → Pages → Connect to Git** → repo `jota-caf-`, y:

| Campo | Valor |
|---|---|
| Production branch | `main` |
| Framework preset | None |
| Build command | *(vacío)* |
| Build output directory | *(vacío)* |

Save and Deploy. Cada push a `main` se publica solo. `_headers` deja las imágenes en caché 30 días.

Para el QR de las mesas, apunta a `…/#carta`: abre directamente en la carta, sin pasar por el hero.

## Confirmar con Jota Café antes de publicar

La carta sale de su ficha de Google, que tiene duplicados con precios distintos. He puesto el
precio más alto en cada caso (mejor sorpresa a favor del cliente que en contra):

| Producto | En Google aparece | Puesto |
|---|---|---|
| Zumo natural / Zumos | 2,20 € y 2,50 € | 2,50 € |
| Caña / Copa de cerveza | 1,90 € y 2,00 € | 2,00 € |
| Tés e infusiones | 2,10 € y 2,20 € | 2,20 € |

Además:
- **Pancakes soufflé**: Google no da precio. Salen sin precio; pedírselo.
- **Tostadas** (5,00 €): ¿es el precio de la media o de la entera? Ahora pone "Media · Entera" y un solo precio.
- **Horario y teléfono**: no los he encontrado publicados; el botón lleva a su ficha de Google Maps.
- "Opción especialidad" y "Café de especialidad" (+0,20 €) eran lo mismo; van fusionados en uno.
- Las fotos de producto son las que nos pasaron; confirmar que pueden usarse en la web.
