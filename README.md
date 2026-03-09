# 🏗️ Comparador de Plantas CAD (Análise de Aditivo)

Este projeto é uma ferramenta web estática e segura projetada para realizar a sobreposição e comparação visual entre duas plantas de imóveis (original vs. aditivo). Ela foi desenvolvida para identificar alterações milimétricas em projetos de apartamentos, utilizando calibração por pontos para ignorar variações de escala em arquivos PDF/Imagens.

## 📋 Contexto do Projeto (Unidade 5706)

O sistema foi configurado para analisar o impacto do termo aditivo do empreendimento **Jardim dos Ipês**. A análise foca na distinção entre:

**Área Útil:** Espaço real interno ("vassoura") onde houve uma redução estimada de **0,56 m²** devido ao reposicionamento de paredes.

**Área Privativa:** Metragem legal de contrato (**55,96 m²**) que permanece inalterada no aditivo para fins de registro em cartório.


## 🚀 Funcionalidades Principais

* **🔒 Privacidade Total:** O processamento é 100% local via `FileReader` API; nenhuma imagem é enviada para servidores externos.
* **🎯 Calibração por 2 Pontos:** Sistema de alinhamento estilo CAD que permite ignorar margens brancas e textos, cravando a escala exata entre as duas imagens.
* **🔬 Modo Raio-X:** Utiliza `mix-blend-mode: difference` para destacar em cores neon apenas o que mudou entre as plantas.
* **⏱️ Modo Pisca-Pisca:** Alterna rapidamente a visibilidade da sobreposição para detectar mudanças sutis através do movimento.
* **📊 Laudo Técnico Integrado:** Tabela comparativa detalhando perdas e ganhos em centímetros por cômodo.

## 🛠️ Tecnologias Utilizadas

* HTML5 / CSS3 (Flexbox e CSS Filters)
* JavaScript Vanilla (API Canvas e DOM)
* Nenhum framework externo (dependência zero)

## 📖 Como Usar

1. **Upload:** Selecione a imagem da planta original (Azul) e a imagem da nova planta (Vermelha).
2. **Calibração:** * Clique em "Calibrar Alinhamento".
* Marque dois pontos fixos na planta azul (ex: quinas externas).
* Marque os mesmos dois pontos na planta vermelha.


3. **Análise:** Utilize os sliders de transparência ou os botões de Raio-X e Pisca-Pisca para inspecionar as divergências.
4. **Consulta:** Verifique a tabela de laudo técnico no rodapé para os valores exatos de diferença.

## ⚠️ Isenção de Responsabilidade (Disclaimer)

O sistema pode cometer erros. As sobreposições e cálculos são representações visuais para facilitar o entendimento e podem conter imprecisões decorrentes da qualidade das imagens enviadas ou do alinhamento manual. Sempre consulte a planta técnica oficial e profissionais qualificados para decisões de projeto ou marcenaria.

---

### 📦 Como publicar?

Para deixar este repositório online:

1. Renomeie seu arquivo principal para `index.html`.
2. No GitHub, vá em **Settings > Pages**.
3. Selecione a branch `main` e salve.

---

**Desenvolvido para análise técnica de aditivos imobiliários.**

---

Gostaria que eu fizesse alguma alteração específica em algum tópico do README?
