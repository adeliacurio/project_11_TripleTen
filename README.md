# project_11_TripleTen
Advanced Event Analytics and A/A/B Testing for a startup's conversion funnel. Used Python and Bonferroni Correction to ensure statistical significance in visual design changes.

---

# Validação Estatística: Experimento A/A/B e Funil de Eventos 👋

## 📋 Descrição do Projeto
Neste projeto de alto rigor técnico, analisei o comportamento dos usuários de um aplicativo de produtos alimentícios. O desafio foi investigar se a alteração das fontes em todo o aplicativo impactaria a jornada de compra, utilizando um experimento A/A/B para garantir que os resultados fossem estatisticamente significativos e não fruto de oscilações casuais.

## 🎯 Objetivos Estratégicos
* Mapear o **Funil de Vendas**, identificando em qual etapa os usuários mais abandonam o app.
* Realizar um **Teste A/A** para validar a integridade da divisão dos grupos e a precisão da ferramenta de teste.
* Executar um **Teste A/B** para comparar a versão original com a nova proposta visual.
* Aplicar a **Correção de Bonferroni** para ajustar os níveis de significância em múltiplos testes.

## 🛠️ Tecnologias e Ferramentas
* **Linguagem:** Python.
* **Bibliotecas:** Pandas (processamento de logs), Matplotlib/Seaborn (funis e distribuições) e Scipy (testes z e p-values).
* **Técnicas:** Análise de Eventos, Funil de Conversão, Testes de Hipóteses e Correção de Bonferroni.

## 📉 Metodologia e Insights
1.  **Análise do Funil:** Identifiquei que a maior perda de usuários ocorre logo na transição da *Main Screen* para a *Offers Screen*, sugerindo oportunidades de melhoria na navegação inicial.
2.  **Preparação dos Logs:** Processamento de dados de eventos (MainScreenAppear, OffersScreenAppear, CartScreenAppear, PaymentScreenSuccessful).
3.  **Rigor no Experimento:** Comparei dois grupos de controle (A1 e A2) entre si para confirmar que a divisão era justa (Teste A/A) antes de compará-los com o grupo de teste (B).
4.  **Múltiplos Testes:** Realizei 16 testes de hipóteses, aplicando a correção de Bonferroni para manter o nível de confiança global e evitar a aceitação de falsas descobertas.

## ✅ Resultados
* **Conclusão de Design:** O teste demonstrou que a mudança de fontes não afetou negativamente a conversão, permitindo que a equipe de design tomasse decisões estéticas com segurança.
* **Diagnóstico de Conversão:** Apenas 47,7% dos usuários que abrem o app chegam a concluir um pagamento, revelando um gargalo crítico no funil de vendas.
* **Cientificidade:** A análise comprovou que, apesar da mudança visual ser segura, o foco da empresa deve ser na retenção entre a página principal e a de ofertas.

---

### 💡 Como utilizar este repositório
1. O notebook segue uma estrutura científica: EDA -> Análise de Funil -> Testes Estatísticos.
2. Os dados de logs estão processados para facilitar a replicação dos testes z.
