# Sistema Web de Tesis

__[Link del GitHub](https://github.com/joshcast777/thesis-project)__

Este es un pequeño sistema web que forma parte del proyecto de tesis para Ingeniería de Sofytware que servirá para que los anotadores puedan dar retroalimentación sobre si las definiciones, ejemplos y casos de uso le ayudan a comprender mejor el término mostrado.

## Información de la Tesis

La tesis contempla el análisis de si las definiciones, ejemplos y casos de uso generados por GPT-3 son útiles para la síntesis de textos científicos.

Los anotadores usarían este sistema web para dar su calificación a lo que generó GPT-3.

## Función del Proyecto de GitHub en la Tesis

Este sistema web se usará para recopilar la calificación que los anotadores darán a las definiciones, ejempos y casos de uso generados por GPT-3.

La calificación de los anotadores será según las siguientes preguntas:

- __Para la definición:__ *¿Considera que esta definición le ayuda a comprender el término en cuestión?*
- __Para el ejemplo:__ *¿Este ejemplo le ha ayudado a comprender mejor el término en cuestión?*
- __Para el caso de uso:__ *¿El caso de uso le ha ayudado a comprender mejor el término en cuestión?*

La calificación también se comprende en el siguiente rango:

- <span style="color:#EF4444">Totalmente de acuerdo.</span>
- <span style="color:#FB923C">De acuerdo.</span>
- <span style="color:#EAB308">Neutro.</span>
- <span style="color:#22C55E">En desacuerdo</span>
- <span style="color:#3B82F6">Totalmente en desascuerdo</span>

Estas opciones son las que el anotador deberá escoger al analizar los textos.

## Herramientas y bibliotecas utilizadas

- React (versión 18.2.0)
- Vite.js (versión 4.4.5)
- TypeScript (versión 5.0.2)
- TailwindCSS (versión 3.3.5)
- Zod (versión 3.22.4)
- Zustand (version 4.4.6)
- React Hook Form (versión 7.48.2)
- Supabase (versión 2.38.4)
- TanStack Query (versión 5.8.2)
- ShadCN UI
- Netlify

## Instalación y ejecución

Para instalar y ejecutar este proyecto deberá tener Node.js instalado en su computador, de preferencia, la última versión.

```bash
# Clona el repositorio
git clone https://github.com/joshcast777/thesis-project.git

# Accede al directorio del proyecto
cd thesis-project

# Instala las dependencias
npm i

# Ejecuta el proyecto
npx run dev
```

El proyecto tiene un archivo `pnpm-lock.yaml`, lo que indica que el proyecto se creó con PNPM y no con NPM.

El usar NPM no causará eproblemas al momento de ejecutarlo, solo descargará los node modules y creará el archivo package-lock.json

## Uso

El anotador ingresará al sitio web y deberá ingresar su cédula, esto revisará si ya está registrado; en caso de ser positivo mostrará las preguntas, en caso de ser negativo mostrará los demás campos a ser llenados.
