---
published: true
permalink: /Mapa-de-decisões-tecnológicas/
layout: slate
filename: Mapa-de-decisões-tecnológicas.md
title: Mapa de decisões - Kit de Dados Abertos
desc: Neste mapa são apresentadas diversas formas de publicação de dados abertos, dando ao gestor parâmetros de apoio à decisão.
---

## Mapa de decisões tecnológicas

A tabela abaixo mostra as soluções mais comuns para publicar dados abertos, ordenadas por complexidade e prazo de implementação.

<!---
Abaixo o código HTML da tabela, markdown não suporta colspan.
--->

<table class="tabela-decisoes-tecnologicas">
    <!--<colgroup>
      <col width="118" />
      <col width="424" />
      <col width="302" />
      <col width="200" />
    </colgroup>-->

    <tr>

      <th>
        Solu&ccedil;&atilde;o
      </th>

      <th>
        Pr&eacute;-requisitos
      </th>

      <th>
        Prazo
      </th>

    </tr>

    <tr>

      <td rowspan="2">
        <a href="#publicar-dump-da-base-de-dados">Publicar dump da base de dados</a>
      </td>

      <td class="celula-meio">
        Acesso &agrave; base de dados
      </td>

      <td rowspan="2">
        Curto<br />
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para arquivos
      </td>

    </tr>

    <tr>

      <td rowspan="2">
        <a href="#publicar-dados-em-arquivos-csv">Publicar dados em arquivos CSV</a>
      </td>

      <td class="celula-meio">
        Mecanismo de ETL (caso esteja em banco relacional)
      </td>

      <td rowspan="2">
        Curto<br />
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para arquivos
      </td>

    </tr>

    <tr>

      <td rowspan="3">
        <a href="#publicar-dados-em-arquivos-json--xml">Publicar dados em arquivos JSON / XML</a>
      </td>

      <td class="celula-meio">
        Mecanismo de ETL (caso esteja em banco relacional)
      </td>

      <td rowspan="3">
        M&eacute;dio
      </td>

    </tr>

    <tr>
      <td class="celula-meio">
        Servi&ccedil;o de desenvolvimento
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para arquivos
      </td>

    </tr>

    <tr>

      <td rowspan="2">
        <a href="#desenvolver-mdulo-de-dados-abertos-em-sistema-existente">Desenvolver m&oacute;dulo de dados abertos em sistema existente</a>
      </td>

      <td class="celula-meio">
        Servi&ccedil;o de desenvolvimento
      </td>

      <td rowspan="2">
        Longo
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para deploy da nova solu&ccedil;&atilde;o
      </td>

    </tr>

    <tr>

      <td rowspan="3">
        <a href="#desenvolver-api-restful-de-dados-abertos-desacoplada-da-soluo">Desenvolver API RESTful de dados abertos desacoplada da
        solu&ccedil;&atilde;o</a>
      </td>

      <td class="celula-meio">
        Mecanismo de ETL
      </td>

      <td rowspan="3">
        Longo
      </td>

    </tr>

    <tr>
      <td class="celula-meio">
        Servi&ccedil;o de desenvolvimento
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para deploy da nova solu&ccedil;&atilde;o
      </td>

    </tr>

    <tr>

      <td rowspan="3">
        <a href="#novo-sistema-com-a-gesto-de-dados-incorporados-em-sua-arquitetura">Novo Sistema, com a gest&atilde;o de dados incorporados em sua arquitetura</a>
      </td>

      <td class="celula-meio">
        Mecanismo de ETL
      </td>

      <td rowspan="3">
        Longo
      </td>

    </tr>

    <tr>
      <td class="celula-meio">
        Servi&ccedil;o de desenvolvimento
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para deploy da nova solu&ccedil;&atilde;o
      </td>

    </tr>

    <tr>

      <td rowspan="3">
        <a href="#publicar-dados-em-arquivos-rdf">Publicar dados em arquivos RDF</a>
      </td>

      <td class="celula-meio">
        Ontologia da &aacute;rea do conhecimento do sistema
      </td>

      <td rowspan="3">
        Longo
      </td>

    </tr>

    <tr>
      <td class="celula-meio">
        Mecanismo de ETL
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para arquivos
      </td>

    </tr>

    <tr>

      <td rowspan="3">
        <a href="#disponibilizar-dados-por-endpoint-sparql">Disponibilizar dados por Endpoint SPARQL</a>
      </td>

      <td class="celula-meio">
        Ontologia da &aacute;rea do conhecimento do sistema
      </td>

      <td rowspan="3">
        Mais Longo
      </td>

    </tr>

    <tr>
      <td class="celula-meio">
        Mecanismo de ETL
      </td>

    </tr>

    <tr>
      <td>
        Banco de dados de triplas
      </td>

    </tr>

    <tr>

      <td rowspan="5">
        <a href="#publicar-dados-em-api-de-dados-ligados-linked-data">Publicar dados em API de dados ligados (Linked Data)</a>
      </td>

      <td class="celula-meio">
        Ontologia da &aacute;rea do conhecimento do sistema
      </td>

      <td rowspan="5">
        Mais Longo
      </td>

    </tr>

    <tr>
      <td class="celula-meio">
        Banco de dados de triplas
      </td>

    </tr>

    <tr>
      <td class="celula-meio">
        Servi&ccedil;o de desenvolvimento
      </td>

    </tr>

    <tr>
      <td class="celula-meio">
        Mecanismo de ETL
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para deploy da nova solu&ccedil;&atilde;o
      </td>

    </tr>
  </table>


#### Publicar dump da base de dados


#### Publicar dados em arquivos CSV


#### Publicar dados em arquivos JSON / XML


#### Desenvolver módulo de dados abertos em sistema existente


#### Desenvolver API RESTful de dados abertos desacoplada da solução


#### Novo Sistema, com a gestão de dados incorporados em sua arquitetura


#### Publicar dados em arquivos RDF


#### Disponibilizar dados por Endpoint SPARQL


#### Publicar dados em API de dados ligados (Linked Data)


