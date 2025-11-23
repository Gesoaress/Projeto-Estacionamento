📘 Sistema Integrado de Automação de Estacionamento

Documentação Técnica • Arquitetura • Requisitos • Modelagem

📌 Visão Geral do Sistema

O Sistema Integrado de Automação de Estacionamento é uma solução
completa para controle digital de entrada e saída de veículos, cobrança
automática e monitoramento de vagas em tempo real. Substitui processos
manuais com OCR/LPR, pagamentos digitais, dashboard e logs estruturados.

------------------------------------------------------------------------

🏛 Arquitetura do Sistema

1. Frontend

-   HTML/CSS/JS ou React
-   Painel, dashboard, gestão e telas operacionais

2. Backend (API REST)

-   Controle de entrada/saída
-   Regras de negócio
-   Pagamentos
-   Integrações
-   Endpoints principais:

    POST /entrada
    POST /saida
    GET /vagas
    GET /dashboard
    POST /pagamento

3. Integrações

-   OCR/LPR
-   Gateways de pagamento
-   Banco de dados relacional

4. Banco de Dados

Tabelas: veículos, entradas_saidas, vagas, mensalistas, pagamentos,
logs, usuários.

------------------------------------------------------------------------

⚙️ Funcionalidades Principais

-   Entrada e saída automatizada
-   Pagamento digital
-   Painel de vagas
-   Dashboard
-   Cadastros
-   Logs e auditoria

------------------------------------------------------------------------

📐 Modelagem

    [OCR] → [API Entrada] → [DB Entradas] → [Painel]

    [Cliente] → [Saída] → [Pagamento] → [DB Pagamentos]

------------------------------------------------------------------------

📜 Requisitos Funcionais (RF)

-   RF01 Registrar entrada
-   RF02 Registrar saída
-   RF03 Atualizar vagas
-   RF04 Mapa visual
-   RF05 Calcular tarifa
-   RF06 Pagamento digital
-   RF07 Recibo
-   RF08 Clientes
-   RF09 Mensalistas
-   RF10 Histórico
-   RF11 Dashboard
-   RF12 Relatórios
-   RF13 Permissões
-   RF14 Busca
-   RF15 Fotos (opcional)
-   RF16 Notificações

------------------------------------------------------------------------

🛡 Requisitos Não Funcionais (RNF)

-   RNF01 Precisão ≥ 95%
-   RNF02 API ≤ 2s
-   RNF03 Disponibilidade ≥ 95%
-   RNF04 LGPD
-   RNF05 Segurança
-   RNF06 Logs imutáveis
-   RNF07 Responsividade
-   RNF08 Usabilidade
-   RNF09 Compatibilidade
-   RNF10 Multiusuário
-   RNF11 Auditoria

------------------------------------------------------------------------

🧩 Casos de Uso Resumidos

-   UC01 Registrar Entrada
-   UC02 Registrar Saída
-   UC03 Gerenciar Vagas
-   UC04 Mensalistas
-   UC05 Dashboard
-   UC06 Usuários
-   UC07 Tarifas

------------------------------------------------------------------------

🌐 Fluxo Operacional

    Entrada → OCR → Vaga → Painel
    Saída → Cálculo → Pagamento → Liberação

------------------------------------------------------------------------

🧪 Tecnologias Recomendadas

-   Python / Node.js
-   React / HTML/CSS/JS
-   PostgreSQL
-   Docker
-   OpenALPR
-   MercadoPago/Gerencianet

------------------------------------------------------------------------

🔗 Links

Repositório GitHub: https://github.com/Gesoaress/Projeto-Estacionamento
Trello:
https://trello.com/invite/b/68c206ae45e5bb3d765e37d7/ATTIb8dff2ad5b0f4c0404f24610fde3294a27C54CE9/projeto-estacionamento

------------------------------------------------------------------------

💼 Como Contribuir

    git clone https://github.com/Gesoaress/Projeto-Estacionamento.git
    
