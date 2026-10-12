# Simulador_Investimento
# 📊 Ferramenta de Controle de Investimentos com Excel

Projeto desenvolvido durante o desafio **Criando uma Ferramenta de Controle de Investimentos com Excel**, da trilha **Reclame Aqui — Dados e IA na Prática**, da [DIO](https://www.dio.me/).

A ferramenta permite simular a evolução do patrimônio por meio de aportes mensais, estimar os dividendos mensais e visualizar a distribuição dos investimentos em diferentes tipos de Fundos de Investimento Imobiliário (FIIs), conforme o perfil selecionado.

## 🎯 Objetivo do Projeto

Desenvolver uma ferramenta interativa no Excel que transforme parâmetros financeiros em informações úteis para o planejamento de investimentos, com cálculos automatizados, cenários de longo prazo e uma interface organizada para facilitar a utilização.

## ⚙️ Funcionalidades

- **Simulação de patrimônio:** cálculo do patrimônio acumulado com base no aporte mensal, no prazo e na taxa de rendimento.
- **Estimativa de dividendos:** projeção dos rendimentos mensais a partir do patrimônio acumulado e da taxa informada.
- **Projeção de cenários:** comparação do patrimônio estimado para períodos de 2, 5, 10, 20 e 30 anos.
- **Sugestão de aporte:** cálculo de uma sugestão de investimento mensal equivalente a 30% do salário informado.
- **Perfis de investimento:** seleção de um perfil por meio de uma lista suspensa, com distribuição percentual entre seis tipos de fundos imobiliários.
- **Distribuição automatizada:** cálculo dos valores destinados a cada categoria de fundo conforme o aporte e o perfil selecionado.
- **Interface organizada:** separação visual entre campos de entrada e células calculadas, facilitando a utilização da ferramenta.

## 🧮 Conceitos e recursos do Excel utilizados

### Função VF

A função `VF` (Valor Futuro) é utilizada para estimar o patrimônio acumulado ao longo do tempo, considerando uma taxa periódica, a quantidade de períodos e os aportes realizados.

Ela permite projetar o crescimento dos investimentos com base nos parâmetros definidos pelo usuário.

**Principais variáveis da simulação:**

- Taxa de rendimento mensal;
- Quantidade de meses do investimento;
- Valor do aporte mensal;
- Valor inicial, quando aplicável;
- Momento em que os pagamentos são realizados.

O resultado é uma estimativa matemática baseada nas premissas informadas, não uma garantia de rentabilidade futura.

### Função PROCV e chave composta

A função `PROCV` é utilizada para consultar a tabela de apoio e retornar o percentual correspondente a cada tipo de fundo dentro do perfil selecionado.

Para identificar corretamente cada combinação, utiliza-se uma **chave composta**, formada pela junção de informações como perfil de investimento e tipo de fundo.

Essa abordagem permite organizar os dados em uma tabela de referência e automatizar a distribuição dos aportes sem precisar alterar manualmente cada percentual.

### Intervalos nomeados

Foram utilizados intervalos nomeados para identificar parâmetros importantes da simulação, como:

- `aporte`
- `taxa_mensal`

O uso de nomes torna as fórmulas mais legíveis, facilita a manutenção da planilha e reduz a dependência de referências diretas a endereços de células.

### Validação de dados

A lista suspensa de perfis utiliza validação de dados para restringir as opções disponíveis e permitir a alteração do perfil de investimento de maneira simples e controlada.

## 📈 Perfis de investimento

A ferramenta distribui o aporte mensal entre seis categorias de fundos imobiliários, de acordo com o perfil selecionado.

Os percentuais são definidos em uma tabela auxiliar e utilizados nos cálculos de distribuição.

**Importante:** os percentuais configurados são parâmetros ilustrativos para fins educacionais. Não representam recomendação de investimento nem uma carteira ideal para qualquer investidor. Cada perfil deve totalizar 100% da distribuição.

## 🛠️ Tecnologias e recursos

- Microsoft Excel ou aplicativo compatível com as funções utilizadas;
- Fórmulas financeiras;
- Funções de busca e referência;
- Validação de dados;
- Intervalos nomeados;
- Formatação e organização visual de planilhas.

## ▶️ Como utilizar

1. Baixe o arquivo da planilha disponibilizado neste repositório.
2. Abra-o no Excel ou em um aplicativo compatível.
3. Informe o salário e o valor do aporte mensal desejado.
4. Defina o prazo do investimento e a taxa de rendimento mensal utilizada na simulação.
5. Consulte o patrimônio acumulado e a estimativa de dividendos mensais.
6. Compare os cenários de investimento em diferentes prazos.
7. Selecione outro perfil de investimento e observe como a distribuição do aporte se altera.

Os resultados são recalculados conforme os parâmetros informados e as fórmulas configuradas na planilha.

## 🧠 Aprendizados

O desenvolvimento deste projeto permitiu praticar conceitos que vão além da criação de fórmulas isoladas:

- Tradução de perguntas de negócio em requisitos funcionais;
- Modelagem de parâmetros e tabelas auxiliares;
- Automatização de cálculos financeiros;
- Uso de referências absolutas e intervalos nomeados;
- Busca de dados por meio de chaves compostas;
- Aplicação de validação de dados;
- Organização visual de uma ferramenta voltada ao usuário final;
- Transformação de dados em informações úteis para tomada de decisão.

## 🚀 Possíveis evoluções

Entre as melhorias que podem ser incorporadas futuramente estão:

- Gráfico de pizza dinâmico para visualizar a distribuição dos aportes;
- Comparação entre o aporte informado e a sugestão baseada em 30% do salário;
- Inclusão de novos cenários e parâmetros de simulação;
- Indicadores visuais para facilitar a comparação entre perfis.

## ⚠️ Aviso

Esta ferramenta possui finalidade **educacional e de simulação financeira**. Os resultados dependem dos valores e das taxas informados pelo usuário. A planilha não considera automaticamente todos os fatores que podem afetar os investimentos, como impostos, taxas, inflação, oscilações de preços e variações nos dividendos.

As projeções não garantem resultados futuros e não constituem recomendação de investimento.

## 👨‍💻 Autor

**Romário — Desenvolvedor Back-End | Análise e Desenvolvimento de Sistemas**

Este projeto faz parte da minha jornada de aprendizado contínuo em tecnologia, análise de dados, automação e resolução de problemas de negócio.

🔗 **GitHub:** [Megadurck](https://github.com/Megadurck)

---

*Projeto desenvolvido como parte da trilha Reclame Aqui — Dados e IA na Prática, da DIO.*
