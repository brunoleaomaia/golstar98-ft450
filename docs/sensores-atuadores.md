---
layout: default
title: Sensores e Atuadores
nav_order: 4
---

# Sensores e Atuadores

Lista dos sensores e atuad instalados ou previstos no projeto, suas funções, características elétricas e a fase em que entram em operação.

---

## Tabela de Sensores
{% capture tabela_sensores %}
{% include_relative tabelas/sensores.md %}
{% endcapture %}
{{ tabela_sensores | markdownify }}

{: .new-title .fs-2 }
> Notas Técnicas
> - Todos os sensores NTC devem usar cabos blindados com retorno de sinal ao pino GND da ECU.  
> - Sensores de pressão 0–5 V devem compartilhar a referência 5 V estabilizada da FT450.  
> - O sensor **MAP interno** é suficiente até ~0,8 bar de pressão positiva (limite aspirado).  
> - O **MAP externo 3–4 bar** deve ser ativado na Fase {{site.fases.f5}}Turbo.  

---

## Tabela de Atuadores
{% capture tabela_atuadores %}
{% include_relative tabelas/atuadores.md %}
{% endcapture %}
{{ tabela_atuadores | markdownify }}

{: .new-title .fs-2 }
> Notas Técnicas
> - Todos os atuadores devem ser **alimentados via relé** com proteção individual.  
> - As saídas da ECU são **ativas por pulso negativo (sink)** — relés e solenoides devem ser conectados ao +12 V.  
> - O **dwell time** das bobinas COP deve ser ajustado conforme o modelo G6 (2,5–3,5 ms típico).  
> - A válvula PWM de marcha-lenta deve operar entre **150–300 Hz**.  
> - Ventoinhas devem ter retorno de feedback de corrente para diagnóstico (opcional).

---

[Chicotes e Pinagem](chicotes-pinagem){: .btn .mb-4 .mb-md-0 .mr-2 }
[Checklists](checklists){: .btn .btn-primary .mb-4 .mb-md-0 .mr-2 }

---

{% include_relative rodape.md %}
