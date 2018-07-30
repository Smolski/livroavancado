# Mapas

Este cap�tulo almeja levantar o ferramental b�sico para a constru��o de mapas simples no RStudio. Ainda, interessa demonstrar os comandos para a manipula��o destes tipos de bases de dados, inclusive possibilitando a jun��o de indicadores de munic�pios, regi�es e pa�ses. Estes dados podem ser advindos de institutos de pesquisas ou mesmo dados criados pelo estudante em suas an�lises.

Os pacotes utilizados neste cap�tulo s�o: `tmap`, `maptools`,
`tmap` e `rgdal`.

## Introdu��o aos *shapes*

Existem v�rios *softwares* espec�ficos para a produ��o de mapas, sejam produtos comerciais ou no formato *software* livre. A grande vantagem da utiliza��o do R para cria��o de mapas � a utiliza��o dos *shapes* disponibilizadas para v�rios programas. 

Denominam-se *shapes* os arquivos que cont�m os elementos gr�ficos, em formato de ponto, linhas ou pol�gonos, contendo coordenadas geogr�ficas para um elemento para que possa ser transformado em mapa. O *shape* � formado por tr�s arquivos principais individuais que armazenam os dados: o arquivo ".shp", ".shx" e ".dbf". Al�m disto, podem ser acompanhados de arquivos ".prj", o ".sbn" e o ".sbx" [@Semace2018].

Os *shapefiles* podem ser obtidos de v�rias fontes oficiais, como institutos de pesquisa e universidades. A seguir alguns links para *download*:

- IBGE: 
ftp://geoftp.ibge.gov.br/organizacao_do_territorio/malhas_territoriais/malhas_municipais/municipio_2016/Brasil/BR/

https://mapas.ibge.gov.br/bases-e-referenciais/bases-cartograficas/malhas-digitais.html

http://dados.gov.br/dataset/malha-geometrica-dos-municipios-brasileiros

- IPEAGEO: http://www.ipea.gov.br/ipeageo/malhas.html

- Forest Gis: http://forest-gis.com/2009/04/base-de-dados-shapefile-do-brasil-todo.html/

- FEPAM: http://www.fepam.rs.gov.br/biblioteca/geo/bases_geo.asp


No exemplo abaixo, � utilizado um *shape* proveniente do IBGE representando os munic�pios do Estado do Rio Grande do Sul. Ao *shape* denominado `municipios_IBGE` ser� dado o nome de MAPA_RS:



























