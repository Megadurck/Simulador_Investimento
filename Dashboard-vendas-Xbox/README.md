# 🎮 Dashboard de Assinaturas — Xbox Game Pass

Projeto de análise de dados desenvolvido durante o Bootcamp **Análise de Dados no Excel com IA**, realizado pela [DIO](https://www.dio.me/) em parceria com o **Reclame Aqui**.

O objetivo é explorar uma base de dados de assinaturas do Xbox Game Pass, organizar informações comerciais e utilizar recursos do Microsoft Excel para construir análises e indicadores que auxiliem na interpretação dos dados.

## 🎯 Objetivo do Projeto

Analisar os registros de assinaturas do Xbox Game Pass, observando aspectos como:

- Distribuição dos assinantes por plano.
- Tipos e periodicidade das assinaturas.
- Adesão à renovação automática.
- Contratação dos adicionais EA Play e Minecraft.
- Aplicação de cupons e seus impactos no valor total.
- Distribuição dos valores registrados nas assinaturas.

## 📁 Estrutura da Planilha

O arquivo `base-xbox.xlsx` contém quatro abas:

| Aba | Finalidade |
|---|---|
| Assets | Elementos visuais, logos, ícones e paleta de cores. |
| Bases | Base principal com os registros de assinaturas. |
| Cálculos | Resumos e tabelas de apoio às análises. |
| Dashboard | Apresentação visual dos indicadores e gráficos. |

As abas de apoio e processamento estão ocultas na pasta de trabalho. A aba Dashboard é a área visual apresentada ao usuário.

## 📊 Base de Dados

A tabela principal contém **295 registros de assinaturas** e 13 colunas.

| Campo | Descrição |
|---|---|
| Subscriber ID | Identificador do assinante. |
| Name | Nome associado ao registro. |
| Plan | Plano contratado: Core, Standard ou Ultimate. |
| Start Date | Data de início da assinatura. |
| Auto Renewal | Indicação de renovação automática. |
| Subscription Price | Preço da assinatura. |
| Subscription Type | Periodicidade: Monthly, Quarterly ou Annual. |
| EA Play Season Pass | Indicação de contratação do adicional EA Play. |
| EA Play Season Pass Price | Preço do adicional EA Play. |
| Minecraft Season Pass | Indicação de contratação do adicional Minecraft. |
| Minecraft Season Pass Price | Preço do adicional Minecraft. |
| Coupon Value | Valor do cupom aplicado. |
| Total Value | Valor total registrado para a assinatura. |

**Período dos registros:** 01/01/2024 a 16/12/2024.

## 🔎 Principais Informações Identificadas

### Distribuição por plano

| Plano | Registros |
|---|---:|
| Core | 101 |
| Ultimate | 98 |
| Standard | 96 |
| **Total** | **295** |

### Tipo de assinatura

| Periodicidade | Registros |
|---|---:|
| Monthly | 139 |
| Quarterly | 85 |
| Annual | 71 |
| **Total** | **295** |

### Renovação automática

| Renovação | Registros |
|---|---:|
| Yes | 148 |
| No | 147 |

### Adicionais

| Adicional | Contratado | Não contratado |
|---|---:|---:|
| EA Play | 98 | 197 |
| Minecraft | 194 | 101 |

Esses números permitem observar a distribuição dos registros e comparar o comportamento das diferentes categorias.

## 💡 Possibilidades de Análise

A estrutura dos dados permite desenvolver análises como:

- Comparação do valor total por plano.
- Participação de cada periodicidade nas assinaturas.
- Relação entre plano contratado e renovação automática.
- Adesão aos adicionais EA Play e Minecraft.
- Impacto dos cupons sobre o valor total.
- Distribuição das assinaturas por período de início.
- Comparação de indicadores entre diferentes categorias.

## 🧮 Regra de Cálculo do Valor Total

A base apresenta uma composição de valor que considera o preço da assinatura, os adicionais contratados e os descontos aplicados:

`Total Value = Subscription Price + EA Play Season Pass Price + Minecraft Season Pass Price - Coupon Value`

Os registros analisados seguem essa regra, considerando a ausência de contratação do EA Play como preço zero.

## ⚠️ Limitações dos Dados

A análise precisa respeitar o que a base efetivamente disponibiliza.

Não existem campos de cancelamento, histórico de pagamentos, utilização do serviço ou eventos efetivos de renovação.

Por isso, não é possível determinar diretamente indicadores como churn, retenção efetiva, utilização do serviço ou receita recorrente mensal.

A soma de `Total Value` representa os valores registrados na base, não necessariamente a receita mensal recorrente do negócio.

Também não há informação suficiente para afirmar se os registros são reais ou sintéticos.

## 🛠️ Ferramentas e Recursos

- Microsoft Excel.
- Organização e análise de dados.
- Fórmulas e funções.
- Tabelas e tabelas dinâmicas.
- Gráficos e dashboards.
- Inteligência Artificial como apoio à análise de dados.

## 📚 Contexto Educacional

Este projeto faz parte das atividades práticas do Bootcamp **Análise de Dados no Excel com IA — DIO + Reclame Aqui**.

A proposta é desenvolver a capacidade de transformar dados estruturados em informações compreensíveis, identificar padrões e construir análises que possam apoiar decisões.

---

**Autor:** Romário Pereira Rezende

[GitHub — Megadurck](https://github.com/Megadurck)