# Dashboard Porsche — Sales Intelligence

- **Dashboard:** [Abrir a dashboard](https://megadurck.github.io/Simulador_Investimento/Dashboard-Porsche/)
- **Repositório:** [Megadurck/Simulador_Investimento](https://github.com/Megadurck/Simulador_Investimento)
- **Branch:** `Dashboard-Porsche`

## Perguntas de negócio

- **Qual modelo vende mais?** Ajuda a identificar a demanda por produto e orientar decisões de estoque e foco comercial.
- **Quais cidades concentram as vendas?** Mostra onde a operação tem maior volume e onde oportunidades regionais podem existir.
- **Como as vendas se distribuem por Model Year?** Permite comparar a composição das vendas por ano-modelo.
- **Quais formas de pagamento aparecem com mais frequência?** Ajuda a entender o perfil de pagamento da base.
- **Qual modelo lidera em cada cidade?** Cruza produto e localização para apoiar análises comerciais locais.

Os filtros de modelo, ano-modelo, cidade e forma de pagamento atualizam os indicadores, gráficos, insights e ranking.

## Prompt e evolução

O histórico disponível não contém o prompt original que gerou o HTML, então não apresento uma transcrição inventada. Para esta publicação, o prompt de implementação registrado foi:

> Publique o HTML existente como dashboard estática no GitHub Pages. Preserve a importação de Excel, o mapeamento de colunas, os filtros por modelo, ano-modelo, cidade e forma de pagamento, os KPIs, gráficos, insights e ranking. Não publique a planilha original nem dados reais; crie uma amostra fictícia claramente identificada para que a página abra pronta para demonstração. Documente as perguntas de negócio, o tratamento dos dados, as ferramentas usadas e o endereço publicado.

O HTML de partida já tinha importação de Excel, seleção de colunas, filtros, KPIs, gráficos, insights e ranking. Para a versão publicada, foi adicionada uma amostra fictícia carregada por padrão; a importação continua disponível e substitui essa amostra. Também foram adicionados este README e o fluxo de publicação no GitHub Pages.

## Tratamento e privacidade dos dados

A planilha original não foi enviada à IA, não foi copiada para este repositório e não está embutida no HTML. Como ela não foi auditada para publicação, a demonstração usa somente 18 registros sintéticos, criados para testar filtros e visualizações; seus valores não representam vendas reais.

Ao importar uma planilha própria, a dashboard lê o primeiro arquivo e a primeira aba no navegador. Ela tenta reconhecer nomes de colunas comuns e permite ajustar o mapeamento antes da análise. Modelo, ano-modelo, cidade e pagamento são necessários; preço/receita é opcional. A receita interpreta valores numéricos e formatos monetários em português. Os dados carregados permanecem no navegador e não são enviados a um servidor pela aplicação.

## Ferramentas

Não foi usado ChatGPT com Canvas para gerar esta versão. O HTML existente foi integrado e documentado com assistência de IA no VS Code; a skill `graphify` foi invocada na conversa anterior para responder uma pergunta sobre o código, mas não foi usada para gerar a dashboard.

## Publicação e demonstração

O workflow [`../.github/workflows/deploy-dashboard-porsche.yml`](../.github/workflows/deploy-dashboard-porsche.yml) publica o conteúdo desta pasta no GitHub Pages a cada atualização da branch `Dashboard-Porsche`. A página abre com os dados sintéticos e os filtros já disponíveis; por exemplo, selecionar **São Paulo** no filtro **CITY** limita os indicadores e gráficos às vendas fictícias dessa cidade.

Para usar dados próprios, selecione **IMPORTAR EXCEL** e escolha uma planilha `.xlsx` ou `.xls`. Não publique planilhas com dados pessoais ou comerciais sensíveis.
