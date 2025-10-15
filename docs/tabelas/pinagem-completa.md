| Categoria | Função / Descrição | Pino FT450 (IO) | Destino no carro | Bitola (mm²) | Cor sugerida | Fusível / Relé | Observações |
|------------|-------------------|-----------------|------------------|---------------|---------------|----------------|-------------|
| {{ site.fases.f1 }} Aliment. | +12V Pós-Chave | +12V | Caixa de relés interna | 2.5 | Vermelho | 10 A (Relé Main ECU) | Fio direto do relé principal |
| {{ site.fases.f1 }} Aliment. | Terra principal | GND | Bloco motor / chassi | 2.5 | Preto | — | Terra limpo e curto |
| {{ site.fases.f1 }} Sensor | Sinal Hall distribuidor | RPM IN | Distribuidor 3 pinos | 0.5 | Cinza | — | Cabo blindado |
| {{ site.fases.f1 }} Sensor | TPS (borboleta) | AN1 | TPS original | 0.5 | Verde | — | 5 V / GND / Sinal |
| {{ site.fases.f1 }} Sensor | MAP interno | Interno | Mangueira plenum | — | — | — | Usar até instalação turbo |
| {{ site.fases.f2 }} Sensor | IAT (Temp. Ar) | AN2 | Coletor pós-TBI | 0.5 | Amarelo | — | NTC Bosch/GM |
| {{ site.fases.f2 }} Sensor | ECT (Temp. Motor) | AN3 | Cabeçote (original) | 0.5 | Azul | — | Curva NTC calibrada |
| {{ site.fases.f2 }} Sensor | Pressão de óleo | AN4 | Próx. ao filtro | 0.5 | Branco | — | Sensor 0-5 V PS150 |
| {{ site.fases.f2 }} Sensor | Pressão combustível | AN5 | Rail / linha | 0.5 | Laranja | — | Sensor 0-5 V PS150 |
| {{ site.fases.f2 }} Entrada | AC Request | DI1 | Botão A/C | 0.5 | Roxo | — | Idle-up automático |
| {{ site.fases.f2 }} Entrada | Pressão DH | DI2 | Press switch DH | 0.5 | Roxo/Preto | — | Idle-up adicional |
| {{ site.fases.f1 }} Saída | Injetor 1 | INJ A | Cilindro 1 | 1.0 | Verde/Preto | — | Bico original OEM |
| {{ site.fases.f1 }} Saída | Injetor 2 | INJ B | Cilindro 2 | 1.0 | Azul/Preto | — | Bico original OEM |
| {{ site.fases.f1 }} Saída | Injetor 3 | INJ C | Cilindro 3 | 1.0 | Amarelo/Preto | — | Bico original OEM |
| {{ site.fases.f1 }} Saída | Injetor 4 | INJ D | Cilindro 4 | 1.0 | Vermelho/Preto | — | Bico original OEM |
| {{ site.fases.f1 }} Saída | Bobina dupla (1/4) | IGN A | Distribuidor OEM | 1.0 | Cinza | — | Ignição original |
| {{ site.fases.f1 }} Saída | Bobina dupla (2/3) | IGN B | Distribuidor OEM | 1.0 | Cinza/Preto | — | Ignição original |
| {{ site.fases.f3 }} Saída | Bobinas G6 (4x) | IGN A–D | Cilindros 1–4 | 1.0 | Cinza | — | 4 bobinas individuais |
| {{ site.fases.f4 }} Saída | Bomba combustível | AUX1 | Relé bomba | 2.5 | Vermelho/Azul | 20 A | Bomba OEM → 255 LPH |
| {{ site.fases.f2 }} Saída | Fan Radiador 1 | AUX2 | Relé Fan 1 | 4.0 | Vermelho/Amarelo | 30 A | Estágio 1 |
| {{ site.fases.f2 }} Saída | Fan Radiador 2 | AUX3 | Relé Fan 2 | 4.0 | Vermelho/Verde | 30 A | Estágio 2 |
| {{ site.fases.f2 }} Saída | AC Clutch | AUX4 | Relé AC | 1.5 | Verde/Amarelo | 15 A | Corte WOT configurável |
| {{ site.fases.f5 }} Saída | Solenoide Boost PWM | AUX5 | Solenoide 3 vias | 1.0 | Laranja/Branco | 5 A | Pré-fiação turbo |
| {{ site.fases.f2 }} Saída | Marcha-lenta (PWM) | AUX6 | Válvula Bosch 2 fios | 1.0 | Azul/Branco | 5 A | Idle-up A/C + DH |
| {{ site.fases.f1 }} Saída | Conta-giros painel | AUX7 | Painel Gol | 0.5 | Verde/Branco | — | Saída configurável |