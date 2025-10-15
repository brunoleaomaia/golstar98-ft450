---
layout: default
title: Chicote e Pinagem
nav_order: 3
---

# Chicote e Pinagem
{: .no_toc }
Descrições e pinagem completa do chicote principal do projeto **GolStar98 FT450**, diagrama funcional, pigtails por fase de ativação, relés e fusíveis,  contemplando todas as fases de evolução (aspirada original → turbo).

---
## Nesta Página
{: .no_toc .text-delta}

1. TOC
{:toc}

---

## Pinagem Completa

Abaixo está a pinagem completa do chicote principal planejado para o projeto **GolStar98  FT450**, contemplando todas as fases de evolução (aspirada original → turbo).
{% capture tabela_pinagem %}
{% include_relative tabelas/pinagem-completa.md %}
{% endcapture %}
{{ tabela_pinagem | markdownify }}

{: .new-title .fs-2 }
> Recomendações
> - Todas as conexões devem ser **crimpadas**, nunca soldadas.  
> - O chicote deve ser **protegido com malha trançada** e fitas antiabrasivas.  
> - Todos os sensores e atuadores devem ter **GND independente do bloco** (retorno direto à ECU).  
> - Evitar loops de fio >30 cm sem fixação.  
> - A pinagem completa foi projetada para suportar upgrades até a fase {{ site.fases.f5 }}Turbo.

---

## Diagrama Funcional
Este diagrama resume o fluxo funcional entre sensores, a ECU FuelTech FT450 e os atuadores do motor, organizando os sinais por fase de evolução do projeto.

{% capture tabela_funcional %}
{% include_relative tabelas/diagrama-funcional.md %}
{% endcapture %}
{{ tabela_funcional | markdownify }}

{: .note-title .fs-2 }
> Lógica de Processamento
> 1. **Entradas Analógicas** (TPS, IAT, ECT, Pressões) → definem as condições de operação do motor.  
> 2. **Entradas Digitais** (Hall, AC Request, DH) → controlam modos auxiliares e marcha-lenta.  
> 3. **Processamento Interno** → a FT450 aplica correções, compensações e limites definidos.  
> 4. **Saídas Digitais/PWM** → acionam atuadores, relés e ventiladores conforme a fase ativa.  

{: .new-title .fs-2 }
> Recomendações
>- Realizar testes elétricos e de continuidade antes de cada nova fase.  
>- Manter logs de calibração, mapas e versões de firmware.  
>- Revisar terminais e conectores a cada atualização física.  
>- Utilizar apenas sensores homologados pela FuelTech ou de padrão equivalente.  

{: .highlight-title .fs-2 }
> Observações
> - A FT450 opera em malha fechada via **Wideband Nano 2 (CAN)** para AFR.  
> - Todos os sensores devem ser calibrados no **FTManager** antes do primeiro start.  
> - A ECU possui entradas e saídas livres suficientes para expansão até a Fase {{site.fases.f5}}Turbo.  

---

## Pigtails por Fase/Ativação

{% capture tabela_pigtails_fases %}
{% include_relative tabelas/pigtails-fases.md %}
{% endcapture %}
{{ tabela_pigtails_fases | markdownify }}

{: .new-title .fs-2 }
> Observações
> - Todos os pigtails acima devem ser incluídos **desde a montagem inicial do chicote**.  
> - Pigtails pré-fiação devem ser **isolados e identificados** com etiqueta termoencolhível.  
> - Recomenda-se usar **malha trançada** para agrupamento por sistema (sensores, atuadores, potência).  
> - A expansão até a Fase {{site.fases.f5}} Turbo pode ser feita sem refazer o chicote principal.  

---

## Relés e Fusíveis

{% capture tabela_reles_fusiveis %}
{% include_relative tabelas/reles-fusiveis.md %}
{% endcapture %}
{{ tabela_reles_fusiveis | markdownify }}

{: .new-title .fs-2 }
> Recomendações
> - Todos os relés devem ser do tipo **automotivo selado 5 pinos (SPDT)**.  
> - Fusíveis de palheta padrão **ATO/Mini** com suporte individual identificado.  
> - Instalar **caixa de relés e fusíveis no cofre**, com identificação gravada.  
> - Relés de alta corrente (bomba, ventoinhas) devem ter fios **≥ 2,5 mm²**.  
> - Usar diodos de **flyback** nas cargas indutivas (ventoinhas e solenóides).

---

[Roadmap de Evolução](roadmap){: .btn .mb-4 .mb-md-0 .mr-2 }
[Sensores e Atuadores](sensores-atuadores){: .btn .btn-primary .mb-4 .mb-md-0 .mr-2 }

---


{% include_relative rodape.md %}
