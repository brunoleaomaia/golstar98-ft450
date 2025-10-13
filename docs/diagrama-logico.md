---
layout: default
title: Diagrama Lógico
nav_order: 9
---

# 🧮 Diagrama Lógico – FT450

O diagrama lógico representa o comportamento interno da ECU FT450 e a relação entre as condições de entrada e os comandos de saída em cada fase de operação do GolStar98.

---

## 🧠 Lógica de Operação por Sistemas

### 🟩 Fase 1 – Base Aspirada
- Leitura de TPS, MAP interno, rotação e temperatura (ECT).  
- Controle de injeção em modo batch (INJ A–D).  
- Ignição por distribuidor (IGN A–B).  
- Acionamento da bomba via relé (AUX1).  

### 🟦 Fase 2 – Sensores e Proteções
- Ativação de sensores auxiliares: IAT, ECT, Pressão de Óleo e Combustível.  
- Lógica de **idle-up** para A/C e direção hidráulica.  
- Acionamento automático dos ventiladores (AUX2 e AUX3).  
- Ativação de failsafes (óleo, combustível e temperatura).  

### 🟧 Fase 3 – Ignição Moderna
- Substituição do distribuidor por roda fônica 60-2 e bobinas individuais (COP).  
- FT450 passa a gerar **sincronismo sequencial**.  
- Ajuste de avanço por rotação e carga.  

### 🟥 Fase 4 – Alimentação Definitiva
- Controle refinado de bomba de combustível 255 LPH.  
- Monitoramento ativo de pressão e delta MAP/Combustível.  

### ⚫ Fase 5 – Turbo
- Adição de controle de **solenoide PWM** para boost.  
- Ativação de sensor MAP 3–4 bar.  
- Ajustes de AFR e avanço por pressão (malha fechada).  

---

## 🔧 Observações Técnicas

- Cada saída AUX é configurável individualmente no **FTManager**.  
- Estratégias de proteção (cut, limiter, correção) podem ser aplicadas a qualquer entrada analógica.  
- A FT450 suporta operação full-sequential com até 4 cilindros.  
- Os mapas devem ser versionados conforme o avanço das fases.  

---

_Conteúdo do rodapé disponível em [rodape.md](rodape.md)._
