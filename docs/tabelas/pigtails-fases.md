| Sistema | Componente / Função | Tipo de Conector | Vias | Comprimento (cm) | Status | Localização | Observações |
|---------|---------------------|------------------|------|------------------|---------|--------------|--------------|
| {{ site.fases.f1 }} Comunicação | Wideband Nano 2 (CAN) | FT CAN 2 vias | 2 | 30 | Ativo | Painel interno | Comunicação CAN FT |
| {{ site.fases.f1 }} Alimentação | Relés Main / ECU / Bomba / AC | Faston 6.3 mm | 4 | 25 | Ativo | Caixa de relés cofre | Base para todas as fases |
| {{ site.fases.f2 }} Sensores | IAT / ECT | Bosch EV1 selado | 2 | 15 | Ativo | Coletor e cabeçote | Sensores NTC |
| {{ site.fases.f2 }} Sensores | Pressão de Óleo / Combustível | Delphi GT150 | 3 | 20 | Pré-fiação | Filtro e rail | Sensores 0–5 V |
| {{ site.fases.f2 }} Atuadores | Válvula Marcha-lenta (PWM) | Bosch 2 vias | 2 | 20 | Ativo | Próx. TBI | Idle-up A/C e DH |
| {{ site.fases.f2 }} Ventoinhas | Fan 1 / Fan 2 | DT2 / Faston | 2 | 25 | Ativo | Frente do radiador | Estágios 1 e 2 |
|{{ site.fases.f3 }} Ignição | Bobinas Gol G6 (x4) | VW COP 4 vias | 4 | 25 | Pré-fiação | Cabeçote AP | Remover distribuidor |
|{{ site.fases.f3 }} Ignição | Sensor rotação 60-2 | Hall 3 pinos | 3 | 20 | Ativo | Polia virabrequim | Sinal principal |
| {{ site.fases.f4 }} Alimentação | Bomba 255 LPH | Faston reforçado | 2 | 25 | Ativo | Próx. tanque | Circuito dedicado |
| {{ site.fases.f5 }} Atuadores | Solenoide Boost (PWM) | Bosch EV1 2 pinos | 2 | 20 | Pré-fiação | Firewall dir. | AUX5 PWM 20–30 Hz |
| {{ site.fases.f5 }} Sensores | MAP Externo 3–4 bar | Bosch Mini 3 pinos | 3 | 15 | Pré-fiação | Firewall | Ativar fase turbo |
| Reservas | Flex Fuel / Press. Turbo | DT3 selado | 3 | 15 | Reserva | Firewall / cofre | Opcional futuro |