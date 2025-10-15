
| Fase | Origem (Sensor) | Tipo de Sinal | Entrada FT450 | Saída (Atuador) | Descrição / Lógica |
|---|------------------|----------------|----------------|------------------|---------------------|
|{{site.fases.f1}} Fase 1| TPS (posição borboleta) | 0–5 V | AN1 | Injetores A–D | Correção de aceleração e carga |
|{{site.fases.f1}} Fase 1| Sinal Hall distribuidor | Pulso Hall | RPM IN | IGN A–B | Sincronismo de ignição (OEM) |
|{{site.fases.f2}} Fase 2| IAT (temp. do ar) | NTC | AN2 | Injeção / Ignição | Compensação térmica |
|{{site.fases.f2}} Fase 2| ECT (temp. do motor) | NTC | AN3 | Ventoinhas | Controle térmico e corte de segurança |
|{{site.fases.f2}} Fase 2| Pressão de óleo | 0–5 V | AN4 | Proteções | Corte por falha de pressão |
|{{site.fases.f2}} Fase 2| Pressão de combustível | 0–5 V | AN5 | Proteções | Delta P combustível/MAP |
|{{site.fases.f3}} Fase 3| Sensor rotação 60-2 (Hall) | Hall | RPM IN | IGN A–D | Ignição sequencial (bobinas G6) |
|{{site.fases.f5}} Fase 5| MAP externo 3–4 bar | 0–5 V | AN6 | Boost Control | Controle de pressão (PWM) |
|{{site.fases.f5}} Fase 5| AUX5 PWM | PWM | — | Solenoide 3 vias | Controle de boost |