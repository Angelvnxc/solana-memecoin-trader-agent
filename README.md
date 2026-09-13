# 🚀 Solana Memecoin Trader Agent

Un agente inteligente y evolutivo de trading de memecoins en Solana que **aprende, adapta y evoluciona** con el tiempo. El agente "nace" con conocimiento base y mejora continuamente mediante análisis de narrativas, patrones de mercado y feedback de trades.

## 🎯 Características Principales

- **🧠 Aprendizaje Evolutivo**: El agente mejora con cada trade y narrativa observada
- **📊 Análisis de Narrativas**: Monitorea Twitter, Discord, Telegram para detectar tendencias
- **🎭 Sentiment Analysis**: Comprende el sentimiento del mercado en tiempo real
- **🤖 Trading Autónomo**: Ejecuta trades con gestión de riesgo inteligente
- **💾 Memoria Persistente**: Almacena patrones, lecciones y estrategias aprendidas
- **⚠️ Detección de Rugs**: Identifica proyectos fraudulentos antes de invertir
- **📈 Backtesting**: Prueba estrategias en datos históricos

## 🏗️ Arquitectura

```
solana-memecoin-trader-agent/
├── agent/
│   ├── __init__.py
│   ├── core.py                 # Núcleo del agente
│   ├── memory.py               # Sistema de memoria y aprendizaje
│   └── strategies.py           # Estrategias de trading
├── narratives/
│   ├── __init__.py
│   ├── collector.py            # Colecta narrativas de redes sociales
│   ├── sentiment.py            # Análisis de sentimiento
│   └── analyzer.py             # Procesamiento de narrativas
├── blockchain/
│   ├── __init__.py
│   ├── solana_client.py        # Conexión a Solana
│   ├── token_analyzer.py       # Análisis de tokens
│   └── executor.py             # Ejecutor de trades
├── models/
│   ├── __init__.py
│   ├── ml_predictor.py         # Modelos de ML para predicción
│   └── pattern_detector.py     # Detección de patrones
├── config/
│   ├── settings.py             # Configuración
│   └── constants.py            # Constantes
├── database/
│   ├── __init__.py
│   └── storage.py              # Almacenamiento persistente (SQLite/PostgreSQL)
├── utils/
│   ├── __init__.py
│   ├── logger.py               # Logging
│   └── helpers.py              # Funciones auxiliares
├── main.py                     # Punto de entrada
├── requirements.txt            # Dependencias
├── .env.example                # Variables de entorno
└── README.md
```

## 🚀 Inicio Rápido

### Requisitos
- Python 3.9+
- Solana RPC endpoint (Helius, QuickNode, etc.)
- API keys opcionales (para redes sociales)

### Instalación

```bash
git clone https://github.com/Angelvnxc/solana-memecoin-trader-agent
cd solana-memecoin-trader-agent
pip install -r requirements.txt
cp .env.example .env
# Edita .env con tus configuraciones
```

### Uso Básico

```python
from agent.core import MemecoinTraderAgent

# Crear agente
agent = MemecoinTraderAgent(config_path="config/settings.py")

# Iniciar el loop de trading
agent.start()
```

## 🧬 Cómo Funciona el Aprendizaje

1. **Fase 1: Nacimiento** 🐣
   - El agente inicia con conocimiento base sobre patrones comunes
   - Tiene reglas de riesgo básicas

2. **Fase 2: Observación** 👀
   - Monitorea narrativas en redes sociales
   - Analiza sentimiento y tendencias
   - Observa movimientos de precios

3. **Fase 3: Experimentación** 🔬
   - Ejecuta pequeños trades para aprender
   - Detecta qué narrativas correlacionan con ganancias
   - Refina su estrategia

4. **Fase 4: Evolución** 📈
   - Mejora modelos ML con nuevos datos
   - Actualiza pesos de estrategias
   - Aprende nuevos patrones de mercado

## 🎓 Narrativas que Aprende

- **Narrativa de Utilidad**: Proyectos con casos de uso reales
- **Narrativa de Comunidad**: Crecimiento orgánico de comunidad
- **Narrativa de Hype**: Movimientos virales en redes sociales
- **Narrativa de Ballenas**: Movimientos de grandes holders
- **Narrativa de Riesgo**: Patrones de rugs y honeypots

## ⚙️ Configuración

Edita `config/settings.py`:

```python
# Solana
RPC_ENDPOINT = "https://api.mainnet-beta.solana.com"

# Trading
MAX_POSITION_SIZE = 0.5  # SOL
STOP_LOSS_PERCENT = -15
TAKE_PROFIT_PERCENT = 50

# Riesgo
MAX_DAILY_LOSS = 5  # SOL
MAX_SLIPPAGE = 1  # %

# Aprendizaje
LEARNING_RATE = 0.01
MEMORY_SIZE = 10000
```

## 📊 Monitoreo

El agente genera logs y métricas:

```
logs/
├── trades.log          # Histórico de trades
├── narratives.log      # Narrativas detectadas
├── errors.log          # Errores y alertas
└── performance.log     # ROI, Sharpe ratio, etc.
```

## 🛡️ Seguridad y Riesgo

- **Gestión de Riesgo**: Stop-loss automático, position sizing
- **Detección de Rugs**: Análisis de liquidez y holder distribution
- **Rate Limiting**: Respeto de límites de API
- **Validación**: Verifica legitimidad de tokens antes de operar

## 📝 Licencia

MIT

## ⚠️ Disclaimer

Este proyecto es educativo. El trading de criptomonedas es altamente riesgoso. No garantiza ganancias y puedes perder todo tu capital. Úsalo bajo tu propio riesgo.

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor abre un issue o pull request.

---

**Creado con ❤️ para traders inteligentes en Solana**
