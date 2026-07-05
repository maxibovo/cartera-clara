# Cartera Clara

Tablero web para cargar una exportacion CSV de Cocos Capital y analizar la composicion del portafolio.

## Version actual

- Marca visual: Cartera Clara.
- Pantalla inicial de producto.
- Navegacion: Inicio, Dashboard e Historial.
- Importacion diaria de CSV.
- Historial local de importaciones.
- Comparacion simple contra la carga anterior.
- Grafico de evolucion del patrimonio.
- Deteccion de cambios por instrumento entre la ultima carga y la anterior.
- Seccion Benchmarks con comparacion manual contra inflacion, dolar MEP, S&P 500 y Merval.
- Reemplazo automatico de importaciones del mismo dia/archivo para evitar duplicados.

## Uso diario

1. Entrar al dominio gratuito de Vercel.
2. Entrar a `Dashboard`.
3. Abrir la seccion `Importacion`.
4. Subir el CSV actualizado exportado desde Cocos Capital.
5. Revisar patrimonio, composicion, liquidez, concentracion y posiciones.
6. Entrar a `Historial` para comparar contra cargas anteriores.
7. Entrar a `Benchmarks` y cargar las variaciones del periodo para comparar rendimiento relativo.

La ultima importacion queda guardada localmente en el navegador de ese dispositivo.
Las comparaciones por instrumento se calculan a partir de importaciones realizadas con esta version o posteriores.

## Publicar en Vercel

1. Entrar a https://vercel.com/new
2. Crear un nuevo proyecto.
3. Subir o importar esta carpeta: `cartera-clara-vercel`.
4. Framework preset: `Other`.
5. Build command: dejar vacio.
6. Output directory: dejar vacio.
7. Deploy.

Vercel va a generar una URL gratis parecida a:

`cartera-clara.vercel.app`

## Publicar con CLI

Si tenes Vercel CLI instalado:

```bash
vercel
vercel --prod
```

## Nota de privacidad

El tablero procesa el CSV en el navegador. En esta version no envia ni guarda datos en un servidor.
