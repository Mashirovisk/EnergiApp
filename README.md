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
- **RF3 – Registro de uso de energia:** Usuário deve poder registrar seu **uso diário de energia (kWh)** através de um formulário na dashboard, informando a **data** e a **quantidade de kWh**. Cada registro deve aparecer imediatamente no histórico e atualizar os gráficos.
- **RF4 – Visualização de gráficos de consumo:** Mostrar **gráficos de consumo diário, semanal e mensal** na dashboard. O gráfico diário mostra o consumo do dia; o semanal mostra a soma/média de cada dia da semana; o mensal mostra o consumo total ou médio por mês. Gráficos atualizam automaticamente quando novos registros são adicionados.
- **RF5 – Alertas de consumo alto:** Exibir alertas visuais na dashboard quando o consumo diário ou semanal ultrapassar a média do usuário. O alerta deve indicar que o consumo está acima do normal e sugerir atenção.
- **RF6 – Histórico de consumo:** Mostrar em uma tabela/lista todos os registros de consumo do usuário, organizados por data. Permitir **filtragem por período** (dia, semana ou mês) para facilitar a visualização.
RF7 – Sugestões de economia:
A dashboard exibirá dicas automáticas de economia de energia baseadas no consumo diário do usuário.

Como vai funcionar:
O sistema analisa o padrão de consumo diário e horários de maior uso.
Quando detectar picos de consumo em certos horários, sugere ao usuário reduzir o uso de eletrodomésticos nesse período.
As dicas não identificam eletrodomésticos específicos, mas usam o horário e o volume de consumo como referência.
As sugestões são atualizadas automaticamente conforme novos registros são adicionados.

Exemplos de dicas:
Evitar ligar muitos aparelhos simultaneamente no horário de pico.
Reduzir uso de aquecimento ou forno em determinados horários.
Monitorar dias com consumo acima da média.

Critério de aceitação:
Usuário vê dicas relevantes e fáceis de entender, atualizadas com base nos registros de consumo.

### 4.2 Requisitos Não Funcionais (RNF)

- **RNF1 – Responsividade:** A aplicação deve funcionar corretamente em **desktop, tablet e smartphone**, mantendo a legibilidade dos gráficos, formulários e alertas na dashboard.

- **RNF2 – Desempenho:** As operações de registro de consumo, geração de gráficos e exibição de alertas devem ser **fluídas e sem travamentos**, garantindo boa experiência ao usuário.

- **RNF3 – Usabilidade:** A interface deve ser **intuitiva**, permitindo que o usuário:
  - Cadastre-se e faça login facilmente;
  - Registre o consumo de energia sem dificuldades;
  - Visualize gráficos de consumo e alertas de forma clara;
  - Entenda e aplique as sugestões de economia.

- **RNF4 – Persistência de dados:** Todos os registros de consumo e histórico de alertas devem ser armazenados no banco de dados e permanecer disponíveis mesmo após logout ou falhas do sistema.

- **RNF5 – Atualização em tempo real:** Gráficos, alertas e sugestões de economia devem ser **atualizados automaticamente** sempre que novos registros de consumo forem adicionados.

- **RNF6 – Segurança básica:** Apesar de não haver criptografia de senhas, o sistema deve **proteger os dados do usuário**, evitando acesso não autorizado a registros de outros usuários.

- **RNF7 – Manutenibilidade:** O código deve ser estruturado de forma modular para facilitar **atualizações futuras**, como inclusão de novos tipos de gráficos, alertas ou funcionalidades.
