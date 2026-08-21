# 📈 BoardingGate — Terminal Financiera & Gestor de Cartera con IA

<p align="center">
  <img src="https://img.shields.io/badge/Financial-Terminal-0A0A0A?style=for-the-badge&logo=probot&logoColor=60A5FA" alt="Financial Terminal" />
  <img src="https://img.shields.io/badge/React%2018-SPA-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React 18" />
  <img src="https://img.shields.io/badge/AI-Multi--Model%20(Gemini%20%2B%20OpenRouter)-8B5CF6?style=for-the-badge&logo=openai&logoColor=white" alt="AI Engine" />
  <img src="https://img.shields.io/badge/Charts-ECharts%20%2B%20TradingView-F59E0B?style=for-the-badge&logo=tradingview&logoColor=white" alt="TradingView" />
  <img src="https://img.shields.io/badge/Cloud-Google%20Drive%20Sync-34A853?style=for-the-badge&logo=googledrive&logoColor=white" alt="Google Drive Sync" />
  <img src="https://img.shields.io/badge/Zero_Install-Single_File-4CAF50?style=for-the-badge" alt="Zero Dependencies" />
</p>

<p align="center">
  <b>BoardingGate</b> es una suite integral de gestión patrimonial, auditoría financiera, rastreo de mercado (<i>Stock Screener</i>) y análisis fundamental asistido por <b>Inteligencia Artificial Multimodelo en tiempo real</b>.
</p>

<p align="center">
  <a href="#-módulos-principales">Módulos</a> •
  <a href="#-motor-de-inteligencia-artificial">Motor IA</a> •
  <a href="#-nube-y-cotizaciones-en-tiempo-real">Sincronización Cloud</a> •
  <a href="#-despliegue-y-uso-local">Instalación</a> •
  <a href="#-seguridad-y-privacidad">Privacidad</a>
</p>

---

## 🏛️ Módulos Principales

La aplicación está diseñada bajo una arquitectura modular de alto rendimiento:

├── 💼 Cartera (Portfolio Manager & Valuation) ├── 💰 Dividendos (Cash Flow &
Retenciones Internacionales) ├── 📊 Resultados & Fiscalidad (IRPF España &
Compensación 4 Años) ├── 🔍 Estudio & Terminal IA (13 Informes, Screener,
Cribado, Grafos) ├── 🔧 Útiles (Interés Compuesto, Renting vs Compra, Hub de
Enlaces) └── ⚙️ Ajustes (Conexión API, Google Script, PIN, Respaldo JSON)


---

### 1. 💼 Cartera (`portfolio`)
* **Gestión de Lotes y FIFO:** Registro pormenorizado de compras, promedios ponderados, comisiones y liquidación estricta bajo normativa **FIFO** (con cálculo automático de remanentes en ventas parciales y trazabilidad de lotes consumidos).
* **Valoración Multidivisa:** Cotizaciones en tiempo real y conversión dinámica de tipos de cambio (EUR, USD, GBP, CHF, JPY, CAD, etc.).
* **Métricas Institucionales:** Rentabilidad Simple vs Anualizada (Time-Weighted), Intradía en vivo con estado de mercados (Abierto, Cerrado, Pre-Market), multiplicador **MoIC** (*Multiple on Invested Capital*) y atribución de rendimiento con y sin dividendos.
* **Auditoría de Margen de Seguridad:** Monitorización continua del *Fair Value* con alertas tempranas cuando el margen cae por debajo del 25% del umbral de entrada ($M_{\text{Current}} < \frac{1}{4} M_{\text{Original}}$).
* **Línea Temporal (Timeline):** Visualizador de eventos interactivo en formato de **Árbol de Decisión / Grafo Jerárquico** o **Calendario Anual** con inspección día a día.
* **Simulador de Objetivos (Take Profit / Stop Loss):** Cálculo de rentabilidad latente si se alcanzan precios objetivos y ratio Riesgo/Beneficio global de cartera.
* **Widgets TradingView:** Integración nativa de gráficos avanzados con velas japonesas, RSI, Medias Móviles, Mapas de Calor sectoriales (S&P 500) y Mapas de Sentimiento Mundial.

---

### 2. 💰 Dividendos (`dividends`)
* **Matriz Anual e Histórica:** Cuadro mensual de cobro (Neto, Retención en Origen, Retención en Destino y Bruto).
* **Doble Imposición Internacional:** Detección automática de dividendos con retención extranjera y cálculo del crédito fiscal (**B.D.I. y deducción del 15%** para la declaración de la renta en España).
* **Previsión de Pagos Asistida por IA:** Consulta online del calendario estimado (*Ex-Dividend Date* y *Payment Date*) para anticipar cobros en el año en curso.
* **Gráficas de Distribución:** Desglose estacional por meses, histórico anual acumulado y concentración por ticker.

---

### 3. 📊 Resultados y Fiscalidad (`results`)
* **Consolidación Anual de Plusvalías/Minusvalías:** Cuadro interactivo con bloqueo de ejercicios cerrados para auditar ganancias y pérdidas patrimoniales.
* **Seguimiento de Compensación a 4 Años:** Control del saldo negativo pendiente de compensar entre Ganancias Patrimoniales (GPP) y el límite del 25% sobre Rendimientos de Capital Mobiliario (RCM).
* **Guía de la Regla de los 2 Meses / 1 Año:** Esquema visual de la normativa anti-aplicación de pérdidas (mercados UE vs Extra-UE).
* **Borrador de la Renta con IA:** Generador automático de informes con las **casillas exactas del Modelo 100 (IRPF)**, desglosando ventas de acciones, reembolsos de fondos de inversión, retenciones de dividendos y gastos deducibles de custodia/administración.

---

### 4. 🔍 Estudio, Screener y Análisis Fundamental (`analysis`)
* **13 Informes Especializados de Wall Street:**
  1. *Análisis Integral 360º:* Modelo de negocio, ventajas competitivas (Moat) y métricas TTM.
  2. *Auditoría de Estados Financieros:* Balance sheet deep dive, calidad del flujo de caja (FCF) y *Red Flags*.
  3. *Revisión de Earnings:* Resultados trimestrales, sorpresas de BPA e ingresos, y *Guidance*.
  4. *Comparativa Peer:* Análisis cruzado con los 6 competidores directos más cercanos.
  5. *Modelos de Valoración (DCF):* Flujo de caja descontado determinista con sensibilidades WACC/CAGR.
  6. *Riesgos y Catalizadores:* Top 5 amenazas y calendario a 12 meses.
  7. *Historia e Identidad:* Estructura legal, marcas, directiva y cuota de mercado.
  8. *Equity Research Senior:* Informe institucional completo para comités de inversión.
  9. *Ranking Sectorial Top 10:* Tabla comparativa con los 10 líderes de la industria.
  10. *Manos Fuertes & Cortos:* Rastreo de superinversores en **Dataroma**, reportes 13F / reguladores locales (CNMV, FCA, BaFin) y *Short Interest*.
  11. *Test de Estrés Macroeconómico:* Resiliencia ante ciclos de tipos de interés, inflación y cisnes negros.
  12. *Advocatus Diaboli:* Tesis bajista crítica (*Bear Case*) y motivos para NO comprar.
  13. *Valor al Accionista:* Evolución histórica del BPA/EPS, recompras (*Buybacks*) y compras de directivos (*Insiders*).
* **Rastreador de Mercado en Tiempo Real (Screener):**
  * Cobertura de 12 bolsas mundiales (EE.UU., España/IBEX, XETRA, LSE, Euronext, Tokio, HKEX, etc.).
  * Filtros fundamentales combinables: PER, PEG, ROI, Div Yield, P/B, Deuda/Equity, FCF Yield y Crecimiento EPS YoY.
  * Filtros de acción del precio: Acciones en Máximos Históricos (ATH) o Desplomes desde máximos (% de caída en $X$ meses).
* **Batalla de Activos (Cribado):** Enfrentamiento comparativo de 2 a 3 empresas con puntuación cuantitativa (0-100) y veredicto de compra.
* **Grafo de Interdependencias:** Renderizado con físicas de partículas de la cadena de valor (Proveedores y Clientes de Nivel 1 y Nivel 2).

---

### 5. 🔧 Útiles Financieros (`utils`)
* **Calculadora de Interés Compuesto:** Simulación con ajuste por inflación (poder adquisitivo real), detección del punto de inflexión (intereses > capital aportado) y notificación de hitos multiplicadores (*n-Baggers*).
* **Renting vs Compra:** Análisis comparativo de Coste Total de Propiedad (TCO) proyectado a $N$ años, considerando depreciación, averías, seguros, energía/combustible y cálculo del precio de venta de equilibrio.
* **Hub de Enlaces Financieros:** Acceso directo y descubrimiento automático de herramientas como TradingView, Dataroma, Gurufocus, Macrotrends, TIKR, Finviz o Simply Wall St.

---

## 🧠 Motor de Inteligencia Artificial

La terminal cuenta con un enrutador inteligente compatible con:

* **Google Gemini (Direct API):** Conexión directa mediante clave gratuita o de facturación cloud para habilitar **Google Search en tiempo real**.
* **OpenRouter API:** Acceso unificado a modelos avanzados como **Claude 3.5 Sonnet, ChatGPT-4o, DeepSeek R1/V3, Kimi K2.5 o Llama 3**, con importación dinámica de nuevos modelos y ordenación por coste de tokens y ventana de contexto ($k$).
* **Modo Sin API (Bypass):** Generación automática de prompts enriquecidos para copiar y pegar directamente en cualquier interfaz externa (ChatGPT, Claude, etc.).

---

## ☁️ Nube y Cotizaciones en Tiempo Real

El sistema utiliza **Google Apps Script** como puente backend serverless (código incluido en los ajustes de la app):

1. **Cotizaciones y Tipos de Cambio:** Consulta periódica automática a Yahoo Finance y TradingView Scanner sin coste.
2. **Sincronización Silenciosa con Google Drive:** Guarda y recupera la base de datos `BOARDINGGATE_DB.json` en tu unidad de Google Drive.
3. **Control de Versiones y Backup (.bak):** Generación automática de copias de seguridad previas ante cualquier sobrescritura, con restauración en un clic.

---

## 🚀 Despliegue y Uso Local

**Zero-Build:** La aplicación no requiere `Node.js`, `npm`, Webpack ni compilación previa.

### 1. Ejecución Local
```bash
# Clona el repositorio
git clone https://github.com/tu-usuario/boardinggate-bolsa.git
cd boardinggate-bolsa

# Abre el archivo en tu navegador
# (Doble clic en BOLSA.HTML o usando Live Server en VS Code)

2. Despliegue en GitHub Pages

1.  Sube BOLSA.HTML a tu repositorio.
2.  Ve a Settings > Pages y activa el despliegue desde la rama main.
3.  ¡Listo! Ya puedes acceder a tu terminal desde cualquier dispositivo
    (ordenador, tablet o móvil).

🔒 Seguridad y Privacidad

  - 100% Client-Side: Tus datos financieros no pasan por ningún servidor
    intermediario; se procesan en tu propio navegador.
  - Protección con PIN: Posibilidad de activar un PIN de acceso de 4 dígitos
    para bloquear la interfaz al recargar.
  - Cifrado Ligero: Las claves de API y URLs sensibles se almacenan ofuscadas en
    el localStorage.
  - Exportación / Importación Masiva: Exporta en cualquier momento tu cartera
    completa en formato JSON o importa extractos masivos mediante PDF / CSV
    asistido por IA.

⚖️ Aviso Legal (Disclaimer)

Esta plataforma tiene fines exclusivamente informativos, analíticos y de gestión
personal. La información y análisis generados por los modelos de Inteligencia
Artificial o las cotizaciones de mercado no constituyen asesoramiento
financiero, legal o tributario. Verifica siempre la información con fuentes
oficiales y asesores cualificados antes de tomar decisiones de inversión.
