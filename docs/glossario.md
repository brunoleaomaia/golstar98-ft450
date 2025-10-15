---
layout: page
title: Glossário
nav_order: 100
---

# Glossário
{: .no_toc }
Lista de siglas, abreviações e termos técnicos utilizados em toda a documentação do projeto **GolStar98 FT450**.

---

## Nesta Página
{: .no_toc .text-delta}

1. TOC
{:toc}

---

## Siglas e Termos Técnicos

- **A/C** - *Ar Condicionado* – sistema de climatização do veículo, controlado pela ECU via sinal “AC Request” e relé do compressor.
- **AFR** - *Air-Fuel Ratio* – razão ar/combustível. Indicador da mistura (14,7:1 é a estequiométrica para gasolina). Monitora-se via sonda wideband.
- **ANx** - *Analog Input* – entradas analógicas da FT450 (ex.: AN1, AN2...) usadas para sensores de 0–5 V ou NTC.
- **AUXx** - *Auxiliary Output* – saídas auxiliares configuráveis da ECU (ex.: AUX1–AUX7) usadas para ventoinhas, solenoides, bomba, etc.
- **CAN** - *Controller Area Network* – protocolo de comunicação digital entre módulos (usado pela Wideband Nano 2 e outros dispositivos FuelTech).
- **COP** - *Coil-On-Plug* – bobinas individuais montadas diretamente sobre as velas, eliminando o distribuidor mecânico.
- **DH** - *Direção Hidráulica* – sistema de assistência de direção. Pode gerar sinal de pressão para idle-up.
- **DIx** - *Digital Input* – entradas digitais da ECU (ex.: DI1, DI2) para sinais on/off como AC Request ou Pressão DH.
- **ECT** - *Engine Coolant Temperature* – temperatura do líquido de arrefecimento do motor, medida por sensor NTC.
- **ECU** - *Electronic Control Unit* – unidade eletrônica de controle (neste caso, a FuelTech FT450). Responsável por gerenciar ignição, injeção e proteções.
- **EV1/EV6** - Padrões de conectores Bosch usados em injetores e solenoides automotivos.
- **FuelTech/FT** - Fabricante brasileira de ECUs e acessórios de gerenciamento eletrônico automotivo.
- **FT450** - Modelo de ECU da FuelTech, com suporte a 4 cilindros, sensores analógicos, saídas PWM e comunicação CAN.
- **FTManager** - Software oficial da FuelTech usado para configuração, calibração e diagnóstico da ECU FT450.
- **GND** - *Ground* – terra elétrico. Referência de 0 V para todos os sensores e atuadores.
- **Hall** - Tipo de sensor que gera sinal digital de rotação/fase através de um campo magnético.
- **IAT** - *Intake Air Temperature* – temperatura do ar admitido, medida por sensor NTC instalado no coletor.
- **IGNx** - *Ignition Output* – saídas de ignição da FT450 (IGN A–D), usadas para acionar bobinas.
- **INJx** - *Injector Output* – saídas de injeção da ECU (INJ A–D), controlam os bicos injetores.
- **Lambda** - Sensor de oxigênio usado para medir AFR. Pode ser narrowband (OEM) ou wideband (preciso).
- **LED** - *Light Emitting Diode* – Indicadores luminosos usados na ECU e painéis.
- **LPH** - *Litros por Hora* – unidade de medida de vazão de bomba de combustível (ex.: 255 LPH).
- **MAP** - *Manifold Absolute Pressure* – sensor de pressão absoluta do coletor. Mede vácuo e sobrepressão.
- **NTC** - *Negative Temperature Coefficient* – tipo de sensor resistivo cuja resistência diminui com o aumento da temperatura. Usado em IAT e ECT.
- **OEM** - *Original Equipment Manufacturer* – peças originais do veículo, conforme especificações de fábrica.
- **PWM** - *Pulse Width Modulation* – modulação por largura de pulso. Técnica usada pela ECU para controlar a velocidade ou fluxo (ex.: válvula de marcha-lenta, solenoide boost).
- **RPM IN** - Entrada de rotação da ECU, que recebe o sinal do sensor Hall (distribuidor ou roda fônica).
- **TBI** - *Throttle Body Injection* – corpo de borboleta onde está instalado o sensor TPS e a válvula de marcha-lenta.
- **TPS** - *Throttle Position Sensor* – sensor de posição da borboleta, fornece à ECU o ângulo de abertura (0–100%).
- **Turbo-Ready** - Termo usado para designar o chicote e a instalação elétrica já preparados para futura adição de turbocompressor.
- **Wideband** - Sensor de oxigênio de banda larga. Mede AFR com precisão em diferentes misturas (utilizado em malha fechada).
- **WOT** - *Wide Open Throttle* – borboleta totalmente aberta. Condição de plena carga usada para ajustes de AFR e avanço.

---

## Conectores e Componentes

- **Faston** - Terminal macho/fêmea padrão automotivo, usado em relés e fusíveis.
- **Deutsch DT / DTM** - Conector selado de alta confiabilidade, usado em ambientes de cofre do motor.
- **Delphi GT150 / GT280** - Linha de conectores selados usada em sensores de pressão.
- **Bosch EV1** - Conector clássico de injetores e sensores automotivos.
- **COP Gol G6** - Conjunto de bobinas individuais (4 vias) utilizadas na ignição moderna do projeto.

---

## Termos Técnicos Complementares

- **Failsafe:** Estratégia de segurança que corta ignição/injeção em caso de falha de sensores críticos.  
- **Idle-up:** Aumento automático da rotação de marcha-lenta quando o A/C ou a direção hidráulica são acionados.  
- **Malha fechada:** Controle automático que ajusta mistura ou pressão com base no feedback de sensores.  
- **Dwell:** Tempo de carga da bobina antes da faísca.  
- **Delta P (Combustível/MAP):** Diferença entre pressão de combustível e pressão no coletor, usada para compensação de injeção.  
- **Cut:** Corte de ignição/injeção configurado como proteção ou limitador.  

---

## Pigtails e Subchicotes

Os pigtails são extensões curtas de fiação com conectores já montados e terminais crimpados, usados para interligar o chicote principal aos sensores, atuadores e relés.

| Tipo | Aplicação | Exemplo de conector |
|------|------------|----------------------|
| Sensor | IAT, ECT, Pressão óleo, MAP | Bosch EV1 / Delphi GT150 |
| Atuador | Solenoide PWM, Válvula Idle | Bosch EV1 / 2 pinos |
| Ignição | Bobinas COP Gol G6 | VW COP 4 vias |
| Comunicação | Wideband CAN | Conector FT 2 vias |
| Alimentação | Relés / Ventoinhas | Faston / DT2 |
| Reserva | Futuros sensores | DT3 selado |

Um pigtail é composto por:
- Conector automotivo (Bosch, Delphi, Sumitomo, Deutsch, etc.);
- Fios entre **10 e 25 cm**, normalmente selados e protegidos;
- Identificação termoencolhível com nome da função;
- Proteção com malha trançada ou fita antiabrasiva.

Eles permitem:
- Substituição rápida de sensores sem cortar o chicote;
- Adaptação entre padrões de conectores (OEM → FT);
- Absorção de vibração e calor do motor;
- Modularidade e facilidade de manutenção.

{: .new-title .fs-2 }
>Boas práticas de montagem
> - Usar **crimpagem profissional**, nunca solda.  
> - Testar continuidade e isolamento antes da instalação.  
> - Isolar pontas não usadas com **termo-retrátil com cola**.  
> - Identificar cada pigtail conforme a tabela de pinagem FT450.  
> - Prever **loops de folga** de 10–15 cm para manutenção.  
> - Agrupar pigtails por sistemas (sensores, ignição, potência).  

{: .highlight-title .fs-2 }
> Observações para o GolStar98
> - Pigtails “cegos” devem ser instalados desde a Fase 1 {{site.fases.f1}} Base Aspirada, identificados e isolados.  
> - Todos os conectores devem ser selados (IP67 ou superior).  
> - A transição de chicote principal → subchicote deve usar **plugs multi-vias selados**.  
> - As bitolas seguem o padrão do chicote principal (0,5 a 2,5 mm²).

---

## Notas Finais

- Todas as siglas aqui listadas aparecem nos documentos técnicos do repositório.  
- Este glossário deve ser atualizado sempre que novos sensores, atuadores ou termos forem adicionados.  
- As descrições seguem o padrão técnico da FuelTech e do setor automotivo

---

[Changelog](changelog){: .btn .mb-4 .mb-md-0 .mr-2 }
[Roadmap de Evolução](roadmap){: .btn .btn-primary .mb-4 .mb-md-0 .mr-2 }

---

{% include_relative rodape.md %}