# PROYECTO-API-REST- Santiago C.

# Mi API REST de Usuarios
## Instalación
```
git clone <url-del-repo>
cd mi-api
npm install
```
## Ejecución
```
node index.js
```
## Autenticación
Todas las peticiones requieren el header:
```
x-api-key: mi-clave-secreta-2024
```
## Endpoints
| Método | Ruta | Descripción |
|---------|-------------------|---------------------------|
| GET | /usuarios | Listar todos |
| GET | /usuarios/:id | Obtener uno por ID |
| POST | /usuarios | Crear usuario |
| PUT | /usuarios/:id | Actualizar usuario |
| DELETE | /usuarios/:id | Eliminar usuario |
| GET | /usuarios?rol=X | Filtrar por rol |


------ análisis de readFileSync vs readFile ----------
La diferencia principal entre readFileSync y readFile es la forma en que leen los archivos. readFileSync es síncrono, es decir, que el programa se detiene hasta que termina de leer el archivo. Esto lo hace más fácil de entender, pero puede volver la aplicación más lenta si el archivo es grande. Por otro lado, readFile es asíncrono, lo que permite que el programa continúe ejecutándose mientras se lee el archivo. Esto es mejor para aplicaciones más grandes o servidores, ya que mejora el rendimiento. En conclusión, readFileSync es útil para pruebas o scripts simples, mientras que readFile es más recomendable en aplicaciones reales porque es más eficiente.
