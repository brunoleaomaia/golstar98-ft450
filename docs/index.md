---
layout: home
title: Home
nav_order: 1
description: Página inicial da documentação técnica do GolStar98 com ECU FuelTech FT450
---

# Bem-vindo

Bem-vindo à documentação técnica do projeto **GolStar98 FT450**, um projeto de modernização do sistema de gerenciamento eletrônico do Volkswagen Gol G2 1.6 MI (1998) utilizando a ECU FuelTech FT450.

O objetivo é documentar de forma detalhada a evolução elétrica e lógica do veículo — desde o sistema `aspirado original` até o estágio `turbo-ready`, mantendo compatibilidade total entre todas as fases.

[Roadmap de Evolução](roadamap){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }
[Glossário](glossario){: .btn .fs-5 .mb-4 .mb-md-0 }

---

### Estrutura das Fases

{% capture tabela_fases %}
{% include_relative tabelas/fases-do-projeto.md %}
{% endcapture %}
{{ tabela_fases | markdownify }}

---

## 🔍 Como usar esta documentação

- Navegue pelas seções através do **menu lateral** ou pelos links acima.  
- Use a **barra de busca (🔍)** no topo do site para localizar termos como *MAP*, *IAT*, *PWM*, *pigtail*, etc.  
- Cada página contém tabelas e esquemas compatíveis com leitura no GitHub e no navegador.  
- O conteúdo técnico é **versão 1.0 (Outubro/2025)** e será atualizado conforme o avanço do projeto.

---

## 🧱 Organização do Repositório

<pre>
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
</pre>

{% include_relative rodape.md %}
