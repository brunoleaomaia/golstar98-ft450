# GolStar98 – Projeto FT450

Documentação técnica completa do projeto de integração da **FuelTech FT450** no **Volkswagen Gol G2 1.6 MI (1998)**, denominado **GolStar98**.

O objetivo deste repositório é centralizar todas as informações elétricas, lógicas e de hardware necessárias para o gerenciamento eletrônico completo do motor, evoluindo de forma modular da configuração **aspirada original** até o estágio **turbo-ready**.

---

## ⚙️ Estrutura do projeto

A documentação está dividida em tópicos técnicos individuais:

- [Índice](indice.md)
- [Checklist de Comissionamento](checklist.md)
- [Chicote e Pinagem](chicote-pinagem.md)
- [Relés e Fusíveis](reles-fusiveis.md)
- [Diagrama Funcional (Sensores → ECU → Atuadores)](diagrama-funcional-sensores-ecu-atuadores.md)
- [Diagrama Lógico](diagrama-logico.md)
- [Sensores](sensores.md)
- [Atuadores](atuadores.md)
- [Pigtails e Subchicotes](pigtails.md)
- [Pigtails por Fase](pigtails-fases.md)
- [Roadmap de Evolução](roadmap.md)
- [Glossário Técnico](glossario.md)
- [Rodapé Padrão](rodape.md)

---

## 🧭 Filosofia de evolução

O projeto foi estruturado em **cinco fases** evolutivas:

| Fase | Ícone | Descrição |
|------|-------|-----------|
| 🟩 1 | Base aspirada | Instalação da FT450 e Wideband CAN com sistema original. |
| 🟦 2 | Sensores e proteções | Inclusão de sensores auxiliares e proteções. |
| 🟧 3 | Ignição moderna | Substituição do distribuidor por roda fônica e bobinas G6. |
| 🟥 4 | Alimentação definitiva | Atualização da bomba e regulador de combustível. |
| ⚫ 5 | Turbo | Adição de turbo, solenoide PWM e MAP 3-4 bar. |

---

## 📦 Estrutura no GitHub

Todos os arquivos estão em formato **Markdown puro**, compatíveis com **GitHub Pages**.  
Cada seção pode ser visualizada diretamente no navegador ou convertida em PDF se necessário.

---

_Conteúdo do rodapé disponível em [rodape.md](rodape.md)._
