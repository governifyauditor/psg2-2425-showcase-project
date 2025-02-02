
# Auditar proyectos de PSG2-2425 con Bluejay.

## 1. Crear y configurar el repositorio.

**1.1. Crear un repositorio en GitHub usando la actividad de GitHub Classroom correspondiente.**

- Actividad disponible en https://classroom.github.com/a/69SYzwAj
- Selecciona tu UVUS.
- Selecciona tu grupo `GX-XY` o créalo si aún no existe.
- Acepta el assignment para poder acceder al repositorio de GitHub.

**1.2. En la rama main modificar el archivo `info.yml`.**

info.yml:
```yaml
project:
  name: 'PSG2-2425-GX-XY'
  owner: 'LX'
  teamId: 'XY'
  identities: {}
  notifications:
    email: 'josemgarcia@us.es,japarejo@us.es,aruiz@us.es,cmuller@us.es,macuna@us.es,amarquez6@us.es'
  members:
    member1:
      name: 'José María'
      surname: 'García' 
      githubUsername: 'josemgarcia'
    member2:
      name: 'Jose Antonio'
      surname: 'Parejo'
      githubUsername: 'japarejo'
    member3:
      name: 'Antonio'
      surname: 'Ruiz'
      githubUsername: 'antonioruizcortes'
    member4:
      name: 'Carlos'
      surname: 'Müller'
      githubUsername: 'cmullercejas'
    member5:
      name: 'Lola'
      surname: 'De Acuña'
      githubUsername: 'loladacuna'
    member6:
      name: 'Alfonso'
      surname: 'Márquez'
      githubUsername: 'alfedu'
```

- Rellenar las X,Y.
    > Por ejemplo, el grupo 54 del Laboratorio 5:
    >```yaml
    >name: 'PSG2-2425-G5-54'
    >owner: 'L5'
    >teamId: '54'
    >```

- Sustituir los datos de cada memberN por los del miembro real.
- Si el número de miembros es menor de los que hay en la plantilla, eliminar los últimos que sobren (por ejemplo, si son 5 miembros, eliminar el bloque completo de `member6`)
- Modificar la cadena de `notifications.email` para que contengan sólo los correos de todos los miembros separados por comas y sin espacios.

## 2. Crear el workspace en ZenHub
- Crea un nuevo workspace sobre el repositorio de GitHub abriendo la extensión de ZenHub y seleccionando la organización `gii-is-psg2`.
- Usa el nombre PSG2-2425-GX-XY para el nuevo workspace, sustituyendo las X e Y igual que en pasos anteriores (por ejemplo: `PSG2-2425-G5-54`).
- Configura el workspace como `private` y asigna el repositorio GitHub al workspace creado (asegúrate de seleccionar la organización `gii-is-psg2`).
- Añade todos los miembros del grupo al workspace (antes deben haber accedido a la actividad de GitHub Classroom).
- Modificar los pipelines para que sigan la siguiente estructura **OBLIGATORIAMENTE:**
  - Elimina las pipelines denominadas `Icebox` y `Product Backlog`.
  - Renombra la pipeline `Sprint Backlog` a `Todo` (case sensitive).
  - Renombra la pipeline `Review/QA` a `In Review` (case sensitive).
- Como resultado tendremos un tablero donde las columnas principales que utilizaremos serán: `Todo, In Progress, In Review, Done` (case sensitive).

## 3. Unir el proyecto a la asignatura auditada por Bluejay

- Accede a [join.bluejay.governify.io](https://join.bluejay.governify.io).
- Añade la **URL del repositorio** de GitHub.
- Click en **CHECK**. Si ha dado error revisa la [sintaxis](https://www.yamllint.com/) del info.yml.
- **Selecciona la clase** a la que te quieres unir (PSG2-2425) y especifica el código que te dará tu profesor.
- Click en **JOIN**.
- En caso de que haya algún otro problema al configurar Bluejay, el equipo de soporte está disponible en [un canal de Gitter dedicado](https://app.gitter.im/#/room/!VTAnLfNgxrEdydQgWd:gitter.im).


