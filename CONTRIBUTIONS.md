# **Contribuciones de Chowdhury Gomez, Junal**
## **Sprint 1**
### Demostracion en video
[Sprint 1 Grupo 2 Proyecto 3](https://www.youtube.com/watch?v=Z1AAJkgW170)

### Mis aportes al Sprint 1
1. **2025-06-21: Creacion de 7 Issues para Sprint 1**
    - **Descripcion**: Defini las tareas del Sprint 1 creando siete issues en un [Epic: Sprint 1](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/8) para guiar al equipo
   - **Issues**:
     - [Issue #1: [1] Configuracion del Repositorio GitHub](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/1)
     - [Issue #2: [2] Creacion de Hook para Formato de Commits](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/2)
     - [Issue #3: [3] Implementacion del Motor de Eventos](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/3)
     - [Issue #4: [4] Configuracion del Entorno Docker](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/4)
     - [Issue #5: [5] Creacion de Scripts para Procesamiento de Eventos](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/5)
     - [Issue #6: [6] Implementación de Pruebas Unitarias](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/6)
     - [Issue #7: [7] Documentacion del Sprint 1](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/7)
   - **Estado**: Cerrados

2. **2025-06-21: [1] Configuracion del Repositorio GitHub (Issue #1)**
   - **Descripcion**: Configuré el repositorio GitHub con protección de ramas para `main` y `develop`, y añadí una plantilla de issue [Issue #1](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/1)
   - **Rama**: [setup-estructura-repositorio](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/tree/setup-estructura-repositorio)
   - **Commit**: `c536757` [setup[#1]: Configurar estructura del repositorio](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/commit/c536757ac18e54e2b90376e66cd1dac8fa0a299f)
     - Cree `src/`, `tests/`, `.gitignore`, `README.md`, `requirements.txt`, `pytest.ini`, `docs`, `reports`
   - **Pull Request**: [merge[#1]: Fusionar rama setup-estructura-repositorio a develop](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/pull/9)
     - Revisado por Andres y Janio, fusionado a `develop` el 21 jun 2025
   - **Estado**: Cerrado (21 jun 2025)

3. **2025-06-21: [4] Configuracion del Entorno Docker (Issue #4)**
   - **Descripcion**: Configuré el entorno Docker, con `Dockerfile`, `docker-compose.yml`[Issue #4](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/4)
   - **Rama**: [setup-entorno-docker](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/tree/setup-entorno-docker)
   - **Commits**: 
      - `38b9241` [setup[#4]: Crear y configurar docker-compose.yml](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/commit/38b924108dbf537951889f4d1e0b78229a061dc5)
      - `9867bf4` [setup[#4]: Crear y configurar Dockerfile](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/commit/9867bf4668712f52f75b3a8e9767c09529f004b3)
     - Cree `Dockerfile`, `docker-compose.yml`
   - **Pull Request**: [merge[#4]: Fusionar rama setup-entorno-docker a develop](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/pull/11)
     - Revisado por Andres y Janio, fusionado a `develop` el 21 jun 2025
   - **Estado**: Cerrado (21 jun 2025)

4. **2025-06-21: [6] Implementación de Pruebas Unitarias (Issue #6)**
  - **Descripcion**: Implemente pruebas unitarias iniciales `test_cargar_workflows.py`, `test_listen_redis.py`, `test_manejar_eventos_archivos.py`, `test_notify.py`[Issue #6](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/6)
  - **Rama**: [test-pruebas-unitarias-sprint-1](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/tree/test-pruebas-unitarias-sprint-1)
  - **Commits**: 
    - `cb7e3a1` [test[#6]: Agregar test para probar notify():notificar por mensaje del Issue #5](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/commit/cb7e3a126b44f94c772df797f5de906e70574d0a)
    - `d32095f` [test[#6]: Agregar test para probar on_created():crea archivos del Issue #3](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/commit/d32095fb96297f4637e1ba656631cdf427ddcc1c)
    - `5c1c47f` [test[#6]: Agregar test para probar listen_redis() del Issue #3](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/commit/5c1c47f74f8e214567780b43cf0cdb709303147f)
    - `36e1bb0` [test[#6]: Agregar test para probar load_workflows() del Issue #3](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/commit/36e1bb0381f6f9a8e69b12801ac0956d88a27908)
  - Cree `test_cargar_workflows.py`, `test_listen_redis.py`, `test_manejar_eventos_archivos.py`, `test_notify.py`

  - **Pull Request**: [merge[#4]: Fusionar rama test-pruebas-unitarias-sprint-1 a develop](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/pull/15)
    - Revisado por Andres y Janio, fusionado a `develop` el 23 jun 2025
  - **Estado**: Cerrado (23 jun 2025)


## **Sprint 2**
### Demostracion en video
[Sprint 2 Grupo 2 Proyecto 3](https://www.youtube.com/watch?v=DnACQzOHIfs)

### Mis aportes al Sprint 2
1. **2025-06-24: Creacion de 5 Issues para Sprint 2**
    - **Descripcion**: Defini las tareas del Sprint 2 creando cinco issues en un [Epic: Sprint 2](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/34) para guiar al equipo
   - **Issues**:
     - [Issue #8: [8] Modificacion de la Configuracion de Flujos para Despliegues en Kubernetes](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/16)
     - [Issue #9: [9] Desarrollo del Modulo de Accion de Kubernetes](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/17)
     - [Issue #10: [10] Integracion del Modulo Kubernetes en el Motor de Eventos](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/18)
     - [Issue #11: [11] Implementacion de Dependencias Basicas entre Flujos de Trabajo](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/19)
     - [Issue #12: [12] Implementacion de Pruebas Unitarias para Kubernetes y Dependencias](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/21)
   - **Estado**: Cerrados


2. **2025-06-25: [12] Implementacion de Pruebas Unitarias para Kubernetes y Dependencias (Issue #12)**
  - **Descripcion**: Creacion y validacion de los tests: `test_cargar_workflows.py`, `test_listen_redis.py`, `test_manejar_eventos_archivos.py`, `test_notify.py`[Issue #12](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/21)
  - **Rama**: [test-pruebas-unitarias-sprint-2](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/tree/test-pruebas-unitarias-sprint-2)
  - **Commits**: 
    - `6bfcb1a` [test[#21]: Agregar tests para workflow_deps.py](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/commit/6bfcb1aa757dda5f3c551f89ababc89d7099056b)
    - `e67fde6` [fix[#21]: Corregir validacion en test_manejar_eventos_archivos.py](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/commit/e67fde63644df3291acbc22988e403f1b62c79fc)
    - `a9dc7cf` [test[#21]: Agregar tests para k8s_deploy.py](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/commit/a9dc7cf83094ca43f63d970271db1813302f4850)
  - Actualice `k8s_deploy.py`, `test_manejar_eventos_archivos.py`, `workflow_deps.py`

  - **Pull Request**: [merge[#21]: Fusionar rama test-pruebas-unitarias-sprint-2 a develop](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/pull/27)
    - Revisado por Andres y Janio, fusionado a `develop` el 25 jun 2025
  - **Estado**: Cerrado (25 jun 2025)


## **Sprint 3**
### Demostracion en video
[Sprint 3 Grupo 2 Proyecto 3](https://www.youtube.com/watch?v=dUviqheerLo)

### Mis aportes al Sprint 3
1. **2025-06-24: Creacion de 3 Issues para Sprint 3**
    - **Descripcion**: Defini las tareas del Sprint 3 creando tres issues en un [Epic: Sprint 3](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/35) para guiar al equipo
   - **Issues**:
     - [Issue #13: [13] Corregir conflicto de eventos entre flujos](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/28)

     - [Issue #14: [14] Mejorar portabilidad de Kubernetes](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/29)

     - [Issue #15: [15] Agregar pruebas unitarias para Kubernetes y dependencias](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/30)
   - **Estado**: Cerrados

2. **2025-06-28: [15] Implementación de Pruebas (Issue #15)**
  - **Descripcion**: Actualice y refactorice los tests: `test_cargar_workflows.py`, `test_listen_redis.py`, `test_manejar_eventos_archivos.py`, `test_notify.py`[Issue #15](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/issues/30)
  - **Rama**: [test-pruebas-unitarias-sprint-3](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/tree/test-pruebas-unitarias-sprint-3)
  - **Commits**: 
    - `9ed32dc` [test[#30]: Crear y Actualizar tests para los eventos](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/commit/9ed32dce69b78f15983d446d01dec38353f2782f)

    - `c4e245c` [test[#30]: Actualizar tests para el manejo de workflows](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/commit/c4e245c5896b4af3a19c6a53fa9b65bfffcbeafa)


    - `82db3e2` [test[#30]: Actualizar tests para el servicio listen de redis](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/commit/82db3e2804a6980e113423f1deaed7214c8d3680)

    - `1bc12b2` [test[#30]: Crear y Actualizar tests k8s_deploy.py](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/commit/1bc12b240b2a9b887a11e8df50a6d5884922d637)

  -  Actualice y refactorice los tests: `test_cargar_workflows.py`, `test_listen_redis.py`, `test_manejar_eventos_archivos.py`, `test_notify.py`
  - **Pull Request**: [merge[#30]: Fusionar rama test-pruebas-unitarias-sprint-3 a develop](https://github.com/JunalChowdhuryG/Grupo-2-Practica-Calificada-4/pull/33)
    - Revisado por Andres y Janio, fusionado a `develop` el 29 jun 2025
  - **Estado**: Cerrado (29 jun 2025)

