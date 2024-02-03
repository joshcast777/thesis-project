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
- ShadCN UI
- Netlify

## Instalación y ejecución

Antes de ejecutar el proyecto, deberá configurar las variables de entorno en el proyecto. Para esto deberá tener a la mano el API Key y la URL de Supabase, que la obtuvo al momento de crear la cuenta en la plataforma. Esto se indica en el __Anexo 5. Manual técnico__ de la tesis a la que pertenece este proyecto.

1. Cambie el nombre del archivo `.env.example` a `.env`.
2. Descomente la las líneas que comienzan con VITE_SUPABASE_API_KEY y VITE_SUPABASE_URL, es decir, borre el signo de numeral que está al inicio de cada línea.
3. Reemplace los valores después del igual por los valores proporcionados en su cuenta de Supabase.

Para instalar y ejecutar este proyecto deberá tener Node.js instalado en su computador, de preferencia, la última versión.

```bash
# Clona el repositorio
git clone https://github.com/joshcast777/thesis-project.git

# Accede al directorio del proyecto
cd thesis-project

# Instala las dependencias
pnpm i

# Ejecuta el proyecto
pnpm run dev
```

Se usó `PNPM` como gestor del proyecto. Sin embargo, puede usar NPM para gestionar el proyecto o el de su preferencia.

Si desea usar `NPM`, después de clonar y acceder a la carpeta, ejecute lo siguiente:

```bash
# Instala las dependencias
npm i

# Ejecuta el proyecto
npm run dev
```

## Uso

El anotador ingresará al sitio web y deberá ingresar su cédula, esto revisará si ya está registrado; en caso de ser positivo mostrará las preguntas, en caso de ser negativo mostrará los demás campos a ser llenados.
