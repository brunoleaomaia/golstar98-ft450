---
layout: home
title: GolStar98 – Projeto FT450
# Index page
---

# GolStar98 – Projeto FT450

Bem-vindo à documentação técnica do **GolStar98**, um projeto de modernização do sistema de gerenciamento eletrônico do **Volkswagen Gol G2 1.6 MI (1998)** utilizando a **ECU FuelTech FT450**.

O objetivo é documentar de forma detalhada a evolução elétrica e lógica do veículo — desde o sistema **aspirado original** até o estágio **turbo-ready**, mantendo compatibilidade total entre todas as fases.

---

## 🧭 Navegação principal

- 📖 [Índice de Documentação](indice)  
  Sumário completo com links para todos os tópicos técnicos do projeto.

- 🧩 [Roadmap de Evolução](roadmap)  
  Linha do tempo com as cinco fases do sistema (🟩 Base aspirada → ⚫ Turbo).

---

## ⚙️ Estrutura das Fases
[tabela-de-fases.md](tabela-de-fases.md)

---

## 🔍 Como usar esta documentação

- Navegue pelas seções através do **menu lateral** ou pelos links acima.  
- Use a **barra de busca (🔍)** no topo do site para localizar termos como *MAP*, *IAT*, *PWM*, *pigtail*, etc.  
- Cada página contém tabelas e esquemas compatíveis com leitura no GitHub e no navegador.  
- O conteúdo técnico é **versão 1.0 (Outubro/2025)** e será atualizado conforme o avanço do projeto.

---

## 🧱 Organização do Repositório

/docs/
├─ index.md → Esta página inicial
├─ indice.md → Sumário completo dos tópicos
├─ roadmap.md → Roadmap de evolução
├─ chicote-pinagem.md → Pinagem completa da ECU e chicote
├─ pigtails.md → Pigtails e subchicotes
├─ pigtails-fases.md → Pigtails por fase
├─ sensores.md → Sensores e características elétricas
├─ atuadores.md → Atuadores e saídas configuráveis
├─ diagrama-logico.md → Lógica interna da ECU
├─ diagrama-funcional-sensores-ecu-atuadores.md
├─ reles-fusiveis.md → Tabela de relés e fusíveis
├─ checklist.md → Verificações e testes
├─ changelog.md → Registro de alterações
├─ glossario.md → Glossário técnico
└─ rodape.md → Rodapé padrão compartilhado

---

{% include_relative rodape.md %}
