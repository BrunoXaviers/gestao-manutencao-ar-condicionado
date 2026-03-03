# 📄 Documento de Requisitos

## Sistema de Gestão de Ordens de Serviço

---

# Requisitos Funcionais (RF)

Requisitos funcionais descrevem o que o sistema DEVE fazer.

### 👤 Módulo de Clientes

**RF01** – O sistema deve permitir cadastrar clientes.
**RF02** – O sistema deve permitir editar dados do cliente.
**RF03** – O sistema deve permitir excluir clientes.
**RF04** – O sistema deve listar todos os clientes cadastrados.
**RF05** – O sistema deve permitir buscar cliente por nome ou CPF/CNPJ.

---

### 🛠 Módulo de Serviços

**RF06** – O sistema deve permitir cadastrar tipos de serviço.
**RF07** – O sistema deve permitir definir valor padrão para cada serviço.
**RF08** – O sistema deve permitir editar serviços.
**RF09** – O sistema deve permitir listar serviços disponíveis.

---

### 📄 Módulo de Ordens de Serviço

**RF10** – O sistema deve permitir abrir uma nova ordem de serviço.
**RF11** – A ordem deve estar vinculada a um cliente.
**RF12** – A ordem deve conter descrição do problema.
**RF13** – A ordem deve possuir status (Aberta, Em andamento, Finalizada, Cancelada).
**RF14** – O sistema deve permitir alterar o status da ordem.
**RF15** – O sistema deve calcular o valor total da ordem.
**RF16** – O sistema deve listar ordens por status.
**RF17** – O sistema deve permitir visualizar histórico de ordens por cliente.

---

### 🔐 Módulo de Usuários

**RF18** – O sistema deve permitir login com usuário e senha.
**RF19** – O sistema deve diferenciar perfil Administrador e Usuário comum.

---

# Requisitos Não Funcionais (RNF)

Requisitos que definem como o sistema deve se comportar.

**RNF01** – O sistema deve ser desenvolvido em Java utilizando Spring Boot.
**RNF02** – O banco de dados deve ser relacional (MySQL ou PostgreSQL).
**RNF03** – O sistema deve seguir arquitetura REST.
**RNF04** – O sistema deve validar dados obrigatórios.
**RNF05** – O sistema deve possuir tratamento de erros adequado.
**RNF06** – O sistema deve garantir segurança básica com autenticação.

---

# Regras de Negócio (RN)

**RN01** – Uma ordem de serviço não pode ser criada sem cliente vinculado.
**RN02** – Uma ordem finalizada não pode voltar para “Em andamento”.
**RN03** – O valor da ordem deve ser maior que zero.
**RN04** – CPF/CNPJ não pode ser duplicado no cadastro.

---

# Possíveis Funcionalidades Futuras (Melhorias)

* Geração de PDF da ordem
* Envio de ordem por WhatsApp
* Relatório mensal de faturamento
* Dashboard com gráficos
* Controle financeiro completo

---