📚 Caderno Temático - Power BI e DAX Avançado com NotebookLM
📖 Sobre o Projeto

Este projeto foi desenvolvido como parte do desafio da DIO utilizando o NotebookLM como ferramenta de aprendizagem ativa.

O objetivo foi explorar conceitos avançados de Power BI e DAX por meio da curadoria de fontes confiáveis, utilização de Inteligência Artificial para geração de conhecimento e construção de um material de consulta rápida para futuras revisões.

🎯 Objetivos de Estudo
Compreender conceitos avançados da linguagem DAX.
Aprimorar a criação de indicadores e KPIs.
Entender o funcionamento do contexto de filtro e contexto de linha.
Aprender boas práticas de modelagem de dados.
Melhorar a performance de dashboards no Power BI.
Utilizar IA como apoio na construção do conhecimento.
📚 Curadoria de Fontes

As seguintes fontes foram utilizadas como base para o estudo e importadas no NotebookLM:

Fonte 1

Documentação Oficial DAX

https://learn.microsoft.com/pt-br/dax/

Fonte 2

Documentação Oficial Power BI

https://learn.microsoft.com/pt-br/power-bi/

Fonte 3

Boas práticas para modelagem de dados

https://learn.microsoft.com/pt-br/power-bi/guidance/star-schema

Fonte 4

Otimização e Performance no Power BI

https://learn.microsoft.com/pt-br/power-bi/guidance/power-bi-optimization

Fonte 5

Guia de Relacionamentos em Modelos Tabulares

https://learn.microsoft.com/pt-br/power-bi/transform-model/desktop-relationships-understand

🤖 Engenharia de Prompts

Durante o estudo foram realizados diversos testes para compreender como a qualidade das perguntas impacta a qualidade das respostas geradas pela IA.

Prompt 1

Pergunta:

Explique a diferença entre contexto de linha e contexto de filtro utilizando exemplos práticos em Power BI.

Resumo da Resposta

A IA explicou que o contexto de linha ocorre quando uma expressão é avaliada linha por linha, enquanto o contexto de filtro considera os filtros aplicados ao modelo de dados.

Foi apresentado um exemplo utilizando colunas calculadas e medidas para demonstrar a diferença entre ambos.

Prompt 2

Pergunta:

Quando devo utilizar CALCULATE em vez de FILTER?

Resumo da Resposta

A resposta mostrou que CALCULATE modifica o contexto de filtro de uma expressão e é uma das funções mais importantes do DAX.

Já FILTER é utilizado para criar tabelas filtradas e normalmente é utilizado dentro de outras funções.

Prompt 3

Pergunta:

Quais são os principais erros que causam lentidão em dashboards Power BI?

Resumo da Resposta

Foram destacados:

Uso excessivo de colunas calculadas.
Relacionamentos inadequados.
Falta de modelagem dimensional.
Medidas complexas sem otimização.
Grande volume de dados sem agregações.
Prompt 4

Pergunta:

Crie uma trilha de aprendizagem para me tornar um especialista em Power BI.

Resumo da Resposta

A IA sugeriu uma sequência de estudos:

Modelagem de Dados
DAX Básico
DAX Intermediário
DAX Avançado
Performance
Power BI Service
Governança e Segurança
🩹 Dificuldades Encontradas (Cicatrizes)

Durante os testes realizados no NotebookLM foram observados alguns desafios:

Perguntas muito genéricas geravam respostas superficiais.
Em alguns momentos a IA fornecia explicações teóricas sem exemplos práticos.
Foi necessário adicionar contexto ao prompt para obter respostas mais completas.
Perguntas abertas produziram respostas extensas e menos objetivas.
Melhores resultados foram obtidos utilizando cenários reais do dia a dia em BI.
Exemplo

Prompt genérico:

"Explique DAX."

Resultado:
Resposta ampla e superficial.

Prompt refinado:

"Explique DAX para um Analista de BI que desenvolve indicadores operacionais no Power BI."

Resultado:
Resposta mais direcionada e aplicável ao contexto profissional.

📘 Miniguia de Estudos
O que é DAX?

DAX (Data Analysis Expressions) é a linguagem utilizada no Power BI para criação de medidas, colunas calculadas e tabelas calculadas.

Seu principal objetivo é permitir análises avançadas sobre os dados.

Contexto de Linha

O contexto de linha ocorre quando uma fórmula é avaliada individualmente para cada registro de uma tabela.

Exemplo:

Valor Total = Vendas[Quantidade] * Vendas[Preço]

A operação é executada linha por linha.

Contexto de Filtro

O contexto de filtro é determinado pelos filtros aplicados ao relatório.

Exemplo:

Um gráfico filtrado para o mês de Janeiro recalculará automaticamente os valores considerando apenas esse período.

Função CALCULATE

A função mais importante do DAX.

Permite alterar o contexto de filtro de uma expressão.

Exemplo:

Vendas SP =
CALCULATE(
    SUM(Vendas[Valor]),
    Clientes[Estado] = "SP"
)
Função FILTER

Retorna uma tabela filtrada.

Exemplo:

FILTER(
    Vendas,
    Vendas[Valor] > 1000
)
Boas Práticas de Modelagem
Utilizar modelo estrela.
Evitar relacionamentos desnecessários.
Criar tabelas fato e dimensão.
Utilizar chaves únicas.
Reduzir colunas não utilizadas.
Dicas de Performance
Evitar excesso de colunas calculadas.
Priorizar medidas.
Remover campos desnecessários.
Reduzir cardinalidade.
Utilizar agregações quando possível.
📖 Glossário
Termo	Definição
DAX	Linguagem de expressões do Power BI
KPI	Indicador-chave de desempenho
Medida	Cálculo dinâmico realizado em tempo de consulta
Coluna Calculada	Coluna criada por fórmula DAX
Contexto de Linha	Avaliação linha por linha
Contexto de Filtro	Conjunto de filtros ativos
Modelo Estrela	Estrutura dimensional para análise
Power Query	Ferramenta de transformação de dados
ETL	Extração, Transformação e Carga
Dashboard	Painel visual para monitoramento
🚀 Prompts Reutilizáveis
Aprendizado

Explique o conceito de [TEMA] utilizando exemplos práticos em Power BI.

Comparação

Compare [FUNÇÃO A] e [FUNÇÃO B] apresentando vantagens, limitações e exemplos.

Exercícios

Crie 10 exercícios práticos sobre [TEMA] com gabarito comentado.

Revisão

Faça um resumo executivo sobre [TEMA] destacando os pontos mais importantes.

Especialização

Monte uma trilha de aprendizagem completa para me tornar especialista em [TEMA].

Troubleshooting

Quais são os erros mais comuns relacionados a [TEMA] e como corrigi-los?

🏆 Conclusão

O NotebookLM demonstrou ser uma ferramenta eficiente para aprendizagem ativa, permitindo centralizar conteúdos, realizar pesquisas contextualizadas e acelerar a construção de conhecimento.

A utilização de IA aliada a fontes confiáveis tornou o processo de estudo mais produtivo, facilitando a compreensão de conceitos avançados de Power BI e DAX e contribuindo para o desenvolvimento profissional na área de Business Intelligence.

👨‍💻 Autor

Projeto desenvolvido como parte dos desafios práticos da DIO (Digital Innovation One), com foco na aplicação de Inteligência Artificial como ferramenta de estudo e construção de conhecimento.
