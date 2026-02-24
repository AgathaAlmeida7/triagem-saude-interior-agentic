🏥 Sistema Agentic de Triagem de Saúde para Áreas Rurais e de Baixo Recurso


📌 Visão Geral

Este projeto implementa um sistema de triagem de saúde baseado em agentes (agentic) utilizando regras estruturadas para classificar o nível de risco de pacientes em ambientes rurais e de baixo recurso.

O sistema avalia entradas clínicas estruturadas como:

Idade

Temperatura corporal

Sintomas

Doenças crônicas

Duração dos sintomas

Com base nesses fatores, o agente calcula um score de risco, classifica o nível de urgência e recomenda ações apropriadas.


🌍 Problema

Em áreas rurais e regiões com acesso limitado à saúde, a avaliação médica imediata nem sempre é possível. Muitos pacientes atrasam a busca por atendimento devido a:

Longas distâncias até hospitais

Falta de transporte

Superlotação de unidades de saúde

Escassez de profissionais

Esses atrasos podem levar a complicações evitáveis, especialmente em idosos e pacientes com doenças crônicas.

Existe a necessidade de um sistema leve, explicável e capaz de funcionar mesmo com baixa conectividade para auxiliar na identificação precoce de casos de maior risco.


🧠 Arquitetura da Solução

O sistema foi desenvolvido de forma modular, garantindo clareza, organização e possibilidade de expansão futura.

Componentes principais:

Modelo de Paciente (entrada estruturada de dados)

Motor de Pontuação de Risco

Módulo de Classificação de Risco

Gerador de Recomendações

Sistema de Registro de Decisões (log)

Essa arquitetura garante:

Transparência

Rastreabilidade

Explicabilidade

Facilidade de manutenção


⚙️ Como Funciona

O agente realiza as seguintes etapas:

Atribui pesos para fatores clínicos relevantes

Avalia combinações de risco (idade + sintomas + comorbidades)

Calcula um score final

Classifica o paciente em níveis de risco:

Baixo

Moderado

Alto

Crítico

Gera recomendação apropriada

Registra a decisão com data e justificativa

O sistema mantém histórico estruturado das decisões, permitindo auditoria e rastreabilidade.


📊 Simulação e Resultados

O sistema foi testado com múltiplos perfis sintéticos de pacientes.

A análise demonstrou que:

Pacientes idosos com sintomas respiratórios e comorbidades tendem a ser classificados como alto ou crítico.

Casos leves são corretamente classificados como baixo ou moderado.

O sistema apresenta comportamento consistente e previsível.

Isso demonstra que o mecanismo baseado em regras é sensível a cenários clínicos multifatoriais.


🚀 Melhorias Futuras

Possíveis evoluções do projeto incluem:

Integração com modelos de linguagem (LLMs)

Integração com bases de dados clínicas reais

Interface mobile para uso comunitário

Deploy offline para regiões sem internet

Dashboard visual para profissionais de saúde


🛠 Tecnologias Utilizadas

Python

Pandas

Lógica baseada em regras

Jupyter Notebook (Kaggle + Colab)

Git e GitHub para versionamento


👩‍💻 Autora

Agatha Almeida

