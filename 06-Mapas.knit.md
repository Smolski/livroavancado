# Mapas

Este capítulo almeja levantar o ferramental básico para a construção de mapas simples no RStudio. Ainda, interessa demonstrar os comandos para a manipulação destes tipos de bases de dados, inclusive possibilitando a junção de indicadores de municípios, regiões e países. Estes dados podem ser advindos de institutos de pesquisas ou mesmo dados criados pelo estudante em suas análises.

Os pacotes utilizados neste capítulo são: `tmap`, `maptools`,
`tmap` e `rgdal`.

## Introdução aos *shapes*

Existem vários *softwares* específicos para a produção de mapas, sejam produtos comerciais ou no formato *software* livre. A grande vantagem da utilização do R para criação de mapas é a utilização dos *shapes* disponibilizadas para vários programas. 

Denominam-se *shapes* os arquivos que contém os elementos gráficos, em formato de ponto, linhas ou polígonos, contendo coordenadas geográficas para um elemento para que possa ser transformado em mapa. O *shape* é formado por três arquivos principais individuais que armazenam os dados: o arquivo ".shp", ".shx" e ".dbf". Além disto, podem ser acompanhados de arquivos ".prj", o ".sbn" e o ".sbx" [@Semace2018].

Os *shapefiles* podem ser obtidos de várias fontes oficiais, como institutos de pesquisa e universidades. A seguir alguns links para *download*:

- IBGE: 
ftp://geoftp.ibge.gov.br/organizacao_do_territorio/malhas_territoriais/malhas_municipais/municipio_2016/Brasil/BR/

https://mapas.ibge.gov.br/bases-e-referenciais/bases-cartograficas/malhas-digitais.html

http://dados.gov.br/dataset/malha-geometrica-dos-municipios-brasileiros

- IPEAGEO: http://www.ipea.gov.br/ipeageo/malhas.html

- Forest Gis: http://forest-gis.com/2009/04/base-de-dados-shapefile-do-brasil-todo.html/

- FEPAM: http://www.fepam.rs.gov.br/biblioteca/geo/bases_geo.asp


No exemplo abaixo, é utilizado um *shape* proveniente do IBGE representando os municípios do Estado do Rio Grande do Sul. Ao *shape* denominado `municipios_IBGE` será dado o nome de MAPA_RS:



























