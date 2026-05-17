# Dashboard-Porsche-IA
# 🏎️ Dashboard da Porsche com Agentes de IA

Este repositório contém a estruturação, planejamento e a lógica prática utilizada para criar um painel inteligente de análise de dados focado na marca Porsche, utilizando IA como copiloto.

## 🤖 Arquitetura Prática no Termux

Para testar o projeto na prática, desenvolvemos um script em Python que funciona como o **Agente Analista de Dados**. Ele consome um arquivo estruturado em JSON contendo as principais **features** (funcionalidades e métricas) de modelos icônicos da Porsche.

### 📋 Banco de Dados do Projeto (porsche_data.json)
```json
[
  {
    "modelo": "Porsche 911 Carrera",
    "ano": 2024,
    "motor": "3.0L Boxer Twin-Turbo",
    "velocidade_maxima": "293 km/h",
    "tipo": "Combustão"
  },
  {
    "modelo": "Porsche Taycan 4S",
    "ano": 2024,
    "motor": "Dois Motores Elétricos",
    "velocidade_maxima": "250 km/h",
    "tipo": "Elétrico"
  },
  {
    "modelo": "Porsche Cayenne Coupé",
    "ano": 2023,
    "motor": "3.0L V6 Turbo",
    "velocidade_maxima": "243 km/h",
    "tipo": "SUV / Combustão"
  }
]
 🐍 Código do Agente Analista (agente.py)

import json
import time

def agente_analista():
    print("🤖 [Agente IA]: Iniciando varredura de dados da Porsche...")
    time.sleep(1.5)
    # Lógica de leitura e exibição dos dados no terminal Termux
