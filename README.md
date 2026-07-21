# Cuaderno de Derivadas

Calculadora web de derivadas simbólicas. El usuario escribe cualquier función y la página muestra la derivada (hasta 4º orden), con notación matemática renderizada.

## Características

- Deriva cualquier función que se pueda escribir como expresión matemática: polinomios, trigonométricas, trigonométricas inversas, hiperbólicas, exponenciales, logaritmos, raíces, etc.
- Derivadas de 1º a 4º orden.
- Convención matemática clara: `ln` = logaritmo natural, `log` = logaritmo base 10.
- Paleta de botones con funciones y símbolos comunes, para no tener que memorizar la sintaxis.
- Notación matemática (LaTeX) renderizada con KaTeX, tanto para la función original como para el resultado.
- Historial de las últimas derivadas calculadas, con clic para volver a cargarlas.
- Sin backend: todo el cálculo simbólico ocurre en el navegador del usuario.

## Tecnología

- HTML, CSS y JavaScript puro (sin frameworks ni proceso de build).
- [math.js](https://mathjs.org/) para el parseo y la derivación simbólica.
- [KaTeX](https://katex.org/) para renderizar las expresiones matemáticas.

Ambas librerías se cargan desde CDN (cdnjs), así que no hace falta instalar nada para correr el proyecto.

## Cómo correrlo en local

Solo abre `index.html` en cualquier navegador. También puedes usar la extensión **Live Server** de VS Code (clic derecho sobre `index.html` → "Open with Live Server") si prefieres tener recarga automática mientras editas.

## Cómo publicarlo con un link (GitHub Pages)

1. Sube esta carpeta a un repositorio de GitHub:
   ```bash
   git init
   git add .
   git commit -m "primera versión de la calculadora"
   git branch -M main
   git remote add origin https://github.com/tu-usuario/tu-repo.git
   git push -u origin main
   ```
2. En GitHub, entra a **Settings → Pages**.
3. En "Branch" selecciona `main` y la carpeta `/root`, luego guarda.
4. En 1-2 minutos tu página estará disponible en:
   `https://tu-usuario.github.io/tu-repo/`

Ese es el link que puedes compartir con cualquiera.

## Estructura del proyecto

```
calculadora-derivadas/
├── index.html      # toda la app: estructura, estilos y lógica
└── README.md
```

## Próximos pasos posibles

- Graficar la función y su derivada.
- Mostrar el procedimiento paso a paso, no solo el resultado final.
- Exportar el historial.
