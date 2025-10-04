# Arquitetura do Sistema EcoWatt

## (i) Tecnologias escolhidas
- Frontend: HTML + CSS + JavaScript + Chart.js
- Backend: Node.js + Express
- Banco de Dados: SQLite
- Atualização em tempo real: AJAX + setInterval

## (ii) Projeto arquitetural elaborado
O EcoWatt é um sistema web para monitoramento do consumo de energia residencial. 
Ele possui três camadas principais: Frontend, Backend/API e Banco de Dados.

### Containers
- **Frontend (HTML/CSS/JS + Chart.js):** interface do usuário, dashboards, formulários e gráficos.  
- **Backend (Node.js + Express):** gerencia usuários, registros, alertas e sugestões.  
- **Banco de Dados (SQLite):** armazena usuários, histórico de consumo e alertas.  
- **Atualização de gráficos/alertas:** via AJAX + setInterval, simulando tempo real.

### Componentes do backend
- AuthController: cadastro e login de usuário.  
- ConsumptionController: registro de consumo.  
- AnalyticsService: cálculo de médias, alertas e sugestões.  
- Repository/DB Layer: interface com banco de dados.

### Fluxo principal
1. Usuário registra consumo no frontend.  
2. Backend recebe dados e grava no banco.  
3. Backend calcula alertas e sugestões.  
4. Frontend atualiza gráficos e alertas automaticamente.

### Diagramas C4
#### Nível 1 – Contexto
<img width="311" height="348" alt="image" src="https://github.com/user-attachments/assets/2c2a6c7a-cc93-4b77-a73f-4791f30cb7fc" />


#### Nível 2 – Containers
<img width="1059" height="577" alt="image" src="https://github.com/user-attachments/assets/a1f06f39-b49a-478e-95b2-a60edca65b0d" />


#### Nível 3 – Componentes
<img width="1215" height="764" alt="image" src="https://github.com/user-attachments/assets/87db06f0-99bd-4f1f-9bdf-205c685a82c3" />


#### Nível 4 – Sequência
<img width="1160" height="256" alt="image" src="https://github.com/user-attachments/assets/a0ae7b2f-80cd-4716-9383-91eb6ae5de9f" />


## (iii) Justificativa do modelo escolhido
- **C4 Model:** permite visualizar o sistema em diferentes níveis de detalhe, do contexto ao fluxo de uma funcionalidade, facilitando entendimento para desenvolvedores e revisores.
- **Tecnologias simples:** HTML/CSS/JS + Chart.js, Node.js + Express e SQLite foram escolhidos por serem fáceis de aprender e integrar, garantindo que um iniciante consiga desenvolver e manter o sistema.
- **Separação de camadas:** cada container tem responsabilidade clara, tornando manutenção e futuras atualizações mais simples.
