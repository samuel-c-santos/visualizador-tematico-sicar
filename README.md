# Visualizador Temático SICAR

Este aplicativo web foi desenvolvido para atender a uma necessidade prática e comum entre colegas técnicos que trabalham diariamente com o **Cadastro Ambiental Rural (CAR)**.

### O Problema: Dados Geoespaciais Complexos do CAR

Frequentemente, o **técnico analista** encaminha via central de comunicação ao **técnico cadastrante** arquivos geoespaciais essenciais para as retificações do CAR notificado. O grande desafio é que todas as camadas temáticas importantes — como área consolidada, remanescente de vegetação nativa, servidão ambiental, entre outras — chegam compiladas em um único arquivo shapefile zipado.

Tradicionalmente, para visualizar essas camadas ou extraí-las individualmente para uso no módulo de cadastro, seria necessário:
1.  Possuir e instalar um software GIS robusto, como o QGIS.
2.  Realizar várias etapas manuais de extração e importação das camadas.
3.  Lidar com possíveis problemas de compatibilidade e codificação.

Esse processo demanda tempo, conhecimento técnico específico em GIS e pode ser um gargalo nas operações diárias.

### A Solução: Visualização Simplificada e Acessível

Para simplificar esse fluxo de trabalho e torná-lo acessível a **qualquer usuário**, sem a necessidade de softwares complexos ou múltiplas etapas, o **Visualizador Temático SICAR** oferece uma solução intuitiva e online. Ele foi pensado para que você possa focar no que realmente importa: **a análise dos dados do CAR**.

Com este aplicativo, basta carregar o arquivo ZIP do Shapefile do SICAR e todas as suas camadas serão exibidas de forma interativa no mapa, prontas para serem visualizadas e, se necessário, exportadas de maneira descomplicada.

---

## Acesso Rápido

É super simples de usar e está disponível diretamente no seu navegador!

1.  **Acesse o aplicativo:** [https://samuel-c-santos.github.io/visualizador-tematico-sicar/](https://samuel-c-santos.github.io/visualizador-tematico-sicar/)
2.  **Importe o Shapefile:** Clique em "Importar arquivo" e selecione o ZIP do Shapefile que você recebeu do SICAR.
3.  **Visualize e Controle:** As camadas aparecerão no mapa. Você pode controlar a visibilidade de cada tema individualmente no menu lateral.
4.  **Exporte Facilmente:** Se precisar dos dados para usar em outras ferramentas ou apenas para arquivar, exporte-os convenientemente como **GeoJSON** ou **KML**. A exportação KML foi especialmente aprimorada para garantir a leitura correta no QGIS, inclusive com caracteres especiais e múltiplas geometrias, solucionando os problemas de "Fonte de dados inválida".

Você também pode explorar diferentes bases de mapa, como imagens de satélite (Google Satélite, Bing Maps) e imagens Sentinel-2 de vários anos, para um contexto visual mais rico.

---

## Captura de Tela

Aqui está uma prévia do aplicativo em funcionamento:

[![Visualizador Temático SICAR](https://github.com/samuel-c-santos/visualizador-tematico-sicar/blob/master/captura-de-tela.png?raw=true)](https://samuel-c-santos.github.io/visualizador-tematico-sicar/)

---

## Fonte dos Dados (SICAR)

Você pode obter os arquivos por cadastro diretamente no site do SICAR:
[SICAR - Consulta Geral](https://car.semas.pa.gov.br/#/consulta/geral?tela=BUSCAR_CADASTRO)

---

## Desenvolvimento

Desenvolvido por [Samuel Santos](https://samuel-c-santos.github.io/).