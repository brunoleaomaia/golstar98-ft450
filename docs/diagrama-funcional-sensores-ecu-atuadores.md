---
layout: default
title: Diagrama Funcional (Sensores → ECU → Atuadores)
nav_order: 8
---

# 🔄 Diagrama Funcional – Sensores → ECU → Atuadores

Este diagrama resume o fluxo funcional entre sensores, a ECU FuelTech FT450 e os atuadores do motor, organizando os sinais por fase de evolução do projeto.

---

## 📊 Tabela de Sinais Funcionais

| Origem (Sensor) | Tipo de Sinal | Entrada FT450 | Saída (Atuador) | Descrição / Lógica | Fase |
|------------------|----------------|----------------|------------------|---------------------|------|
| TPS (posição borboleta) | 0–5 V | AN1 | Injetores A–D | Correção de aceleração e carga | 🟩 |
| Sinal Hall distribuidor | Pulso Hall | RPM IN | IGN A–B | Sincronismo de ignição (OEM) | 🟩 |
| IAT (temp. do ar) | NTC | AN2 | Injeção / Ignição | Compensação térmica | 🟦 |
| ECT (temp. do motor) | NTC | AN3 | Ventoinhas | Controle térmico e corte de segurança | 🟦 |
| Pressão de óleo | 0–5 V | AN4 | Proteções | Corte por falha de pressão | 🟦 |
| Pressão de combustível | 0–5 V | AN5 | Proteções | Delta P combustível/MAP | 🟦 |
| Sensor rotação 60-2 (Hall) | Hall | RPM IN | IGN A–D | Ignição sequencial (bobinas G6) | 🟧 |
| MAP externo 3–4 bar | 0–5 V | AN6 | Boost Control | Controle de pressão (PWM) | ⚫ |
| AUX5 PWM | PWM | — | Solenoide 3 vias | Controle de boost | ⚫ |

---

## ⚙️ Lógica de Processamento

1. **Entradas analógicas** (TPS, IAT, ECT, Pressões) → definem as condições de operação do motor.  
2. **Entradas digitais** (Hall, AC Request, DH) → controlam modos auxiliares e marcha-lenta.  
3. **Processamento interno** → a FT450 aplica correções, compensações e limites definidos.  
4. **Saídas digitais/PWM** → acionam atuadores, relés e ventiladores conforme a fase ativa.  

---

## 🧠 Observações

- A FT450 opera em malha fechada via **Wideband Nano 2 (CAN)** para AFR.  
- Todos os sensores devem ser calibrados no **FTManager** antes do primeiro start.  
- A ECU possui entradas e saídas livres suficientes para expansão até a Fase ⚫ Turbo.  

---

_Conteúdo do rodapé disponível em [rodape.md](rodape.md)._
