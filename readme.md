# Entrega Final de Proyecto Talento Tech 
## Framework de Automatización de Pruebas

---

### Alumno/a:
Esteban Luna

### Curso:
QA Automation

### Proyecto:
Framework de Automatización de Pruebas – UI y API

### Repositorio:
https://github.com/H2KMedia/FINAL_QA_E_LUNA

---

## 1. Introducción

El presente proyecto corresponde a la **Entrega Final del curso**, cuyo objetivo es desarrollar un **framework de automatización de pruebas completo**, aplicando los conocimientos adquiridos a lo largo de la cursada.

El framework fue desarrollado en **Python**, utilizando **Selenium WebDriver** para pruebas de interfaz de usuario (UI) y **Requests** para pruebas de API, integrados mediante el framework de testing **Pytest** y siguiendo el patrón de diseño **Page Object Model (POM)**.

---

## 2. Objetivo del Proyecto

El objetivo principal es:

- Automatizar pruebas de UI y API
- Aplicar buenas prácticas de programación
- Utilizar Page Object Model
- Implementar pruebas data-driven
- Generar reportes HTML claros y detallados
- Facilitar la escalabilidad del framework

---

## 3. Tecnologías Utilizadas

- **Python 3**
- **Pytest**
- **Selenium WebDriver**
- **Requests**
- **Page Object Model (POM)**
- **pytest-html**
- **Logging (logging module)**
- **Git y GitHub**
- **GitHub Actions (CI/CD)**

---

## 4. Estructura del Proyecto

```
FINAL_QA_E_LUNA/
│
├── pages/
├── tests/
├── utils/
├── data/
├── reports/
├── screenshots/
├── conftest.py
├── pytest.ini
├── requirements.txt
└── README.md
```

---

## 5. Pruebas de UI

Se implementaron casos de prueba que cubren flujos completos:
login exitoso, login inválido, navegación, carrito y checkout.

---

## 6. Pruebas de API

Se implementaron pruebas GET, POST y DELETE utilizando una API pública.

---

## 7. Reportes

Se generan reportes HTML automáticos en la carpeta `/reports`.
Se realizan capturas de pantalla por cada test que haya fallado y se encuentran en la siguiente ubicacion: ```reports/screens/```

---

## 8. Logging

Se implementó logging para facilitar la depuración.
Tambien se genera un log con informacion detallada de toda la ejecución de las pruebas en la siguiente ubicacion: ```logs/suite.log```

---

## 9. Instalación

```bash
pip install -r requirements.txt
```

---

## 10. Ejecución

```bash
python -m run_test.py
```

---

## ¿Como interpretar los reportes?
- Al ejecutar `run_test.py`, se genera un archivo HTML en la carpeta raiz.
- El reporte incluye:
    - Lista completa de test ejecutados
    - El estado de cada prueba
    - La duracion de cada test
    - Las capturas de pantalla para pruebas fallidas

## Pruebas incluidas
- Login exitoso y fallido
- Login exitoso y fallido usando faker
- Comportamiento de la pagina de inventario
- Comportamiento de la pagina del carrito
- API (Reqres): GET users, POST create user, DELETE user, validaciones de codigos HTTP, validaciones de estructura JSON

## Manejo de datos de prueba
- En la carpeta `datos` se incluyen archivos como:
    - `data_login.csv` -> datos de usuarios validos o invalidos
    - `productos.json` -> datos de productos para validacion


## 11. CI/CD

Integración con GitHub Actions.

## 12. Conclusión

El proyecto cumple con todos los requisitos de la consigna.

Este proyecto ofrece una estructura organizada y escalable para automatizar pruebas de API utilizando Python y Pytest. Incluye un flujo simple de ejeucion mediante `run_test.py`, generacion automatica de reporte HTML facilitando el analisis de las pruebas.

La arquitectura del proyecto esta pensada para agregar nuevos casos de prueba y configuraciones sin modificar el nucleo del proyecto, manteniendo buenas practicas y permitiendo su escalabilidad en el tiempo.
