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
        Publicar dump da base de dados
      </td>

      <td>
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
        Publicar dados em arquivos CSV
      </td>

      <td>
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
        Publicar dados em arquivos JSON / XML
      </td>

      <td>
        Mecanismo de ETL (caso esteja em banco relacional)
      </td>

      <td rowspan="3">
        M&eacute;dio
      </td>

    </tr>

    <tr>
      <td>
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
        Desenvolver m&oacute;dulo de dados abertos em sistema existente
      </td>

      <td>
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
        Desenvolver API RESTful de dados abertos desacoplada da
        solu&ccedil;&atilde;o
      </td>

      <td>
        Mecanismo de ETL
      </td>

      <td rowspan="3">
        Longo
      </td>

    </tr>

    <tr>
      <td>
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
        Novo Sistema, com a gest&atilde;o de dados incorporados em sua arquitetura
      </td>

      <td>
        Mecanismo de ETL
      </td>

      <td rowspan="3">
        Longo
      </td>

    </tr>

    <tr>
      <td>
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
        Publicar dados em arquivos RDF
      </td>

      <td>
        Ontologia da &aacute;rea do conhecimento do sistema
      </td>

      <td rowspan="3">
        Longo
      </td>

    </tr>

    <tr>
      <td>
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
        Disponibilizar dados por Endpoint SPARQL
      </td>

      <td>
        Ontologia da &aacute;rea do conhecimento do sistema
      </td>

      <td rowspan="3">
        Mais Longo
      </td>

    </tr>

    <tr>
      <td>
        Servi&ccedil;o de ETL
      </td>

    </tr>

    <tr>
      <td>
        Banco de dados de triplas
      </td>

    </tr>

    <tr>

      <td rowspan="5">
        Publicar dados em API de dados ligados (Linked Data)
      </td>

      <td>
        Ontologia da &aacute;rea do conhecimento do sistema
      </td>

      <td rowspan="5">
        Mais Longo
      </td>

    </tr>

    <tr>
      <td>
        Banco de dados de triplas
      </td>

    </tr>

    <tr>
      <td>
        Servi&ccedil;o de desenvolvimento
      </td>

    </tr>

    <tr>
      <td>
        Mecanismo de ETL
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para deploy da nova solu&ccedil;&atilde;o
      </td>

    </tr>
  </table>


1. Publicar dump da base de dados
2. Publicar dados em arquivos CSV
3. Publicar dados em arquivos JSON / XML
4. Desenvolver módulo de dados abertos em sistema existente
5. Desenvolver API RESTful de dados abertos desacoplada da solução
6. Novo Sistema, com a gestão de dados incorporados em sua arquitetura
7. Publicar dados em arquivos RDF
8. Disponibilizar dados por Endpoint SPARQL
9. Publicar dados em API de dados ligados (Linked Data)





