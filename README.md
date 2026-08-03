# Portafolio $10k en 3 Años 📈

Este repositorio contiene los scripts en Python para realizar un *backtest* cuantitativo que simula la acumulación de capital mediante aportes recurrentes, utilizando el rendimiento histórico real de diversos ETFs (como SMH, SPYG, VTI, entre otros). 

El objetivo principal de este código es demostrar, con datos empíricos del mercado, el efecto del interés compuesto y la constancia en la inversión frente a la simple acumulación de efectivo.

## 🚀 Características

* **Extracción de Datos Reales:** Se conecta a la API de Yahoo Finance mediante `yfinance` para descargar la serie de precios de cierre ajustados de cualquier ticker válido.
* **Cálculo de Retornos:** Calcula los retornos mensuales reales y el crecimiento del portafolio asumiendo un aporte mensual fijo (ej. $200/mes).
* **Visualización Dinámica y Estática:** Genera gráficos exportables en formato `.png` y animaciones en formato `.gif` (ideales para redes sociales o eToro) donde se compara la línea base de los aportes frente al valor real del portafolio capitalizado.

## 🛠️ Requisitos e Instalación

Para ejecutar este proyecto de forma local, necesitas tener Python instalado y las siguientes librerías de análisis y visualización.

Puedes instalar las dependencias ejecutando:

```bash
pip install yfinance pandas matplotlib pillow

## 💻 Uso

El script principal está configurado por defecto para simular aportes de $200 mensuales durante 36 meses (3 años) utilizando el ETF SMH (VanEck Semiconductor ETF).
Para ejecutarlo y generar la gráfica estática en tu directorio local:

# Parámetros editables en el script:
pago_mensual = 200
meses_simulacion = 36
ticker = "SPYG"  # Modificable por cualquier otro ETF como "SMH", "VTI", "IEMG", etc.

Simplemente corre el script en tu entorno (Jupyter, VS Code, terminal) y el código descargará los datos automáticamente, procesará la simulación y exportará la gráfica correspondiente.

## 👨‍💻 Acerca del Autor

Soy economista y data scientist. Mi enfoque se centra en la estructuración de portafolios cuantitativos indexados buscando el crecimiento compuesto a largo plazo. Utilizo herramientas programáticas (Python, R, Power BI) para automatizar diagnósticos de datos y simulaciones financieras.

Actualmente gestiono mi portafolio público como Popular Investor (nivel Champion) en eToro, donde aplico esta misma filosofía de transparencia y educación financiera basada en datos duros.

📊 eToro: [https://etoro.tw/4lkmjxn]
🎥 YouTube: [https://youtube.com/@andalejo1109?si=mFUajKT2k3K0L-Os]

# ⚠️ Disclaimer
Este repositorio tiene fines estrictamente educativos y de demostración analítica. Los rendimientos pasados de un instrumento financiero (como los ETFs utilizados en la simulación) no son garantía de rendimientos futuros. Este código no constituye una recomendación de inversión.
