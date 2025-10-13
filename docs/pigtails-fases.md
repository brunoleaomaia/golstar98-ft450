---
layout: default
title: Pigtails por Fase
nav_order: 13
---

# 🧮 Pigtails por Fase – Resumo de Ativação

Tabela de todos os pigtails previstos no chicote definitivo do GolStar98, indicando status (ativo, pré-fiação ou reserva) e a fase de utilização.

---

## 📋 Tabela Resumida

| Fase | Sistema | Componente / Função | Tipo de Conector | Vias | Comprimento (cm) | Status | Localização | Observações |
|------|----------|---------------------|------------------|------|------------------|---------|--------------|--------------|
| 🟩 | Comunicação | Wideband Nano 2 (CAN) | FT CAN 2 vias | 2 | 30 | ✅ Ativo | Painel interno | Comunicação CAN FT |
| 🟩 | Alimentação | Relés Main / ECU / Bomba / AC | Faston 6.3 mm | 4 | 25 | ✅ Ativo | Caixa de relés cofre | Base para todas as fases |
| 🟦 | Sensores | IAT / ECT | Bosch EV1 selado | 2 | 15 | ✅ Ativo | Coletor e cabeçote | Sensores NTC |
| 🟦 | Sensores | Pressão de Óleo / Combustível | Delphi GT150 | 3 | 20 | ⚙️ Pré-fiação | Filtro e rail | Sensores 0–5 V |
| 🟦 | Atuadores | Válvula Marcha-lenta (PWM) | Bosch 2 vias | 2 | 20 | ✅ Ativo | Próx. TBI | Idle-up A/C e DH |
| 🟦 | Ventoinhas | Fan 1 / Fan 2 | DT2 / Faston | 2 | 25 | ✅ Ativo | Frente do radiador | Estágios 1 e 2 |
| 🟧 | Ignição | Bobinas Gol G6 (x4) | VW COP 4 vias | 4 | 25 | ⚙️ Pré-fiação | Cabeçote AP | Remover distribuidor |
| 🟧 | Ignição | Sensor rotação 60-2 | Hall 3 pinos | 3 | 20 | ✅ Ativo | Polia virabrequim | Sinal principal |
| 🟥 | Alimentação | Bomba 255 LPH | Faston reforçado | 2 | 25 | ✅ Ativo | Próx. tanque | Circuito dedicado |
| ⚫ | Atuadores | Solenoide Boost (PWM) | Bosch EV1 2 pinos | 2 | 20 | ⚙️ Pré-fiação | Firewall dir. | AUX5 PWM 20–30 Hz |
| ⚫ | Sensores | MAP Externo 3–4 bar | Bosch Mini 3 pinos | 3 | 15 | ⚙️ Pré-fiação | Firewall | Ativar fase turbo |
| — | Reservas | Flex Fuel / Press. Turbo | DT3 selado | 3 | 15 | 💤 Reserva | Firewall / cofre | Opcional futuro |

---

## 🔧 Observações
- Todos os pigtails acima devem ser incluídos **desde a montagem inicial do chicote**.  
- Pigtails pré-fiação devem ser **isolados e identificados** com etiqueta termoencolhível.  
- Recomenda-se usar **malha trançada** para agrupamento por sistema (sensores, atuadores, potência).  
- A expansão até a Fase ⚫ Turbo pode ser feita sem refazer o chicote principal.  

---

_Conteúdo do rodapé disponível em [rodape.md](rodape.md)._
