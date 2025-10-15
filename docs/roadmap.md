---
layout: default
title: Roadmap de Evolução
nav_order: 2
---
# Roadmap de Evolução
Este projeto foi estruturado em cinco fases de evolução planejadas, garantindo compatibilidade elétrica e lógica desde o sistema `original aspirado` até a fase `turbo`.

---

## Fases do Projeto
{% capture tabela_fases %}
{% include_relative tabelas/fases-do-projeto.md %}
{% endcapture %}
{{ tabela_fases | markdownify }}

{: .new-title .fs-2 }
> Dependências entre Fases
>
> - O Chicote e a ECU são **comuns a todas as fases**.  
> - Cada nova etapa **ativa sensores ou atuadores** previamente instalados.  
> - As configurações do FTManager devem ser salvas como `FT450_FASE_X.FTM`.  
> - O chicote principal permanece **único e definitivo** (Turbo-Ready).

---

## Diagrama Lógico

O diagrama lógico representa o comportamento interno da ECU FT450 e a relação entre as condições de entrada e os comandos de saída em cada fase de operação do GolStar98.

### Lógica de Operação por Sistemas

#### {{site.fases.f1}} Fase 1 – Base Aspirada
- Leitura de TPS, MAP interno, rotação e temperatura (ECT).  
- Controle de injeção em modo batch (INJ A–D).  
- Ignição por distribuidor (IGN A–B).  
- Acionamento da bomba via relé (AUX1).  

#### {{site.fases.f2}} Fase 2 – Sensores e Proteções
- Ativação de sensores auxiliares: IAT, ECT, Pressão de Óleo e Combustível.  
- Lógica de **idle-up** para A/C e direção hidráulica.  
- Acionamento automático dos ventiladores (AUX2 e AUX3).  
- Ativação de failsafes (óleo, combustível e temperatura).  

#### {{site.fases.f3}} Fase 3 – Ignição Moderna
- Substituição do distribuidor por roda fônica 60-2 e bobinas individuais (COP).  
- FT450 passa a gerar **sincronismo sequencial**.  
- Ajuste de avanço por rotação e carga.  

#### {{site.fases.f4}} Fase 4 – Alimentação Definitiva
- Controle refinado de bomba de combustível 255 LPH.  
- Monitoramento ativo de pressão e delta MAP/Combustível.  

#### {{site.fases.f5}}  Fase 5 – Turbo
- Adição de controle de **solenoide PWM** para boost.  
- Ativação de sensor MAP 3–4 bar.  
- Ajustes de AFR e avanço por pressão (malha fechada).  

{: .new-title .fs-2 }
>Observações Técnicas
> - Cada saída AUX é configurável individualmente no **FTManager**.  
> - Estratégias de proteção (cut, limiter, correção) podem ser aplicadas a qualquer entrada analógica.  
> - A FT450 suporta operação full-sequential com até 4 cilindros.  
> - Os mapas devem ser versionados conforme o avanço das fases.  


---

{% include_relative rodape.md %}
