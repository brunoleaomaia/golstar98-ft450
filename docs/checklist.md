---
layout: default
title: Checklist de Comissionamento
nav_order: 5
---

# ✅ Checklist de Comissionamento – GolStar98 FT450

Este checklist define as etapas obrigatórias de verificação elétrica, lógica e funcional para cada fase da evolução do sistema de gerenciamento do GolStar98.

---

## 🧩 Etapas de verificação por fase

| Etapa | Verificação | Fase |
|--------|--------------|------|
| Verificação inicial | Conferir polaridade e continuidade de todos os circuitos. | 🟩 |
| Teste de sensores | Checar leitura de TPS, IAT, ECT e MAP (interno). | 🟦 |
| Marcha-lenta | Ajustar idle com A/C ligado e verificar resposta da válvula PWM. | 🟦 |
| Ignição | Validar rotação com roda fônica e sincronismo das bobinas G6. | 🟧 |
| Alimentação | Testar pressão da linha com bomba 255 LPH e retorno ativo. | 🟥 |
| Turbo | Conferir funcionamento do MAP 3–4 bar e da solenoide PWM. | ⚫ |

---

## ⚙️ Procedimentos adicionais
- Confirmar leitura estável dos sensores antes do primeiro start.  
- Verificar se todos os GNDs estão bem fixados e de baixa resistência (<0,1 Ω).  
- Validar os cortes de proteção (óleo, combustível, temperatura) no software FTManager.  
- Checar tensão de alimentação da ECU (mínimo 11,8 V em partida).  
- Garantir aterramento separado para sensores e atuadores de potência.  
- Após cada atualização de fase, executar backup da configuração `.FTM`.

---

_Conteúdo do rodapé disponível em [rodape.md](rodape.md)._
