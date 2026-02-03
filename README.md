# Job-Market-Analysis-
System to collect and analyze tech job market data using Python and SQL.
¿De qué trata este proyecto?
Este proyecto nace de una idea simple: quiero entender el mercado laboral tech mientras demuestro que sé trabajar con datos de verdad.
Aquí construí un sistema que extrae ofertas de empleo reales, limpia los datos, los organiza, los analiza y los muestra en un dashboard interactivo.
En pocas palabras, desde el dato crudo hasta la información útil lista para tomar decisiones.
Este proyecto no es solo para practicar, sino para mostrar cómo trabajo con datos como lo haría en un empleo real.

Qué hace este proyecto
1.Obtención de datos
  -Extrae ofertas de sitios como RemoteOK, LinkedIn, Indeed, Computrabajo y CGetOnBoard.
  -Guarda los datos en un archico CSV/JSON tal como se obtienen en data/raw/ para       siempre tener el original.

2.Limpieza y preparación de datos
  -Normaliza salarios, roles y tecnologías.
  -Elimina duplicados y errores.
  -Guarda los datos limpios en data/cleaned/, listos para análisis.

3.Almacenamiento en base de datos
  -Inserta la información en PostgreSQL o MySQL.
  -Permite hacer consultas SQL para responder preguntas clave sobre el mercado.

4.Análisis de tendencias del mercado
  -Detecta cuáles son las habilidades más buscadas.
  -Calcula salarios promedio por rol y país.
  -Identifica los países con más ofertas remotas.

5.Visualización de datos
  -Dashboard interactivo con Streamlit o Power BI.
  -Permite explorar los resultados de manera clara y rápida.

6.Automatización completa
  -Los scripts están organizados para que el flujo sea automático: desde extraer hasta analizar.
  -Código limpio y modular (extract.py, clean.py, load_db.py, analysis.py).

Estructura del proyecto
  job-market-analysis/
  │
  ├── data/
  │   ├── raw/         # Datos tal como los descargamos
  │   └── cleaned/     # Datos limpios y listos para análisis
  ├── scripts/         # Código Python: extracción, limpieza, carga, análisis
  ├── dashboard/       # Dashboards interactivos o Power BI
  ├── sql/             # Consultas y scripts de base de datos
  └── README.md        # Esta documentación

Tecnologías que uso
  -Python – extracción, limpieza, análisis y automatización
  -Pandas, Requests, BeautifulSoup, SQLAlchemy, Streamlit
  -Base de datos: PostgreSQL o MySQL
  -Visualización: Streamlit o Power BI
  -Control de versiones: Git y GitHub
Todo lo que muestro aquí es aplicable a un entorno laboral real.

Cómo usarlo
1.Clonar el repositorio:
 git clone https://github.com/AlbertoAlarcon-14/Job-Market-Analysis-.git
 cd job-market-analysis

2.Instalar dependencias:
 pip install -r requirements.txt

3.Ejecutar scripts:
 python scripts/extract.py   # descarga ofertas
 python scripts/clean.py     # limpia y normaliza
 python scripts/load_db.py   # guarda en la base de datos
 python scripts/analysis.py  # análisis y estadísticas

4.Abrir el dashboard:
 streamlit run dashboard/app.py
