# **Proyecto 3: Orquestador de flujos de trabajo basado en eventos (Local)**

## **Informacion Personal**
* **Alumno:** `Chowdhury Gomez, Junal Johir` `20200092K`  
* **Grupo:** `2`
* **Correo:** `junal.chowdhury.g@uni.pe` 
* **Repositorio Grupal:** [Grupo 2: Repositorio Grupal](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4)  
* **Repositorio Individual**: [https://github.com/JunalChowdhuryG/PC4-Chowdhury-Proyecto-3-Grupo-2](https://github.com/JunalChowdhuryG/PC4-Chowdhury-Proyecto-3-Grupo-2)

## **Videos**
*  Sprint 1
   - [Link del video del Sprint 1](https://www.youtube.com/watch?v=Z1AAJkgW170)

* Sprint 2
   - [Link del video del Sprint 2](https://www.youtube.com/watch?v=DnACQzOHIfs)

* Sprint 3
   - [Link del video del Sprint 3](https://www.youtube.com/watch?v=dUviqheerLo)


## **Descripcion:**
Este repositorio documenta mis contribuciones al **Proyecto 3: Orquestador de flujos de trabajo basado en eventos (Local)** de la **Practica Calificada 4** del **Grupo 2** (Chowdhury, Zapata, La Torre) para la asignatura **Desarrollo de Software CC3S2** en el periodo academico **25-1** (2025). Este documento describe mis contribuciones a las pruebas del Proyecto 3, un orquestador de flujos de trabajo basado en eventos diseñado para monitorear eventos por ejemplo, creación de archivos, mensajes en colas y activar acciones predefinidas (como scripts Bash, scripts Python o despliegues en Kubernetes). Mi enfoque se centró en desarrollar y mantener un conjunto robusto de pruebas a lo largo de los tres sprints para garantizar la funcionalidad, confiabilidad del sistema. A continuación, detallo mis contribuciones a las pruebas en cada sprint.

## **Mi Rol**
Fui lider de desarrollo, coordinador de sprints y tester, responsable de:
- **Sprint 1**: Configurar la estructura del repositorio ([Issue #1](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/1)) y desarrollar los tests([Issue #4](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/4)).
   - Los tests desarrollados fueron:
      - `test_cargar_workflows.py`: Validaba la carga de workflows
      - `test_listen_redis.py`: Verifica la funcionalidad de redis al escuchar
      - `test_manejar_eventos_archivos.py`: Veirfica la funcionalidad de `event_engine.py` para el manejo de eventos 
      - `test_notify.py`: Verifica la funcionalidad de notificar mensajes a travez de canal redis

- **Sprint 2**: Agregue el test `test_workflows.py` y refactorice los tests del sprint 1 ([Issue #12](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/21)).
   - Se creo el test `test_workflows.py` para validar la naturaleza de los workflows
   - Se refactorizo los tests del sprint 1

- **Sprint 3**: Finalice la suite de Tests ([Issue #15](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/30))
   - Se valido la cobertura de >85%

## **Demostración de mis Contribuciones**

A continuación, se detallan los pasos para reproducir las pruebas de cada sprint, verificar la cobertura de código y limpiar el entorno. Estos pasos permiten validar las pruebas que desarrollé para garantizar la calidad del proyecto.

### Sprint 1: Pruebas Unitarias e Integración
1. **Clonar el repositorio**:
   ```bash
   git clone https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4
   ```
2. **Entrar a la carpeta del proyecto**:
   ```bash
   cd Grupo-2-Practica-Calificada-4
   ```
3. **Cambiar a la rama de pruebas del Sprint 1**:
   ```bash
   git checkout test-pruebas-unitarias-sprint-1
   ```
4. **Levantar los servicios con Docker Compose**:
   ```bash
   docker-compose up -d --build
   ```
5. **Ejecutar las pruebas**:
   ```bash
   docker-compose run event-engine pytest tests/ --cov=src --cov-report=term-missing
   ```
   - Verifica que la salida muestre una cobertura del **98%** con **9 pruebas** ejecutadas correctamente.
6. **Limpiar el entorno**:
   - Detener el contenedor:
   ```bash
   docker-compose down
   ```
   - Restaurar logs
   ```bash
   git restore reports/
   ```
   - Eliminar archivos y directorios no rastreados por Git 
   ```bash
   git clean -fd
   ```
   - Esto detiene y elimina los contenedores de Docker y limpia los archivos generados no rastreados por Git.

### Sprint 2: Pruebas de Kubernetes y Dependencias
1. **Cambiar a la rama de pruebas del Sprint 2**:
   ```bash
   git checkout test-pruebas-unitarias-sprint-2
   ```
2. **Levantar los servicios con Docker Compose**:
   ```bash
   docker-compose up -d --build
   ```
3. **Ejecutar las pruebas**:
   ```bash
   docker-compose run event-engine pytest tests/ --cov=src --cov-report=term-missing
   ```
   - Verifica que la salida muestre una cobertura de al menos **85%**, incluyendo pruebas para `src/k8s_deploy.py` y `src/workflow_deps.py`.
4. **Limpiar el entorno**:
   - Detener el contenedor:
   ```bash
   docker-compose down
   ```
   - Restaurar logs
   ```bash
   git restore reports/
   ```
   - Eliminar archivos y directorios no rastreados por Git 
   ```bash
   git clean -fd
   ```

### Sprint 3: Terminar la Suite de test
1. **Cambiar a la rama de pruebas del Sprint 3**:
   ```bash
   git checkout test-pruebas-unitarias-sprint-3
   ```
2. **Levantar los servicios con Docker Compose**:
   ```bash
   docker-compose up -d --build
   ```
3. **Ejecutar las pruebas**:
   ```bash
   docker-compose run event-engine pytest tests/ --cov=src --cov-report=term-missing
   ```
   - Verifica que la salida muestre una cobertura de al menos **90%**
4. **Limpiar el entorno**:
   - Detener el contenedor:
   ```bash
   docker-compose down
   ```
   - Restaurar logs
   ```bash
   git restore reports/
   ```
   - Eliminar archivos y directorios no rastreados por Git 
   ```bash
   git clean -fd
   ```

- **Planificacion**: Crear issues para los sprints:
  - [Epic: Sprint 1](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/8)
  - [Epic: Sprint 2](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/34)
  - [Epic: Sprint 3](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/35)


## Contribuciones
Para detalles de mis contribuciones, incluyendo commits, pull requests, y videos, consulta [CONTRIBUTIONS.md](CONTRIBUTIONS.md)
