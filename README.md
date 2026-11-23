# Dashboard de vendas Xbox

Projeto de Excel da DIO para organizar e visualizar os dados de vendas de assinaturas.

## Dados
Base didática da DIO, com 295 registros iniciados em 2024. Nomes e identificadores originais foram omitidos. Campos de preço de EA Play com hífen foram normalizados para zero. A base não especifica a moeda, por isso os valores são apresentados em unidades monetárias.

Fonte: https://hermes.dio.me/files/assets/805d54f9-6d53-4246-bed7-4aa2da615923.xlsx

## Arquivo e uso
Abra dashboard-xbox.xlsx no Excel. Na aba Dashboard, selecione o tipo de assinatura em C5: Todos, Annual, Monthly ou Quarterly. Os totais e os gráficos nativos atualizam com as fórmulas. A aba Dados contém a base utilizada e a conciliação por registro.

## Indicadores
- Quantidade de registros, valor total e valor médio.
- Valores por plano e por mês de início.
- Composição por assinaturas, EA Play, Minecraft e cupons.

O valor de cada registro é somado uma única vez. Não há anualização ou suposição de receitas recorrentes. O valor total da base é 7.633 e o número de registros é 295.

## Reprodução e validação
As agregações usam SUMIFS e COUNTIFS, vinculadas ao filtro C5. Os gráficos leem as tabelas calculadas. A conciliação calcula assinatura + EA Play + Minecraft - cupom e compara com o valor original. Todas as 295 diferenças são zero. Os quatro filtros foram comparados com somas independentes da base.
