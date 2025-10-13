---
layout: default
title: Chicote e Pinagem
nav_order: 6
---

# 🧵 Chicote – Pinagem e Ligações

Abaixo está a pinagem completa do chicote principal planejado para o projeto **GolStar98 – FT450**, contemplando todas as fases de evolução (aspirada → turbo).

---

## 📋 Tabela de pinagem

| Categoria | Função / Descrição | Pino FT450 (IO) | Destino no carro | Bitola (mm²) | Cor sugerida | Fusível / Relé | Observações | Fase |
|------------|-------------------|-----------------|------------------|---------------|---------------|----------------|-------------|------|
| Alimentação | +12V Pós-Chave | +12V | Caixa de relés interna | 2.5 | Vermelho | 10 A (Relé Main ECU) | Fio direto do relé principal | 🟩 |
| Alimentação | Terra principal | GND | Bloco motor / chassi | 2.5 | Preto | — | Terra limpo e curto | 🟩 |
| Sensor | Sinal Hall distribuidor | RPM IN | Distribuidor 3 pinos | 0.5 | Cinza | — | Cabo blindado | 🟩 |
| Sensor | TPS (borboleta) | AN1 | TPS original | 0.5 | Verde | — | 5 V / GND / Sinal | 🟩 |
| Sensor | MAP interno | Interno | Mangueira plenum | — | — | — | Usar até instalação turbo | 🟩 |
| Sensor | IAT (Temp. Ar) | AN2 | Coletor pós-TBI | 0.5 | Amarelo | — | NTC Bosch/GM | 🟦 |
| Sensor | ECT (Temp. Motor) | AN3 | Cabeçote (original) | 0.5 | Azul | — | Curva NTC calibrada | 🟦 |
| Sensor | Pressão de óleo | AN4 | Próx. ao filtro | 0.5 | Branco | — | Sensor 0-5 V PS150 | 🟦 |
| Sensor | Pressão combustível | AN5 | Rail / linha | 0.5 | Laranja | — | Sensor 0-5 V PS150 | 🟦 |
| Entrada | AC Request | DI1 | Botão A/C | 0.5 | Roxo | — | Idle-up automático | 🟦 |
| Entrada | Pressão DH | DI2 | Press switch DH | 0.5 | Roxo/Preto | — | Idle-up adicional | 🟦 |
| Saída | Injetor 1 | INJ A | Cilindro 1 | 1.0 | Verde/Preto | — | Bico original OEM | 🟩 |
| Saída | Injetor 2 | INJ B | Cilindro 2 | 1.0 | Azul/Preto | — | Bico original OEM | 🟩 |
| Saída | Injetor 3 | INJ C | Cilindro 3 | 1.0 | Amarelo/Preto | — | Bico original OEM | 🟩 |
| Saída | Injetor 4 | INJ D | Cilindro 4 | 1.0 | Vermelho/Preto | — | Bico original OEM | 🟩 |
| Saída | Bobina dupla (1/4) | IGN A | Distribuidor OEM | 1.0 | Cinza | — | Ignição original | 🟩 |
| Saída | Bobina dupla (2/3) | IGN B | Distribuidor OEM | 1.0 | Cinza/Preto | — | Ignição original | 🟩 |
| Saída | Bobinas G6 (4x) | IGN A–D | Cilindros 1–4 | 1.0 | Cinza | — | 4 bobinas individuais | 🟧 |
| Saída | Bomba combustível | AUX1 | Relé bomba | 2.5 | Vermelho/Azul | 20 A | Bomba OEM → 255 LPH | 🟥 |
| Saída | Fan Radiador 1 | AUX2 | Relé Fan 1 | 4.0 | Vermelho/Amarelo | 30 A | Estágio 1 | 🟦 |
| Saída | Fan Radiador 2 | AUX3 | Relé Fan 2 | 4.0 | Vermelho/Verde | 30 A | Estágio 2 | 🟦 |
| Saída | AC Clutch | AUX4 | Relé AC | 1.5 | Verde/Amarelo | 15 A | Corte WOT configurável | 🟦 |
| Saída | Solenoide Boost PWM | AUX5 | Solenoide 3 vias | 1.0 | Laranja/Branco | 5 A | Pré-fiação turbo | ⚫ |
| Saída | Marcha-lenta (PWM) | AUX6 | Válvula Bosch 2 fios | 1.0 | Azul/Branco | 5 A | Idle-up A/C + DH | 🟦 |
| Saída | Conta-giros painel | AUX7 | Painel Gol | 0.5 | Verde/Branco | — | Saída configurável | 🟩 |

---

## 🔧 Observações gerais

- Todas as conexões devem ser **crimpadas**, nunca soldadas.  
- O chicote deve ser **protegido com malha trançada** e fitas antiabrasivas.  
- Todos os sensores e atuadores devem ter **GND independente do bloco** (retorno direto à ECU).  
- Evitar loops de fio >30 cm sem fixação.  
- A pinagem completa foi projetada para suportar upgrades até a Fase ⚫ Turbo.

---

_Conteúdo do rodapé disponível em [rodape.md](rodape.md)._
