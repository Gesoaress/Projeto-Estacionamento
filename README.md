# 📘 Sistema Integrado de Automação de Estacionamento

**Documentação Técnica • Arquitetura • Modelagem • Requisitos •
Protótipo**

Sistema desenvolvido para automatizar completamente o fluxo operacional
de um estacionamento --- desde a entrada do veículo até o pagamento ---
aplicando conceitos de **Engenharia de Requisitos**, **Modelagem de
Processos (Bizagi)** e **Protótipos (Pencil)**.

------------------------------------------------------------------------

# 📌 1. Visão Geral do Sistema

O Sistema Integrado de Automação de Estacionamento visa eliminar
processos manuais por meio de OCR/LPR, painel de vagas, pagamentos
digitais e dashboard gerencial.

------------------------------------------------------------------------

# 🏛 2. Arquitetura do Sistema

### **2.1 Frontend**

-   React ou HTML/CSS/JS\
-   Telas operacionais e administrativas\
-   UI responsiva

### **2.2 Backend (API REST)**

Endpoints principais:

    POST /entrada
    POST /saida
    GET  /vagas
    GET  /dashboard
    POST /pagamento

### **2.3 Integrações**

-   OCR/LPR\
-   Gateways Pix / Cartão\
-   CFTV (opcional)

### **2.4 Banco de Dados**

Tabelas: veículos, entradas_saidas, vagas, mensalistas, pagamentos,
logs, usuários.

------------------------------------------------------------------------

# ⚙️ 3. Funcionalidades Principais

-   Entrada automática\
-   Saída + cálculo automático\
-   Pagamento digital\
-   Mapa de vagas em tempo real\
-   Dashboard e relatórios\
-   Cadastro de clientes/mensalistas\
-   Auditoria

------------------------------------------------------------------------

# 📐 4. Modelagem (Resumo)

### **Fluxo de Entrada**

    [OCR] → [API Entrada] → [DB Entradas] → [Painel]

### **Fluxo de Saída**

    [Cliente] → [Cálculo] → [Pagamento] → [Liberação]

------------------------------------------------------------------------

# 📜 5. Requisitos Funcionais (RF)

-   RF01 Registrar entrada\
-   RF02 Registrar saída\
-   RF03 Atualizar vagas\
-   RF04 Mapa visual\
-   RF05 Cálculo automático\
-   RF06 Pagamento digital\
-   RF07 Recibo digital\
-   RF08 Clientes\
-   RF09 Mensalistas\
-   RF10 Histórico\
-   RF11 Dashboard\
-   RF12 Relatórios\
-   RF13 Permissões\
-   RF14 Busca\
-   RF15 Fotos (opcional)\
-   RF16 Notificações

------------------------------------------------------------------------

# 🛡 6. Requisitos Não Funcionais (RNF)

-   RNF01 Precisão ≥ 95%\
-   RNF02 API ≤ 2s\
-   RNF03 Disponibilidade ≥ 95%\
-   RNF04 LGPD\
-   RNF05 Segurança\
-   RNF06 Logs imutáveis\
-   RNF07 Responsividade\
-   RNF08 Usabilidade\
-   RNF09 Compatibilidade\
-   RNF10 Multiusuário\
-   RNF11 Auditoria

------------------------------------------------------------------------

# 🧩 7. Casos de Uso

-   UC01 Registrar Entrada\
-   UC02 Registrar Saída e Pagamento\
-   UC03 Mapa de Vagas\
-   UC04 Mensalistas\
-   UC05 Dashboard/Relatórios\
-   UC06 Usuários\
-   UC07 Tarifas

------------------------------------------------------------------------

# 🌐 8. Fluxo Operacional

    Entrada → OCR → Vaga → Painel
    Saída   → Cálculo → Pagamento → Liberação

------------------------------------------------------------------------

# 🧪 9. Tecnologias Recomendadas

-   Python / Node.js\
-   React / HTML/CSS\
-   PostgreSQL\
-   Docker\
-   OpenALPR\
-   MercadoPago / Gerencianet

------------------------------------------------------------------------

# 🔗 10. Links

**GitHub:** https://github.com/Gesoaress/Projeto-Estacionamento\
**Trello:** https://trello.com/invite/b/68c206ae45e5bb3d765e37d7

------------------------------------------------------------------------

# 💼 11. Como Contribuir

``` sh
git clone https://github.com/Gesoaress/Projeto-Estacionamento.git
git checkout -b nova-feature
git commit -m "Implementa nova funcionalidade"
git push origin nova-feature
```

------------------------------------------------------------------------

# 🏁 12. Créditos

Baseado na documentação técnica completa da AP2.
