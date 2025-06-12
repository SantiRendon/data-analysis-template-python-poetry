# Data Analysis Template Python Poetry

Template base para proyectos de análisis de datos en Python, utilizando **[Poetry](https://python-poetry.org/)** como gestor de dependencias y entorno virtual.

## 🧰 Características

- Gestión de entorno y dependencias con Poetry
- Estructura modular organizada por carpetas
- Preparado para notebooks, scripts, y modelos de base de datos
- Listo para entornos colaborativos y control de versiones

## ⚙️ Requisitos

- Python 3.9 o superior
- Poetry ([ver instrucciones de instalación](https://python-poetry.org/docs/#installing-with-the-official-installer))

## 🚀 Instalación rápida

1. Clona el repositorio:

```bash
https://github.com/SantiRendon/data-analysis-template-python-poetry.git
```

2. Navega al directorio del proyecto:
```bash
cd data-analysis-template-python-poetry
```

3. Instala las dependencias del proyecto con Poetry:
```bash
poetry install
```

## 📦 Dependencias incluidas

Este template incluye paquetes esenciales para análisis de datos en Python:

* **pandas**: Manipulación y análisis de datos tabulares con estructuras como DataFrame.
* **numpy**: Computación numérica eficiente con arrays multidimensionales.
* **matplotlib**: Visualización básica de datos en gráficos estáticos.
* **seaborn**: Visualización estadística avanzada sobre matplotlib, con estilo mejorado.
* **jupyter**: Herramientas para ejecutar notebooks interactivos desde el navegador.
* **ipykernel**: Permite usar entornos de Poetry como kernel en Jupyter.
* **mysql-connector-python**: Conector oficial de MySQL para conectarse a bases de datos desde Python.

## 📦 Uso de Poetry

### Personalizar el proyecto

Edita el archivo `pyproject.toml` para ajustar los metadatos del proyecto:

- `name`: nombre del proyecto
- `version`: versión inicial
- `description`: breve descripción
- `authors`: tu nombre y correo

Ejemplo:

```toml
[tool.poetry]
name = "mi-analisis-datos"
version = "0.1.0"
description = "Análisis exploratorio del consumo de energía en Latinoamérica"
authors = [
    {name = "santiDev",email = "xantirendonc@gmail.com"}
]
```

### Agregar una nueva dependencia

```bash
poetry add nombre_paquete
```

Ejemplo:

```bash
poetry add pandas matplotlib jupyterlab
```

### Instalar todas las dependencias del proyecto (incluyendo las de desarrollo)

```bash
poetry install --with dev
```

## 🗂️ Estructura del Proyecto

```
📁 data-analysis-template-python-poetry
│
├── 📁data
│   ├── 📁external
│   ├── 📁processed
│   ├── 📁raw
│   └── 📁tables
│
├── 📁database
│   ├── 📁models
│   ├── 📁queries
│   └── 📁scripts
│
├── 📁docs
│   ├── 📁diagrams
│   ├── 📁planning
│   └── 📁research
│
├── 📁notebooks
├── 📁reports
│   └── 📁figures
├── 📁src
│   └── 📁scripts
│
├── .gitignore
├── LICENSE
├── README.md
└── pyproject.toml
```

## 📜 Licencia

Este proyecto está bajo la licencia [MIT](LICENSE).
