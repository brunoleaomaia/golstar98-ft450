| Circuito | Relé (A) | Fusível (A) | Alimentação | Saída | Observações |
|-----------|-----------|--------------|-------------|--------|--------------|
| {{ site.fases.f1 }} Main ECU | 30 A | 10 A | Pós-chave | FT450 + sensores | Alimenta ECU e sensores |
| {{ site.fases.f1 }} Bomba Combustível | 40 A | 20 A | 12 V direto | Bomba tanque | Relé dedicado com fio 2,5 mm² |
| {{ site.fases.f2 }} Fan 1 | 40 A | 30 A | 12 V direto | Ventoinha baixa | Estágio 1 controlado pela ECU |
| {{ site.fases.f2 }} Fan 2 | 40 A | 30 A | 12 V direto | Ventoinha alta | Estágio 2 controlado pela ECU |
| {{ site.fases.f2 }} AC Clutch | 30 A | 15 A | 12 V direto | Compressor A/C | Controlado via AUX4 (FT450) |
| {{ site.fases.f3 }} Ignição / Periféricos | 30 A | 15 A | Pós-chave | Bobinas / Wideband | Relé opcional fase 3 → turbo |