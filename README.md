# Substack Dossier — muestras reales

Informes de *due diligence* de publicaciones de Substack, generados automáticamente a partir de **datos públicos**
(archivo público de la publicación y su HTML público). Este repositorio contiene **muestras reales** generadas por la
herramienta el **2026-09-17**, en español e inglés.

## Muestras

| Publicación | ES | EN | Lectura |
|---|---|---|---|
| Noahpinion (economía, ~458.000 suscriptores declarados, franja de pago declarada) | [PDF](noahpinion-es.pdf) | [PDF](noahpinion-en.pdf) | publicación grande con datos completos |
| Error500 (tecnología, ~9.000 suscriptores declarados, **sin** franja de pago declarada) | [PDF](error500-es.pdf) | [PDF](error500-en.pdf) | publicación menor: el informe dice «sin dato» en lugar de estimar |

El Markdown intermedio de cada informe está en `md/`, para que el contenido sea auditable sin abrir el PDF.

## Qué incluye un informe

Seis bloques, calculados sobre los **últimos 12 meses** de archivo público:

1. **Perfil** — nombre, URL, suscriptores declarados, franja de pago publicada, primer post analizado.
2. **Cadencia** — posts por mes, día de la semana más frecuente, tendencia (3 meses frente a los 9 anteriores).
3. **Participación** — mediana y p90 de reacciones, comentarios y restacks; reacciones por suscriptor declarado;
   tendencia y los 5 posts con más tracción.
4. **Muro de pago** — porcentaje de posts solo para suscriptores, longitud media de los posts gratuitos frente a los
   de pago, y qué temas se reservan al pago.
5. **Red de recomendaciones** — a quién recomienda y qué recomendaciones son **recíprocas** (verificadas una a una).
6. **Veredicto** — cinco banderas verde/ámbar/rojo con su regla explícita, y la estimación de suscriptores de pago
   **como rango**, nunca como cifra exacta.

## Qué NO incluye (dicho claro)

- **No** accede a la cuenta del autor ni a datos privados: solo datos públicos.
- **No** incluye emails de lectores, ni contenido de pago, ni aperturas, clics o ingresos reales.
- **No** calcula un MRR exacto ni percentiles contra una cohorte de publicaciones: los números son de esa
  publicación y sus propios 12 meses.
- Si la publicación no declara su franja de pago, el informe escribe «sin dato» en lugar de estimar.

## Precios

| Producto | Precio | Cómo pedirlo |
|---|---|---|
| Informe de una publicación | **149 €** | [pagar con tarjeta](https://buy.stripe.com/fZu3cxa0k1XF5ADbkKfrW06) |
| Comparativa de tres publicaciones | **290 €** | [pagar con tarjeta](https://buy.stripe.com/5kQ9AV3BW6dVfbd4WmfrW07) |
| Retainer (4 informes al mes) | **190 €/mes** | [suscribirse](https://buy.stripe.com/00w3cx3BWcCj2or3SifrW08) |

Entrega por email en menos de 24 h, como PDF bilingüe. Si prefieres hablar antes de pagar, escribe a
**jd.robles@gmail.com** indicando la publicación.

---

*Hecho con `substack-dossier`: TypeScript sobre Node 22, sin base de datos, 1 petición por segundo y caché diaria.
Los datos de archivo cambian a diario; cada informe lleva su fecha de corte.*
