# GolStar98 FT450

Bem-vindo à documentação técnica do projeto **GolStar98 FT450**, um projeto de modernização do sistema de gerenciamento eletrônico do Volkswagen Gol G2 1.6 MI (1998) utilizando a ECU FuelTech FT450.

O objetivo é documentar de forma detalhada a evolução elétrica e lógica do veículo, desde o sistema `aspirado original` até a fase `turbo`, mantendo compatibilidade total entre todas as fases.

| Fase | Nome | Descrição |
|-------|------|---------------------|
| Fase 1 | Base Aspirada | Instalação da FT450 e Wideband CAN. Mantém injeção, bomba e ignição originais (distribuidor). Validação inicial e funcionamento básico. |
| Fase 2 | Sensores e Proteções | Adição de sensores auxiliares (IAT, ECT, pressão de óleo e combustível). Ativação de failsafes e compensações térmicas. Idle-up do A/C e direção hidráulica. |
| Fase 3 | Ignição Moderna | Instalação da roda fônica 60-2 e bobinas individuais Gol G6. Remoção do distribuidor e ativação da ignição sequencial COP. |
| Fase 4 | Alimentação Definitiva | Substituição da bomba de combustível por 255 LPH e revisão de regulador/retorno. Validação de pressão de linha e delta combustível-MAP. |
| Fase 5 | Turbo | Instalação de kit turbo, solenoide PWM e MAP 3–4 bar. Ajuste de AFR e avanço por pressão, com proteções em malha fechada. |

---

## Documentação Online
Acesse a documentação técnica completa no GitHub Pages:  

**[https://brunoleaomaia.github.io/golstar98-ft450/](https://brunoleaomaia.github.io/golstar98-ft450/)**

---

## Documentação Local
Se quiser visualizar o site Just the Docs localmente antes de publicar:

```bash
# Instalar Jekyll e dependências
gem install bundler jekyll

# Instalar dependências
bundle install

# Rodar localmente
bundle exec jekyll serve --source docs --livereload
````

---

## Contribuindo

- Sugestões e correções são bem-vindas via **Pull Request**.
- Use o padrão Markdown simples (sem HTML customizado).
- Atualize o [changelog](docs/changelog.md) ao realizar alterações significativas.

---

## Links Externos

- [@GolStar98](https://www.instagram.com/golstar98/) - Instagram do Gol Star 1998 do Projeto.
- [FuelTech](https://www.fueltech.com.br/) — Site da FuelTech.
- [FT Education](https://fteducation.com.br/) — Site da FT Education.
- [Manual FT450](https://ftmanager.fueltech.com.br/downloads/manual/Portugues/FT450_FT550_FT600.pdf) — Manual em Português da ECU FuelTech FT450.