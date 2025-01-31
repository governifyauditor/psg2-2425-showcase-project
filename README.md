
# Auditar proyectos de PSG2-2425 con Bluejay.

## 1. Crear y configurar el repositorio.

**1.1. Crear un repositorio en GitHub usando la actividad de GitHub Classroom correspondiente.**

**1.2. En la rama main modificar el archivo `info.yml`.**

info.yml:
```yaml
project:
  name: 'PSG2-2425-LX-XY'
  owner: 'LX'
  teamId: 'XY'
  identities: {}
  notifications:
    email: 'member1@alum.us.es,member2@alum.us.es'
  members:
    member1:
      name: 'Manuel'
      surname: 'Otero' 
      githubUsername: 'motero2k'
    member2:
      name: 'Javi'
      surname: 'Fernandez' 
      githubUsername: 'JaviFdez7'
    member3:
      name: 'XXXXXXXXXXX'
      surname: 'XXXXXXXXXXX' 
      githubUsername: 'XXXXXXXXXXX'
    member4:
      name: 'XXXXXXXXXXX'
      surname: 'XXXXXXXXXXX' 
      githubUsername: 'XXXXXXXXXXX'
```

- Rellenar las X,Y.
    > Por ejemplo, el grupo 54 del Laboratorio 2:
    >```yaml
    >name: 'PSG2-2425-L2-54'
    >owner: 'L2'
    >teamId: '54'
    >```

- Sustituir los datos de cada memberN por los del miembro real.
- Si el número de miembros es menor de los que hay en la plantilla, eliminar los últimos que sobren (por ejemplo, si son 5 miembros, eliminar el bloque completo de `member6`)
- Modificar la cadena de `notifications.email` para que contengan sólo los correos de todos los miembros separados por comas y sin espacios.

## 2. Crear el workspace en ZenHub
- Crear el workspace sobre el repositorio de GitHub abriendo la extensión de ZenHub
- Asignar el repositorio al workspace creado.
- Añadir todos los miembros del grupo al workspace.
- Modificar los nombres de los pipelines para que sean **OBLIGATORIAMENTE:** `Todo, In Progress, In Review, Done` (case sensitive).

## 3. Unir el proyecto a la asignatura auditada por bluejay

- Accede a [join.bluejay.governify.io](https://join.bluejay.governify.io).
- Añade la **URL del repositorio** de GitHub.
- Click en **CHECK**. Si ha dado error revisa la [sintaxis](https://www.yamllint.com/) del info.yml.
- **Selecciona la clase** a la que te quieres unir (PSG2-2425) y especifica el código que te dará tu profesor.
- Click en **JOIN**.


