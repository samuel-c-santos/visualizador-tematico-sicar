# Visualizador Temático SICAR

Este aplicativo web permite a visualização e exportação de temas de arquivos Shapefile (.zip) do Sistema Nacional de Cadastro Ambiental Rural (SICAR). Desenvolvido para facilitar a análise de dados geográficos, o visualizador agora oferece opções de exportação para GeoJSON e KML, garantindo compatibilidade com diversos softwares SIG.

## Funcionalidades

* **Importação de Shapefile:** Carregue arquivos Shapefile compactados (.zip) provenientes do SICAR.
* **Visualização Temática:** Os temas do Shapefile são exibidos no mapa, permitindo controle individual da visibilidade de cada camada.
* **Exportação de Dados:** Exporte as camadas temáticas para:
    * **GeoJSON:** Formato padrão para dados geográficos na web, amplamente compatível.
    * **KML:** Formato keyhole markup language, adequado para visualização no Google Earth e outros SIGs. (Com correções de codificação para melhor compatibilidade com QGIS).
* **Base de Mapas:** Alterne entre diferentes bases de mapas, incluindo imagens de satélite (Google Satélite, Bing Maps) e mapas de ruas (OpenStreetMap, CartoDB Voyager), além de camadas Sentinel-2 de vários anos.

## Problemas Resolvidos (Versão Atual)

* **Exportação de Shapefile Removida:** A opção de exportação para Shapefile foi descontinuada devido a problemas de compatibilidade e complexidade, focando em formatos mais acessíveis (GeoJSON e KML).
* **Corrupção de Nomes de Arquivos na Exportação (KML):** Nomes de arquivos e de temas com acentos e caracteres especiais agora são devidamente sanitizados e escapados, garantindo a integridade dos dados exportados para KML, especialmente ao serem abertos em softwares como o QGIS.
* **Legibilidade KML no QGIS:** A estrutura KML foi aprimorada, incluindo a marca de ordem de byte (BOM) UTF-8 e o tratamento correto de multi-geometrias (MultiPoint, MultiLineString, MultiPolygon e Polygons com furos), garantindo que os arquivos KML sejam reconhecidos e exibidos sem erros no QGIS.

## Como Usar

1.  **Baixe** o código fonte completo.
2.  **Descompacte** os arquivos em uma pasta local.
3.  **Abra** o arquivo `index.html` diretamente em seu navegador web (Google Chrome, Firefox, etc.).
4.  **Importe** um arquivo Shapefile zipado do SICAR utilizando o botão "Importar arquivo".
5.  **Visualize** as camadas e utilize os botões de exportação para salvar os temas em GeoJSON ou KML.

## Acesso ao SICAR

Você pode obter os arquivos por cadastro diretamente no site do SICAR:
[SICAR - Consulta Geral](https://car.semas.pa.gov.br/#/consulta/geral?tela=BUSCAR_CADASTRO)

## Desenvolvimento

Desenvolvido por [Samuel Santos](https://samuel-c-santos.github.io/).