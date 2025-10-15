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

## Lógica de Operação por Fase

A seguir são descritas as fases de operação do sistema de gerenciamento eletrônico do **GolStar98** utilizando a **ECU FuelTech FT450**.  
Cada fase representa uma etapa evolutiva da configuração, com diferentes sensores, atuadores e estratégias de controle.

### {{site.fases.f1}} Fase 1 – Base Aspirada
{: .text-delta }
- Leitura de TPS, MAP interno, rotação e temperatura (ECT).  
- Controle de injeção em modo batch (INJ A–D).  
- Ignição por distribuidor (IGN A–B).  
- Acionamento da bomba via relé (AUX1).  

### {{site.fases.f2}} Fase 2 – Sensores e Proteções
{: .text-delta }
- Ativação de sensores auxiliares: IAT, ECT, Pressão de Óleo e Combustível.  
- Lógica de **idle-up** para A/C e direção hidráulica.  
- Acionamento automático dos ventiladores (AUX2 e AUX3).  
- Ativação de failsafes (óleo, combustível e temperatura).  

### {{site.fases.f3}} Fase 3 – Ignição Moderna
{: .text-delta }
- Substituição do distribuidor por roda fônica 60-2 e bobinas individuais (COP).  
- FT450 passa a gerar **sincronismo sequencial**.  
- Ajuste de avanço por rotação e carga.  

### {{site.fases.f4}} Fase 4 – Alimentação Definitiva
{: .text-delta }
- Controle refinado de bomba de combustível 255 LPH.  
- Monitoramento ativo de pressão e delta MAP/Combustível.  

### {{site.fases.f5}}  Fase 5 – Turbo
{: .text-delta }
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

[Home](index){: .btn .mb-4 .mb-md-0 .mr-2 }
[Chicote e Pinagem](chicote-pinagem){: .btn .btn-primary  .mb-4 .mb-md-0 .mr-2 }

---

{% include_relative rodape.md %}
