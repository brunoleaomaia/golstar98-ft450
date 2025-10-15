---
layout: default
title: Checklists
nav_order: 5
---

# Checklist de Comissionamento

Este checklist define as etapas obrigatórias de verificação elétrica, lógica e funcional para cada fase da evolução do sistema de gerenciamento do GolStar98.

---

## Etapas de Verificação por Fase

| Etapa | Verificação | Fase |
|--------|--------------|------|
| Verificação inicial | Conferir polaridade e continuidade de todos os circuitos. | {{site.fases.f1}} Fase 1 |
| Teste de sensores | Checar leitura de TPS, IAT, ECT e MAP (interno). | {{site.fases.f2}} Fase 2 |
| Marcha-lenta | Ajustar idle com A/C ligado e verificar resposta da válvula PWM. | {{site.fases.f2}} Fase 2 |
| Ignição | Validar rotação com roda fônica e sincronismo das bobinas G6. | {{site.fases.f3}} Fase 3 |
| Alimentação | Testar pressão da linha com bomba 255 LPH e retorno ativo. | {{site.fases.f4}} Fase 4  |
| Turbo | Conferir funcionamento do MAP 3–4 bar e da solenoide PWM. | {{site.fases.f5}} Fase 5  |

{: .new-title .fs-2 }
> Procedimentos Adicionais
> - Confirmar leitura estável dos sensores antes do primeiro start.  
> - Verificar se todos os GNDs estão bem fixados e de baixa resistência (<0,1 Ω).  
> - Validar os cortes de proteção (óleo, combustível, temperatura) no software FTManager.  
> - Checar tensão de alimentação da ECU (mínimo 11,8 V em partida).  
> - Garantir aterramento separado para sensores e atuadores de potência.  
> - Após cada atualização de fase, executar backup da configuração `.FTM`.

---

[Sensores e Atuadores](sensores-atuadores){: .btn .mb-4 .mb-md-0 .mr-2 }
[Changelog](changelog){: .btn .btn-primary .mb-4 .mb-md-0 .mr-2 }

---
{% include_relative rodape.md %}
