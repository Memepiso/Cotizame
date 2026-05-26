# ⚡ Delivery S.O.S™ 🏍️ — Cotízame
### 🎁 Herramienta gratuita y libre para deliveries independientes de Honduras

---

## ¿Qué es esto?

Un cotizador web profesional que podés usar **gratis** desde tu celular. Tu cliente abre un enlace, selecciona el servicio, marca origen y destino en el mapa, ve el precio desglosado y al confirmar **te llega todo directo a tu WhatsApp** con la ubicación, indicaciones y detalles del pedido.

Sin apps. Sin pagos. Sin instalaciones. Solo un enlace.

---

## 🚀 Cómo usarlo en 10 minutos

### Opción A — Usar este mismo repositorio (la más fácil)

1. Creá una cuenta gratis en **github.com**
2. Entrá a este repositorio y tocá **Fork** (arriba a la derecha)
3. Activá GitHub Pages: Settings → Pages → Branch: main → Save
4. Tu enlace queda: `https://tu-usuario.github.io/cotizame`
5. Editá el archivo `index.html`, buscá esta línea:

```
const WA_NEGOCIO = "50487371300";
```
6. Cambiá ese número por el tuyo (con código de país, sin espacios ni guiones):
```
const WA_NEGOCIO = "50498765432";
```
7. Guardá con Commit changes. ¡Listo!

---

### Opción B — Crear tu propio repositorio desde cero

1. Descargá el archivo `index.html` de este repositorio
2. Creá un repositorio nuevo en GitHub llamado `cotizame`
3. Subí el archivo y renombralo `index.html`
4. Activá GitHub Pages en Settings → Pages
5. Cambiá el número de WhatsApp como se indica arriba

---

### Opción C — Netlify (sin cuenta de GitHub)

1. Entrá a **netlify.com/drop**
2. Descargá y modificá el `index.html` con tu número
3. Arrastrá el archivo a Netlify Drop
4. Te genera un enlace instantáneo gratis

---

## ✏️ Personalizaciones básicas

Abrí el archivo `index.html` y buscá estas líneas para personalizarlo:

```javascript
// Tu número de WhatsApp (con 504, sin espacios)
const WA_NEGOCIO = "50487371300";

// Tu nombre y marca
const LOGO_NAME = "⚡Delivery S.O.S™ 🏍️";
```

Para cambiar tu logo, reemplazá la imagen en la etiqueta:
```html
<img src="TU_LOGO_AQUI" alt="Tu nombre">
```

---

## 💰 ¿Puedo cambiar los precios?

Sí. Buscá en el código la sección `// TARIFAS` y ajustá los valores según tu zona y competencia:

```javascript
const T = {
  mensajeria: {
    rangos: [
      {hasta:3,  base:55},  // 0 a 3 km → L.55
      {hasta:6,  base:75},  // 3 a 6 km → L.75
      ...
    ]
  }
}
```

---

## 🛍️ Servicios incluidos

- 📦 Mensajería con paradas múltiples y tipos de carga
- 🛵 Moto Taxi exclusivo para mujeres
- 📋 Trámites y gestiones (bancos, IHSS, SAR, RENAVIH, notarías)
- Extras: lluvia, nocturno, feriado, urgente, zona de riesgo, fuera de ciudad

---

## 🗺️ Tecnologías libres utilizadas

| Tecnología | Licencia | Uso |
|---|---|---|
| Leaflet.js | BSD-2-Clause | Mapas |
| OpenStreetMap | ODbL | Datos del mapa |
| Nominatim | ODbL | Búsqueda de direcciones |
| Google Fonts | SIL OFL 1.1 | Tipografía |

100% código abierto. Libre para uso comercial personal.

---

## ❓ Preguntas frecuentes

**¿Funciona sin internet?**
No, necesita conexión para cargar el mapa.

**¿El cliente puede pagar desde aquí?**
No, solo cotiza. El pago se coordina por WhatsApp.

**¿Puedo usarlo en Tegucigalpa o Choloma?**
Sí, el mapa funciona en toda Honduras. Solo ajustá las tarifas a tu zona.

**¿Necesito saber programar?**
Solo para cambiar el número y el nombre. Son dos líneas de texto, nada más.

---

## 📞 Proyecto original

**⚡Delivery S.O.S™ 🏍️** · San Pedro Sula, Honduras
WhatsApp: [+504 8737-1300](https://wa.me/50487371300)

*Si te ayudó esta herramienta, compartila con otros deliveries 🤝*