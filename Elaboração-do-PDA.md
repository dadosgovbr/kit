---
published: true
permalink: /Elaboração-do-PDA/
layout: slate
filename: Elaboração-do-PDA.md
title: Elaboração do PDA - Kit de Dados Abertos
desc: Este documento se dispõe a resumir os principais passos do manual e trazer novas referências.
---

Elaboração do Plano de Dados Abertos
====

O conteúdo que orienta a criação de um PDA está estruturado no
[Manual para elaboração de Plano de Dados Abertos](http://www.planejamento.gov.br/secretarias/upload/Arquivos/governo_aberto/manual_elaboracao_plano_dados_abertos.pdf). 
Este documento se dispõe a resumir os principais passos do manual e trazer
novas referências.

Antes de mergulhar na construção do PDA, há uma etapa anterior muito importante:
Definir quem serão os responsáveis pela iniciativa e reunir as pessoas
relevantes para as atividades em questão. Essas atividades estão estruturadas no
[processo sistêmico]({{ site.baseurl }}Processo-sistêmico),
a leitura do qual sugere-se antes deste processo.

De maneira resumida, o processo de criação do PDA consiste em 4 etapas:

## Organizar Inventário de Dados

Antes de definir quais dados são publicados é imprescindível que a organização faça
um levantamento de quais dados possui. Apesar de ser muito útil, poucos órgãos
públicos tem esse levantamento feito.

Existem algumas formas de fazer esse levantamento, provavelmente a melhor estratégia é uma combinação delas:

* Levantar, junto com os representantes das diversas áreas, quais são os sistemas usados por cada uma
* Fazer uma lista com os dados pedidos pelo SIC
* Caso a manutenção de todos os sistemas seja centralizada em uma única área de TI, obter a lista dos sistemas com a área


## Priorizar os dados que serão abertos

A priorização ocorre porque não vale a pena a organização fazer um esforço para publicar todos os seus dados simultaneamente, o custo é alto e não implica necessariamente na publicação de **dados relevantes para o público**. 

Conforme o [manual para elaboração de PDA](http://www.planejamento.gov.br/secretarias/upload/Arquivos/governo_aberto/manual_elaboracao_plano_dados_abertos.pdf), a etapa de priorização deve considerar esses critérios:

1. O grau de relevância para o cidadão, observando-se especialmente as
   **demandas encaminhadas via solicitações de [acesso à
   informação](http://www.acessoainformacao.gov.br/)**, dentre as quais, as
   realizadas a partir de junho de 2015 e que não contenham informações
   restritas (pessoais ou sigilosas), podem ser consultadas pela [busca de
   pedidos e respostas do sistema
   e-SIC](http://www.acessoainformacao.gov.br/assuntos/busca-de-pedidos-e-respostas).
   Os temas mais procurados também podem ser levantados a partir de
   estatísticas da ouvidoria do órgão, bem como dos setores e dos serviços
   mais procurados em seus sítios eletrônicos. Adicionalmente, a organização
   pode também realizar um encontro com os principais consumidores de seus
   dados (ex: organizações da sociedade civil, ONGs, pesquisadores, outros
   órgãos públicos) para entender aonde concentram-se suas necessidades;
2. Os normativos legais e os compromissos formalmente assumidos pelo órgão, inclusive perante organismos internacionais (ex: [OGP]({{ site.baseurl }}Glossário#ogp)); 
3. O alinhamento perante o Planejamento Estratégico Institucional (PEI) e os planejamentos setoriais, bem como os relacionados às áreas de tecnologia da informação;
4. O conjunto de informações e sistemas sob a gestão do órgão, em especial, se houver, sistemas estruturadores que são de uso obrigatório transversal para os órgãos da APF;
5. O nível de maturidade e organização das informações e dados existentes.

Outra fonte importante para orientação é a lista de [conjuntos de dados de alto valor](https://www.gov.uk/government/publications/open-data-charter/g8-open-data-charter-and-technical-annex#action-2-release-of-high-value-data), 
trazida pelo [Open Data Charter](https://www.gov.uk/government/publications/open-data-charter) do [G8](http://en.wikipedia.org/wiki/G8).

## Definir estratégias de abertura

Priorizados os dados mais importantes, é hora de definir de que forma eles serão publicados. Essa forma será influenciada pelos seguintes fatores:

* Local onde os dados estão estruturados
* Forma como os dados estão estruturados
* Capacidade técnica da organização

Na prática, esses fatores se traduzem em possíveis cenários de status dos dados, como dados estruturados em várias planilhas, bancos de dados locais, bancos de dados situados no fornecedor, conjuntos muito volumosos, plataforma alta ou baixa, data warehouse, etc. 

Cada cenário envolve uma tática diferente, em casos de dados muito volumosos, uma separação em diversos arquivos compactados, por exemplo, ou a criação de API, a depender também da capacidade dos órgãos. Dados de data warehouse devem ser evitados por causa dos princípios dos dados brutos e primários, mas excepcionalmente podem ser utilizados quando a extração direta não for viável.

Além da forma de publicação, a periodicidade de publicação e a forma de hospedagem precisam ser definidas, a depender das particularidades da área de negócio, dos sistemas de informação relacionados e dos recursos de infraestrutura disponíveis.


## Definir cronograma e marcos

Nesse momento já está definido, para cada um dos dados priorizados, a tática
de publicação, dentro das limitações da organização e das particularidades das
bases de dados. Resta agora pensar nas datas de publicação de cada um deles.

Entretanto, é preciso ter em mente que não apenas as ações de abertura de
dados devem integrar o Plano de Ação do Plano de Dados Abertos. É importante
pensar também em ações como:

* melhorias na qualidade de dados de dados que já são publicados
* melhorias na frequência de atualização automatizada dos dados já publicados
* melhorias na documentação dos dados já publicados (incluindo dicionários de dados, metadados, etc.)
* criação de catálogos de dados institucionais
* ações de integração de catálogos de dados existentes na instituição com o [Portal Brasileiro de Dados Abertos](http://dados.gov.br)
* ações de capacitação interna

Além disso, essa é a ocasião certa para pensar em ações de comunicação e
articulação com a sociedade civil para aumentar a legitimidade e potencializar
a publicação dos dados. Conforme o [Manual para elaboração de
PDA](http://www.planejamento.gov.br/secretarias/upload/Arquivos/governo_aberto/manual_elaboracao_plano_dados_abertos.pdf), exemplos de ações como essas são: 

* realizar encontros com os interessados nos dados (por exemplo, promover uma [expedição de dados](http://escoladedados.org/expedicao-de-dados/))
* realizar concursos de aplicativos (exemplos pioneiros: [concursos do MJ](http://www.justica.gov.br/dados-abertos), [concursos do INEP](http://hackathondadoseducacionais.org.br/), [concurso do Ministério do Planejamento](http://dados.gov.br/noticia/conheca-os-vencedores-do-concurso-nacional-de-dados-abertos/), 
[Desarrollando América Latina](http://desarrollandoamerica.org/))
* produzir guias de utilição dos dados
* apresentar em destaque os dados mais pedidos pelo SIC
* estimular o uso interno e por outros órgãos públicos dos dados publicados
* disseminar na organização a cultura de acesso à informação e de disponibilização de dados públicos.

