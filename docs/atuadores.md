---
layout: default
title: Atuadores
nav_order: 11
---

# ⚙️ Atuadores – GolStar98 FT450

Esta seção descreve os atuadores controlados pela ECU FuelTech FT450 no projeto GolStar98, suas características elétricas, funções e fases de ativação.

---

## 🧩 Tabela de Atuadores

| Atuador | Tipo / Sinal | Saída FT450 | Alimentação | Função | Observações | Fase |
|----------|---------------|--------------|--------------|----------|--------------|------|
| Injetores 1–4 | PWM (positivo) | INJ A–D | 12 V (pós-chave) | Injeção de combustível | Injetores originais multiponto (OEM) | 🟩 |
| Bobinas duplas (1–4 / 2–3) | Digital | IGN A–B | 12 V (pós-chave) | Ignição original via distribuidor | Fase base aspirada | 🟩 |
| Bobinas individuais (COP Gol G6) | Digital | IGN A–D | 12 V (pós-chave) | Ignição sequencial | Exige roda fônica 60-2 | 🟧 |
| Válvula marcha-lenta (PWM) | PWM 150–300 Hz | AUX6 | 12 V (pós-chave) | Controle de ar de marcha-lenta | Idle-up A/C e DH | 🟦 |
| Ventoinha 1 (Fan baixa) | Digital | AUX2 | 12 V direto (via relé) | Resfriamento estágio 1 | Controlada por ECT | 🟦 |
| Ventoinha 2 (Fan alta) | Digital | AUX3 | 12 V direto (via relé) | Resfriamento estágio 2 | Ativada por temperatura alta | 🟦 |
| Bomba de combustível | Digital | AUX1 | 12 V direto (via relé) | Alimentação do sistema | Atualizada p/ 255 LPH na F4 | 🟥 |
| Solenoide de boost | PWM 20–30 Hz | AUX5 | 12 V (via relé) | Controle de pressão turbo | Fase final (turbo-ready) | ⚫ |
| AC Clutch | Digital | AUX4 | 12 V (via relé) | Acionamento do compressor A/C | Corte WOT configurável | 🟦 |
| Conta-giros painel | Digital | AUX7 | — | Saída de RPM | Configurável FTManager | 🟩 |

---

## 🔧 Especificações elétricas

- Todos os atuadores devem ser **alimentados via relé** com proteção individual.  
- As saídas da ECU são **ativas por pulso negativo (sink)** — relés e solenoides devem ser conectados ao +12 V.  
- O **dwell time** das bobinas COP deve ser ajustado conforme o modelo G6 (2,5–3,5 ms típico).  
- A válvula PWM de marcha-lenta deve operar entre **150–300 Hz**.  
- Ventoinhas devem ter retorno de feedback de corrente para diagnóstico (opcional).

---

_Conteúdo do rodapé disponível em [rodape.md](rodape.md)._
