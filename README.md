# Starter: Arquitectura de 3 capas

Capa 1 - Nivel de usuario/presentación
Capa 2 - Nivel de aplicación
Capa 3 - Nivel de datos
Este _starter_ es un repositorio modular (_modulith_) con una arquitectura de tres capas con un front Vue Typescript Vite a nivel de usuario, un back en Python a nivel de aplicación y una base de datos MySQL a nivel de datos. Es un punto de partida para realizar pruebas de concepto. Contiene tests y herramientas que automatizan su creación y despliege, así como su calidad y seguridad.

**Requiere tener instalado Docker para el despliegue**. Podría migrarse a Kubernetes.

## Instrucciones

**1. Arrancar el proyecto**

```bash
docker-compose build
docker-compose up -d

```

| capa       | puerto |
| ---------- | ------ |
| usuario    | 4002   |
| aplicación | 8000   |
| datos      | 3308   |

En la capa de aplicación está disponible SwaggerUI para visualizar y probar todos los endpoints (http://localhost:8000/docs)

**2. Parar el proyecto**
La base de datos tiene persistencia, así que al parar el contenedor no se pierden los datos.

```bash
docker-compose down
```

**Autor**: Carlos Marchena
**Licencia**: [Creative Commons BY 4.0 Atribución 4.0 Internacional](https://creativecommons.org/licenses/by/4.0/deed.en)  
[Detalle licencia](https://creativecommons.org/licenses/by/4.0/legalcode.es)
