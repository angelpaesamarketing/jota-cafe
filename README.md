# Jota Café — landing con carta digital

```
public/index.html   la página (hero con los 3 platos girando + carta + visítanos)
public/img/         pancakes, café, tostada, logo 3D y la escena del encargado
                    (encargado/encargado-presenta, clienta/clienta-feliz y tortitas.webp aparte
                    para que el plato pase de la mano a la mesa)
public/_headers     caché de 30 días para las imágenes
wrangler.jsonc      le dice a Cloudflare que publique solo public/
```

## Publicación

Está conectada a Cloudflare Workers (proyecto `jota-cafe`, deploy command `npx wrangler deploy`).
Cada push a `main` se publica solo. Solo sale a internet lo que hay en `public/`: este README no.

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
