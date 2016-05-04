---
published: true
permalink: /
layout: slate
filename: README.md
title: Kit para Dados Abertos
desc: O kit é um conjunto de documentos que descreve o processo, métodos e técnicas para a implementação de uma política de dados abertos no âmbito de uma instituição.
---

O kit é um conjunto de documentos que descreve o processo, métodos e técnicas
para a implementação de uma política de dados abertos no âmbito de uma
instituição. Ele é primariamente focado em órgãos e entidades da administração
pública federal, para a execução de sua [política de dados
abertos](http://wiki.gtinda.ibge.gov.br/Politica-de-Dados-Abertos.ashx) e para
a criação e implementação de seus respectivos [Planos de Dados
Abertos](Glossário#plano-de-dados-abertos) (PDAs), mas procura ser geral o
suficiente para que possa ser aproveitado em outras instituições.

## Contexto e objetivo

A publicação de dados abertos é a nova tendência presente na estratégia de governo digital do Brasil e de diversos países do mundo. Seu compromisso foi assumido pela presidente Dilma no momento da assinatura da [declaração](http://www.cgu.gov.br/governoaberto/a-ogp/o_que_e_Governo_Aberto.html) da [Parceria para Governo Aberto](http://www.cgu.gov.br/governoaberto/a-ogp/iniciativa.asp) ([OGP](http://www.opengovpartnership.org/)) e pelos diversos órgãos do executivo nos dois [Planos de Ação da Parceria](http://www.cgu.gov.br/governoaberto/no_Brasil/plano-brasileiro/index.html).

A recomendação da Presidência da República e do Ministério do Planejamento, Orçamento e Gestão é que os gestores públicos tratem a pauta criando Planos de Dados Abertos em suas organizações.

As organizações que desenvolvem Planos de Dados Abertos precisam de orientação, métodos e técnicas para sua criação e implementação. A proposta do Kit é fornecer os insumos necessários para esses momentos e servir como guia para referência futura.


## Definições e conceitos

1. [O que são dados abertos](http://dados.gov.br/dados-abertos/) - Definições básicas sobre características dos dados abertos;
2. [Vantagens de publicar dados abertos](vantagens-dados-abertos);
3. A [Parceria para Governo Aberto](http://www.governoaberto.cgu.gov.br/a-ogp/o-que-e-a-iniciativa) e a [Estratégia de Governança Digital](http://www.governoeletronico.gov.br/estrategia-de-governanca-digital-egd/) - políticas relacionadas a dados abertos;
4. O [Portal Brasileiro de Dados Abertos](http://dados.gov.br/sobre/) - Sobre o catálogo de dados;
5. O que é a [Infraestrutura Nacional de Dados Abertos - INDA](http://dados.gov.br/instrucao-normativa-da-inda/) e a [Política de dados abertos](http://wiki.gtinda.ibge.gov.br/Politica-de-Dados-Abertos.ashx) do executivo federal;
6. [Glossário](Glossário) dos termos utilizados neste kit.

## Guia para implementação de um Plano de Dados Abertos

A criação e implementação de um Plano de Dados Abertos para uma instituição pode ser organizado em fluxos de atividade como no diagrama a seguir:

[<img alt="Diagrama do processo sistêmico de um plano de dados abertos" src="https://raw.githubusercontent.com/dadosgovbr/kit/master/public/img/Processo%20Sist%C3%AAmico%20de%20um%20PDA.png">](Processo-sist%C3%AAmico)

Esse processo pode ser visto com maiores detalhes no documento [Processo sistêmico de um Plano de Dados Abertos - PDA](Processo-sist%C3%AAmico).

Os seguintes subprocessos estão detalhados:

* [Elaboração de um PDA](Elabora%C3%A7%C3%A3o-do-PDA)
* [Execução de um PDA](Execu%C3%A7%C3%A3o-do-PDA)
  * [Abertura de bases de dados](Abertura-de-dados)


## Ferramentas

Esta seção é uma lista exemplificativa, e não exaustiva, de ferramentas úteis
para [projetos de abertura de dados](Abertura-de-dados). É importante ter em
mente que o rol de ferramentas para lidar com dados está em constante mutação.
São criadas novas ferramentas e outras, mesmo que muito utilizadas,
[são descontinuadas](http://techtohuman.com/5_in_5_teaching/#tool-volatility).
Por isso, é altamente recomendável não se basear apenas em listas e
levantamentos de ferramentas, mas sempre fazer novas pesquisas visando
encontrar a ferramenta mais adequada para o problema que se pretende tratar.

Todas as ferramentas aqui listadas são livres, criadas por comunidades de
[software livre](Glossário#software-livre), e podem ser utilizadas pelos
órgãos governamentais sem restrição. Em geral, são soluções para extração,
manipulação e preparação dos dados para sua publicação na Internet. A lista é
baseada no [_Project Open Data_](http://project-open-data.github.io/#tools) e
[_ODI open data tech
review_](https://github.com/dadosgovbr/open-data-tech-review/wiki). Contudo,
está restrita a ferramentas que podem ser utilizadas sem a necessidade de
conhecimentos de programação.

### Criação de APIs de dados abertos

* [CSV to API](https://github.com/project-open-data/csv-to-api) - Dinamicamente gera APIs Restful de arquivos CSVs estáticos 
* [sandman](https://github.com/jeffknupp/sandman) - Cria API Restful automaticamente a partir de conexão com bancos de dados relacionais

### Conversão de dados

* [JSON-to-CSV Converter](http://konklone.io/json/) - Conversor manual e online de arquivos JSON para visualizar como planilha e baixá-la no formato CSV;
* [dat](https://github.com/maxogden/dat) - Ferramenta para conversão e transformação de dados em linha de comando;
* [csvkit](http://csvkit.readthedocs.org/en/0.8.0/) - Transformações e tratamento de arquivos CSV;
* [ESRI2Open](http://github.com/project-open-data/esri2open) - Ferramenta que converte dados espaciais e não-espaciais do software; proprietário ESRI em arquivos de dados abertos, CSV, JSON, ou GeoJSON.

### Higienização de dados

* [Open Refine](http://openrefine.org/) - Limpeza e transformação de dados, unificação de registros duplicados, etc.

## Guias de referência

Os guias abaixo servem como referência para a construção de uma política ou iniciativa de dados abertos (por exemplo, em um estado ou município).

* Guia de Dados Abertos ([_Open Data Handbook_](http://opendatahandbook.org/pt_BR/)) - da [_Open Knowledge_](https://okfn.org/);
* [Manual dos dados abertos: governo](http://www.w3c.br/pub/Materiais/PublicacoesW3C/Manual_Dados_Abertos_WEB.pdf) - do [W3C Brasil](http://www.w3c.br);
* [Open Government Data Toolkit](http://opendatatoolkit.worldbank.org/en/index.html) - do Banco Mundial.

## PDAs publicados

Para informações sobre quais instituições do poder executivo federal já publicaram planos de dados abertos, consulte a [wiki da INDA](http://wiki.gtinda.ibge.gov.br/Plano-de-Dados-Abertos.ashx).

## Legislação relacionada

* [Lei de acesso à informação](http://www.lexml.gov.br/urn/urn:lex:br:federal:lei:2011-11-18;12527) - Dispõe sobre o acesso às informações públicas, inclusive pela internet
* [Decreto nº 7724](http://www.lexml.gov.br/urn/urn:lex:br:federal:decreto:2012-05-16;7724) - Regulamenta a Lei de acesso à informação no âmbito do poder executivo federal
* [Instrução Normativa da INDA](http://dados.gov.br/instrucao-normativa-da-inda/) - Institui a Infraestrutura Nacional de Dados abertos e seu funcionamento
* [Decreto de 15 de setembro de 2011](http://www.lexml.gov.br/urn/urn:lex:br:federal:decreto:2011-09-15;seq-sf-0) - Institui o CIGA e o Plano Nacional de Governo Aberto
* [Decreto 8.638, de 15 de janeiro de 2016](http://www.lexml.gov.br/urn/urn:lex:br:federal:decreto:2016-01-15;8638) - Institui a Política de Governança Digital

