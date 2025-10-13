---
layout: default
title: Relés e Fusíveis
nav_order: 7
---

# ⚡ Relés e Fusíveis – GolStar98 FT450

Tabela de relés e fusíveis do sistema, considerando alimentação separada entre ECU, atuadores e periféricos.

---

## 🔋 Tabela técnica

| Circuito | Relé (A) | Fusível (A) | Alimentação | Saída | Observações | Fase |
|-----------|-----------|--------------|-------------|--------|--------------|------|
| Main ECU | 30 A | 10 A | Pós-chave | FT450 + sensores | Alimenta ECU e sensores | 🟩 |
| Bomba Combustível | 40 A | 20 A | 12 V direto | Bomba tanque | Relé dedicado com fio 2,5 mm² | 🟥 |
| Fan 1 | 40 A | 30 A | 12 V direto | Ventoinha baixa | Estágio 1 controlado pela ECU | 🟦 |
| Fan 2 | 40 A | 30 A | 12 V direto | Ventoinha alta | Estágio 2 controlado pela ECU | 🟦 |
| AC Clutch | 30 A | 15 A | 12 V direto | Compressor A/C | Controlado via AUX4 (FT450) | 🟦 |
| Ignição / Periféricos | 30 A | 15 A | Pós-chave | Bobinas / Wideband | Relé opcional fase 3 → turbo | 🟧 |

---

## ⚙️ Recomendações
- Todos os relés devem ser do tipo **automotivo selado 5 pinos (SPDT)**.  
- Fusíveis de palheta padrão **ATO/Mini** com suporte individual identificado.  
- Instalar **caixa de relés e fusíveis no cofre**, com identificação gravada.  
- Relés de alta corrente (bomba, ventoinhas) devem ter fios **≥ 2,5 mm²**.  
- Usar diodos de **flyback** nas cargas indutivas (ventoinhas e solenóides).

---

_Conteúdo do rodapé disponível em [rodape.md](rodape.md)._
