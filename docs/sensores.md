---
layout: default
title: Sensores
nav_order: 10
---

# 🌡️ Sensores – GolStar98 FT450

Lista dos sensores instalados ou previstos no projeto, suas funções, características elétricas e a fase em que entram em operação.

---

## 📋 Tabela de Sensores

| Sensor | Tipo | Local de Instalação | Entrada FT450 | Faixa de Operação | Alimentação | Observações | Fase |
|---------|-------|---------------------|----------------|--------------------|--------------|--------------|------|
| TPS – Posição da borboleta | Potenciômetro 3 pinos | TBI original | AN1 | 0–5 V | 5 V / GND | Ajustar via FTManager (100%/0%) | 🟩 |
| MAP interno | Sensor de pressão absoluto | Corpo da ECU | Interno | 0–1 bar | — | Usado até instalação do turbo | 🟩 |
| IAT – Temp. do ar | NTC | Coletor de admissão | AN2 | -20 °C a 120 °C | 5 V / GND | Bosch padrão GM | 🟦 |
| ECT – Temp. do motor | NTC | Cabeçote original | AN3 | -20 °C a 120 °C | 5 V / GND | Calibrar curva NTC | 🟦 |
| Pressão de óleo | Transdutor 0–5 V | Perto do filtro | AN4 | 0–150 psi | 5 V / GND | PS150 ou PS300 | 🟦 |
| Pressão de combustível | Transdutor 0–5 V | Linha de combustível | AN5 | 0–100 psi | 5 V / GND | Permite delta P | 🟦 |
| MAP externo 3–4 bar | Transdutor 0–5 V | Firewall (dir.) | AN6 | 0–400 kPa | 5 V / GND | Fase turbo | ⚫ |
| Sensor de rotação | Hall 3 fios | Polia do virabrequim | RPM IN | 60-2 dentes | 12 V / GND | Sensor Fiat 3 pinos | 🟧 |
| Sensor de fase (opcional) | Hall 3 fios | Comando / distribuidor | DI3 | 1 dente | 12 V / GND | Para sequential COP | ⚫ |
| AC Request | Digital | Botão painel A/C | DI1 | — | — | Idle-up automático | 🟦 |
| Pressão DH | Digital | Linha de direção hidráulica | DI2 | — | — | Idle-up adicional | 🟦 |
| Lambda – Wideband | CAN | Painel interno | CAN | AFR 0,65–1,35 | CAN FT | Nano 2 em malha fechada | 🟩 |

---

## ⚙️ Notas Técnicas
- Todos os sensores NTC devem usar cabos blindados com retorno de sinal ao pino GND da ECU.  
- Sensores de pressão 0–5 V devem compartilhar a referência 5 V estabilizada da FT450.  
- O sensor **MAP interno** é suficiente até ~0,8 bar de pressão positiva (limite aspirado).  
- O **MAP externo 3–4 bar** deve ser ativado na Fase ⚫ Turbo.  

---

_Conteúdo do rodapé disponível em [rodape.md](rodape.md)._
