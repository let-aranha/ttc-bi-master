# Título do Trabalho

#### Aluno: [Letícia Aranha](https://github.com/let-aranha)
#### Orientador: [Leonardo Mendonza](https://github.com/leofome8)

---

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".

- [Link para o código](https://github.com/let-aranha/ttc-bi-master). <!-- caso não aplicável, remover esta linha -->

---

### Resumo

Em um cenário em que a concorrência entre mercados está cada mais acirrada, um Serviço de Atendimento ao Cliente de qualidade torna-se diferencial competitivo. Para a VTEX, empresa multinacional brasileira de tecnologia, desenvolvedora da plataforma VTEX Cloud Commerce, esse time de atendimento denominado Customer Excellence, presta suporte especializado sobre os mais diversos temas que envolvem o funcionamento de sua infraestrutura *multitenant*.

Para potencializar a formação de profissionais e contribuir para a curva de aprendizado de novos analistas, tornando o processo de on boarding escalável e mensurável, o presente Trabalho de Conclusão de Curso tem como objetivo apresentar uma Proof of Concept (PoC), ou Prova de Conceito, utilizando técnicas de classificação, com o objetivo fim de prever as classes de saída de chamados de acordo com quatro níveis de complexidade: *“Low”, “Moderate”, “High” e “Very High”.*

O modelo utiliza como base dados estruturados obtidos através da ferramenta Zendesk, canal oficial de comunicação do suporte VTEX. Dentre os dados coletados, é possível encontrar informações referentes ao nível de conhecimento da plataforma do usuário responsável pela abertura do chamado, assim como contexto da organização e funcionamento de seu ecommerce.

Foram realizados alguns tratamentos na base de dados dentro da etapa de Pré-Processamento, incluindo One Hot Encoding, verificação de registro nulos e substituição dos mesmos pela moda, PCA para redução da dimensionalidade da base, técnicas de balanceamento da base, como Under-Sampling e Random Over-Sampling e Under-Sampling com SMOTEENN.

Após os ajustes na base, foram testados quatro modelos de classificação:

**1. Decision Tree**
**2. Random Forest**
**3. SVM**
**4. K Neighbors Classifier**

Todos os quatro modelos acima se mostraram incapazes de prever com exatidão as classes minoritárias, que representam os tickets de maior complexidade. Para aferir o desempenho dos resultados, foram utilizadas métricas como **Acurácia, Kappa** e **F1-Score.**

Por fim, utilizou-se a técnica de **K-Means** e o **Método Elbow** para entender se a divisão de classes utilizada pela empresa apresenta os melhores resultados, ou se existe uma formatação diferenciada de clusters que melhor interpretaria os valores da base.

O trabalho foi desenvolvido utilizando linguagem Python, com o auxílio das bibliotecas de classificação como *DecisionTreeClassifier, RandomForestClassifier, SVC* e *K Neighbors Classifier*, além do método *K-Means*.


---

Matrícula: 191.671.041

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*
