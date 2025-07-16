# 💻 Auditoría de Software no Licenciado

Script en Python que escanea equipos con Windows para detectar software no autorizado o no licenciado, generando un reporte automatizado en Excel con un marcado visual (verde para programas autorizados, rojo para no autorizados).  
Ideal para auditorías en entornos educativos o empresariales.

🔐 **Seguridad**, 💻 **Licencias**, 🏁 **Automatización**

---

## 📌 Descripción del Proyecto

La herramienta fue desarrollada con el objetivo de **identificar software no oficial** instalado en equipos portables de una empresa de almacenes de alimentos, permitiendo a los departamentos de TI **tomar decisiones rápidas** sobre desinstalación o regularización de licencias.

Incluye:
- Escaneo automatizado mediante comandos nativos de Windows y (`wmic`) en su version para ejecutar en powershell (w10-w11).
- Comparación con una lista blanca de programas autorizados, proporcionada por la empresa, aquí no se pública la oficial.
- Generación de un informe en Excel para fácil visualización.

---

## 🧪 Tecnologías Usadas

- **Python 3.x**  
- Librerías:
  - `subprocess` → ejecución de comandos Windows.
  - `openpyxl` → generación del reporte en Excel con colores.
- **Sistema Operativo**: Windows (requiere `wmic` habilitado).

---

## 📂 Estructura del Repositorio
├── auditoria_sf_v1.py # Script principal (de dos reportes)
├── auditoria_software_powershell.py # Ejecutar si; wmic no reconocido, Permisos denegados, No genera datos
├── lista_software_permitido.txt # Lista blanca de software autorizado alterada, no la proporcionada por PYME.
├── reporte_auditoria.xlsx # Reporte generado automáticamente una vez ejecutado el script.
└── README.md
