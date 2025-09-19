# Projeto: EcoWatt – Monitoramento de Consumo de Energia

## 1. Objetivo
Desenvolver uma aplicação web para monitoramento do consumo de energia elétrica residencial, fornecendo gráficos de consumo, alertas e sugestões de economia, promovendo uso consciente da energia (ODS 7).

## 2. Problema a ser resolvido
Muitas residências não possuem controle eficiente do consumo de energia, gerando desperdício, custos elevados e impacto ambiental. O sistema permitirá registrar, monitorar e analisar o consumo de energia, com alertas e sugestões de economia.

## 3. Tipo de solução
Aplicação web full-stack:
- **Front-end:** interface para cadastro, registro de consumo, gráficos e sugestões.
- **Back-end:** API para gerenciar usuários, consumo e gerar alertas/sugestões.
- **Banco de dados:** armazenamento de usuários e histórico de consumo.

## 4. Requisitos da aplicação

### 4.1 Requisitos Funcionais (RF)

- **RF1 – Cadastro de usuário:** Permitir que o usuário se cadastre informando **nome e senha**. Nome deve ser único; mensagem de erro se já existir.

- **RF2 – Login de usuário:** Permitir que o usuário faça login usando **nome e senha**. Login bem-sucedido leva à dashboard; login incorreto mostra mensagem de erro.

- **RF3 – Registro de uso de energia:** Usuário deve poder registrar seu **uso diário de energia (kWh)** através de um formulário na dashboard, informando a **data** e a **quantidade de kWh**. Cada registro deve aparecer imediatamente no histórico e ser usado para atualizar os gráficos.

- **RF4 – Visualização de gráficos de consumo:** Mostrar **gráficos de consumo diário, semanal e mensal** na dashboard. O gráfico diário mostra o consumo do dia; o semanal mostra a soma/média de cada dia da semana; o mensal mostra o consumo total ou médio por mês. Gráficos atualizam quando novos registros são adicionados.

- **RF5 – Alertas de consumo alto:** Exibir alertas visuais na dashboard quando o consumo diário ou semanal ultrapassar a média do usuário. O alerta deve indicar que o consumo está acima do normal e sugerir atenção.

- **RF6 – Histórico de consumo:** Mostrar em uma tabela/lista todos os registros de consumo do usuário, organizados por data. Permitir **filtragem por período** (dia, semana ou mês) para facilitar a visualização.

