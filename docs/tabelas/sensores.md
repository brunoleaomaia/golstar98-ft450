| Sensor | Tipo | Local de Instalação | Entrada FT450 | Faixa de Operação | Alimentação | Observações |
|---------|-------|---------------------|----------------|--------------------|--------------|--------------|
|{{site.fases.f1}} TPS – Posição da borboleta | Potenciômetro 3 pinos | TBI original | AN1 | 0–5 V | 5 V / GND | Ajustar via FTManager (100%/0%) |
|{{site.fases.f1}} MAP interno | Sensor de pressão absoluto | Corpo da ECU | Interno | 0–1 bar | — | Usado até instalação do turbo |
|{{site.fases.f2}} IAT – Temp. do ar | NTC | Coletor de admissão | AN2 | -20 °C a 120 °C | 5 V / GND | Bosch padrão GM |
|{{site.fases.f2}} ECT – Temp. do motor | NTC | Cabeçote original | AN3 | -20 °C a 120 °C | 5 V / GND | Calibrar curva NTC |
|{{site.fases.f2}} Pressão de óleo | Transdutor 0–5 V | Perto do filtro | AN4 | 0–150 psi | 5 V / GND | PS150 ou PS300 |
|{{site.fases.f2}} Pressão de combustível | Transdutor 0–5 V | Linha de combustível | AN5 | 0–100 psi | 5 V / GND | Permite delta P |
|{{site.fases.f5}} MAP externo 3–4 bar | Transdutor 0–5 V | Firewall (dir.) | AN6 | 0–400 kPa | 5 V / GND | Fase turbo |
|{{site.fases.f3}} Sensor de rotação | Hall 3 fios | Polia do virabrequim | RPM IN | 60-2 dentes | 12 V / GND | Sensor Fiat 3 pinos |
|{{site.fases.f5}} Sensor de fase (opcional) | Hall 3 fios | Comando / distribuidor | DI3 | 1 dente | 12 V / GND | Para sequential COP |
|{{site.fases.f2}} AC Request | Digital | Botão painel A/C | DI1 | — | — | Idle-up automático |
|{{site.fases.f2}} Pressão DH | Digital | Linha de direção hidráulica | DI2 | — | — | Idle-up adicional |
|{{site.fases.f2}} Lambda – Wideband | CAN | Painel interno | CAN | AFR 0,65–1,35 | CAN FT | Nano 2 em malha fechada |