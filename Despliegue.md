
# Despliegue Pokedex Angular en Azure App Service

## 1. Crear la aplicación web
1. Crear una nueva aplicación web en Azure.
2. Configurar los siguientes datos:
   - Grupo de recursos: gr-pokemon-prod
   - Nombre de la instancia: web-pokemon-app-jma
   - Pila del entorno: .NET 10 LTS
   - Región: East US
3. Hacer clic en Revisar y crear.
4. Luego hacer clic en Crear.
5. Esperar a que la aplicación termine de desplegarse.

## 2. Acceder a herramientas avanzadas
1. Cuando la aplicación web-pokemon-app-jma esté lista.
2. Ir a Herramientas de desarrollo.
3. Entrar en Herramientas avanzadas.

## 3. Preparar el proyecto Angular
1. Ir a la cuenta de GitHub.
2. Descargar el proyecto Angular.
3. Descomprimir el proyecto.
4. Abrir CMD en la carpeta del proyecto.
5. Ejecutar:
   npm install
6. Luego ejecutar:
   npm run build
7. Esto generará la carpeta:
   dist/

## 4. Subir archivos a Azure usando Kudu
1. Volver a Azure.
2. Ir a Herramientas avanzadas.
3. Se abrirá Kudu.
4. En Kudu seleccionar:
   - Debug console
   - CMD

## 5. Navegar a la carpeta de despliegue
1. Dentro de la consola CMD de Kudu ir a:
   site
2. Luego entrar a:
   wwwroot
3. Ruta final:
   site/wwwroot

## 6. Copiar archivos del build
1. Dentro de la carpeta dist.
2. Entrar a la carpeta:
   pokedex-angular
3. Copiar todo el contenido.
4. Pegar el contenido en:
   site/wwwroot

## 7. Verificación
1. Abrir la URL de la aplicación web. https://web-pokemon-app-jma.azurewebsites.net/
2. Verificar que el proyecto pokedex-angular esté correctamente desplegado.
