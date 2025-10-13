---
layout: default
title: Roadmap de Evolução
nav_order: 3
---

# 🧭 Roadmap de Evolução – GolStar98 FT450

O projeto **GolStar98** foi estruturado em cinco fases de evolução planejadas, garantindo compatibilidade elétrica e lógica entre o sistema original aspirado e a configuração turbo-ready.

---

## 📈 Fases de Evolução

| Fase | Ícone | Nome | Descrição |
|------|-------|------|------------|
| 🟩 | Fase 1 | Base aspirada | Instalação da FT450 e Wideband CAN. Mantém injeção, bomba e ignição originais (distribuidor). Validação inicial e funcionamento básico. |
| 🟦 | Fase 2 | Sensores e proteções | Adição de sensores auxiliares (IAT, ECT, pressão de óleo e combustível). Ativação de failsafes e compensações térmicas. Idle-up do A/C e direção hidráulica. |
| 🟧 | Fase 3 | Ignição moderna | Instalação da roda fônica 60-2 e bobinas individuais Gol G6. Remoção do distribuidor e ativação da ignição sequencial COP. |
| 🟥 | Fase 4 | Alimentação definitiva | Substituição da bomba de combustível por 255 LPH e revisão de regulador/retorno. Validação de pressão de linha e delta combustível-MAP. |
| ⚫ | Fase 5 | Turbo | Instalação de kit turbo, solenoide PWM e MAP 3–4 bar. Ajuste de AFR e avanço por pressão, com proteções em malha fechada. |

---

## 🔄 Dependências entre fases

- A fiação e a ECU são **comuns a todas as fases**.  
- Cada nova etapa **ativa sensores ou atuadores** previamente instalados.  
- As configurações do FTManager devem ser salvas como `FT450_FASE_X.FTM`.  
- O chicote principal permanece **único e definitivo** (Turbo-Ready).  

---

## 🧱 Estrutura modular do sistema

Cada grupo de componentes evolui de forma independente, mas compatível:

| Subsistema | F1 | F2 | F3 | F4 | F5 |
|-------------|----|----|----|----|----|
| ECU / Alimentação | 🟩 | 🟩 | 🟩 | 🟩 | 🟩 |
| Sensores | — | 🟦 | 🟦 | 🟦 | ⚫ |
| Ignição | 🟩 | 🟩 | 🟧 | 🟧 | 🟧 |
| Combustível | 🟩 | 🟩 | 🟩 | 🟥 | 🟥 |
| Turbo / Boost | — | — | — | — | ⚫ |

---

## ⚙️ Recomendações gerais

- Realizar testes elétricos e de continuidade antes de cada nova fase.  
- Manter logs de calibração, mapas e versões de firmware.  
- Revisar terminais e conectores a cada atualização física.  
- Utilizar apenas sensores homologados pela FuelTech ou de padrão equivalente.  

---

_Conteúdo do rodapé disponível em [rodape.md](rodape.md)._
