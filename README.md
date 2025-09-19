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
- **RF3 – Registro de consumo:** Permitir que o usuário registre **consumo diário de energia (kWh)**.
- **RF4 – Visualização de gráfico diário:** Exibir **gráfico de consumo diário** atualizado automaticamente.
- **RF5 – Visualização de gráfico semanal:** Exibir **gráfico de consumo semanal** mostrando soma ou média diária.
- **RF6 – Visualização de gráfico mensal:** Exibir **gráfico de consumo mensal** mostrando consumo agregado por mês.
- **RF7 – Alertas de consumo alto:** Gerar alertas quando o consumo diário ou semanal estiver acima da média.
- **RF8 – Histórico de consumo:** Permitir que o usuário visualize **todos os registros de consumo** passados, ordenados por data.
- **RF9 – Sugestões de economia:** Fornecer **dicas de economia de energia** com base no consumo registrado.

### 4.2 Requisitos Não Funcionais (RNF)
- **RNF1 – Responsividade:** Aplicação deve funcionar em **desktop, tablet e smartphone**.
- **RNF2 – Desempenho:** Tempo de resposta da aplicação não deve exceder **2 segundos**.
- **RNF3 – Usabilidade:** Interface deve ser **intuitiva e de fácil navegação**.
- **RNF4 – Confiabilidade:** Suportar **múltiplos usuários simultâneos** sem falhas.
