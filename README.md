# 🚗 GolStar98 – Projeto FT450

Documentação técnica e evolução do sistema eletrônico do **Volkswagen Gol G2 1.6 MI (1998)** com **ECU FuelTech FT450**.

Este repositório centraliza toda a parte elétrica, lógica e de configuração do projeto, desde a fase **aspirada original** até o estágio **turbo-ready**, com diagramas, tabelas, pigtails e roadmap de evolução.

---

## 🌐 Documentação Online

Acesse a documentação técnica completa no GitHub Pages:  
🔗 **[https://brunoleaomaia.github.io/golstar98-ft450/](https://brunoleaomaia.github.io/golstar98-ft450/)**

Ou, navegue diretamente pelos arquivos Markdown em [`/docs`](docs/).

---

## 🧭 Estrutura do Projeto

| Pasta / Arquivo | Função |
|------------------|--------|
| `/docs/` | Contém toda a documentação técnica em Markdown (usada pelo GitHub Pages). |
| `/docs/index.md` | Página inicial da documentação (carregada automaticamente no Pages). |
| `/docs/indice.md` | Sumário completo e hierárquico de todos os tópicos. |
| `_config.yml` | Configuração do site (tema Just the Docs). |
| `SUMMARY.md` | Sumário auxiliar para leitura dentro do GitHub. |

---

## ⚙️ Tecnologias utilizadas

- **FuelTech FT450** – ECU principal de gerenciamento eletrônico.  
- **Wideband Nano 2 (CAN)** – Sensor lambda de banda larga com comunicação digital.  
- **Just the Docs** – Tema técnico para o GitHub Pages.  
- **Markdown (.md)** – Linguagem de documentação técnica estruturada.  

---

## 🧱 Organização das Fases

| Fase | Ícone | Nome | Descrição |
|------|-------|------|-----------|
| 🟩 | F1 | Base aspirada | Instalação inicial da ECU e wideband CAN. |
| 🟦 | F2 | Sensores e proteções | Inclusão de sensores auxiliares e failsafes. |
| 🟧 | F3 | Ignição moderna | Conversão para bobinas individuais Gol G6. |
| 🟥 | F4 | Alimentação definitiva | Atualização da bomba e regulador de combustível. |
| ⚫ | F5 | Turbo | Instalação do kit turbo e controle PWM de boost. |

---

## 💡 Como visualizar o site localmente

Se quiser visualizar o site Just the Docs localmente antes de publicar:

```bash
# Instalar Jekyll e dependências
gem install bundler jekyll

# Instalar dependências
bundle install

# Rodar localmente
bundle exec jekyll serve --source docs --livereload
````

Depois, acesse:
👉 [http://localhost:4000](http://localhost:4000)

*(Essa etapa é opcional; o GitHub Pages renderiza automaticamente o conteúdo de `/docs`.)*

---

## 🤝 Contribuindo

* Sugestões e correções são bem-vindas via **Pull Request**.
* Use o padrão Markdown simples (sem HTML customizado).
* Mantenha o rodapé padrão referenciando [rodape.md](docs/rodape.md).
* Atualize o [changelog](docs/changelog.md) ao realizar alterações significativas.

---

## 📄 Licença

Conteúdo técnico sob licença livre para fins educacionais e documentais.
Marcas e nomes FuelTech pertencem aos seus respectivos proprietários.

---

*Conteúdo técnico detalhado disponível em [/docs](docs/) e publicado via GitHub Pages.*