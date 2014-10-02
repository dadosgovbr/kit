---
published: true
permalink: /Mapa-de-decisões-tecnológicas/
layout: slate
filename: Mapa-de-decisões-tecnológicas.md
title: Mapa de decisões - Kit de Dados Abertos
desc: Neste mapa são apresentadas diversas formas de publicação de dados abertos, dando ao gestor parâmetros de apoio à decisão.
---

<!---
Abaixo o código HTML da tabela, markdown não suporta colspan. Melhorar isso =p
--->

<table><colgroup><col width="118"/><col width="424"/><col width="302"/><col width="200"/><col width="117"/></colgroup><tr ><td  ><p>Complexidade</p></td><td  ><p>Solução</p></td><td  ><p>Pré-requisitos</p></td><td  ><p>Prazo de implementação</p></td><td  > </td></tr><tr ><td rowspan="2"  ><p>1</p></td><td rowspan="2"  ><p>Publicar dump da base de dados</p></td><td  ><p>Acesso à base de dados</p></td><td rowspan="2"  ><p>Curto<br/></p></td><td  > </td></tr><tr ><td  ><p>Servidor web para arquivos</p></td><td  > </td></tr><tr ><td rowspan="2"  ><p>2</p></td><td rowspan="2"  ><p>Publicar dados em arquivos CSV</p></td><td  ><p>Mecanismo de ETL (caso esteja em banco relacional)</p></td><td rowspan="2"  ><p>Curto<br/></p></td><td  > </td></tr><tr ><td  ><p>Servidor web para arquivos</p></td><td  > </td></tr><tr ><td rowspan="3"  ><p>3</p></td><td rowspan="3"  ><p>Publicar dados em arquivos JSON / XML</p></td><td  ><p>Mecanismo de ETL (caso esteja em banco relacional)</p></td><td rowspan="3"  ><p>Médio</p></td><td  > </td></tr><tr ><td  ><p>Serviço de desenvolvimento</p></td><td  > </td></tr><tr ><td  ><p>Servidor web para arquivos</p></td><td  > </td></tr><tr ><td rowspan="2"  ><p>4</p></td><td rowspan="2"  ><p>Desenvolver módulo de dados abertos em sistema existente</p></td><td  ><p>Serviço de desenvolvimento</p></td><td rowspan="2"  ><p>Longo</p></td><td  > </td></tr><tr ><td  ><p>Servidor web para deploy da nova solução</p></td><td  > </td></tr><tr ><td rowspan="3"  ><p>5</p></td><td rowspan="3"  ><p>Desenvolver API RESTful de dados abertos desacoplada da solução</p></td><td  ><p>Mecanismo de ETL</p></td><td rowspan="3"  ><p>Longo</p></td><td  > </td></tr><tr ><td  ><p>Serviço de desenvolvimento</p></td><td  > </td></tr><tr ><td  ><p>Servidor web para deploy da nova solução</p></td><td  > </td></tr><tr ><td rowspan="3"  ><p>6</p></td><td rowspan="3"  ><p>Novo Sistema, com a gestão de dados incorporados em sua arquitetura</p></td><td  ><p>Mecanismo de ETL</p></td><td rowspan="3"  ><p>Longo</p></td><td  > </td></tr><tr ><td  ><p>Serviço de desenvolvimento</p></td><td  > </td></tr><tr ><td  ><p>Servidor web para deploy da nova solução</p></td><td  > </td></tr><tr ><td rowspan="3"  ><p>8</p></td><td rowspan="3"  ><p>Publicar dados em arquivos RDF</p></td><td  ><p>Ontologia da área do conhecimento do sistema</p></td><td rowspan="3"  ><p>Longo</p></td><td  > </td></tr><tr ><td  ><p>Mecanismo de ETL</p></td><td  > </td></tr><tr ><td  ><p>Servidor web para arquivos</p></td><td  > </td></tr><tr ><td rowspan="3"  ><p>9</p></td><td rowspan="3"  ><p>Disponibilizar dados por Endpoint SPARQL</p></td><td  ><p>Ontologia da área do conhecimento do sistema</p></td><td rowspan="3"  ><p>Mais Longo</p></td><td  > </td></tr><tr ><td  ><p>Serviço de ETL</p></td><td  > </td></tr><tr ><td  ><p>Banco de dados de triplas</p></td><td  > </td></tr><tr ><td rowspan="5"  ><p>11</p></td><td rowspan="5"  ><p>Publicar dados em API de dados ligados (Linked Data)</p></td><td  ><p>Ontologia da área do conhecimento do sistema</p></td><td rowspan="5"  ><p>Mais Longo</p></td><td  > </td></tr><tr ><td  ><p>Banco de dados de triplas</p></td><td  > </td></tr><tr ><td  ><p>Serviço de desenvolvimento</p></td><td  > </td></tr><tr ><td  ><p>Mecanismo de ETL</p></td><td  > </td></tr><tr ><td  ><p>Servidor web para deploy da nova solução</p></td><td  > </td></tr></table>


1. Publicar dump da base de dados
2. Publicar dados em arquivos CSV
3. Publicar dados em arquivos JSON / XML
4. Desenvolver módulo de dados abertos em sistema existente
5. Desenvolver API RESTful de dados abertos desacoplada da solução
6. Novo Sistema, com a gestão de dados incorporados em sua arquitetura
7. Publicar dados em arquivos RDF
8. Disponibilizar dados por Endpoint SPARQL
9. Publicar dados em API de dados ligados (Linked Data)





