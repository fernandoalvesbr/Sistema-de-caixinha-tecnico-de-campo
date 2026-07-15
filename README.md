# 💰 Sistema de Controle de Caixinha por Períodos

Um sistema desenvolvido em **PHP** com armazenamento em **JSON**, criado para controlar a movimentação financeira de equipes técnicas.

Foi desenvolvido para funcionar em hospedagens compartilhadas, sem necessidade de banco de dados.

---

## ✨ Recursos

- 🔐 Login com autenticação
- 👥 Controle de usuários
- 📅 Controle por períodos
- 💰 Registro de entregas
- 🧾 Registro de gastos
- 🚇 Cadastro de transportes
- ⚡ Cálculo automático de passagens
- 👨‍🔧 Cadastro de técnicos
- 📊 Gráficos
- 📈 Comparativos históricos
- 📤 Exportação para Excel (CSV)
- 🖨️ Impressão de relatórios
- 💾 Backup em ZIP
- 🌙 Tema claro/escuro
- 📋 Auditoria de alterações
- 📂 Armazenamento em JSON

---

## 🚀 Tecnologias

- PHP
- Bootstrap 5
- Chart.js
- JSON

**Não utiliza MySQL nem SQLite.**

---

## ✅ Compatibilidade

- PHP 5.x
- PHP 7.x
- PHP 8.x

Compatível com praticamente qualquer hospedagem compartilhada.

---

## 📁 Estrutura

```text
index.php
caixinha_dados.json
backup_historico_*.json
```

---

## 🔑 Primeiro acesso

O sistema cria automaticamente o usuário administrador.

**Usuário**

```text
admin
```

**Senha**

```text
admin
```

> Recomenda-se alterar a senha após o primeiro acesso.

---

## 👥 Níveis de acesso

### 👑 Administrador

Permissões:

- Criar usuários
- Excluir usuários
- Criar períodos
- Renomear períodos
- Excluir períodos
- Alterar caixa inicial
- Registrar entregas
- Registrar gastos
- Editar lançamentos
- Excluir lançamentos
- Cadastrar técnicos
- Excluir técnicos
- Ocultar técnicos dos gráficos
- Cadastrar transportes
- Excluir transportes
- Exportar relatórios
- Gerar backup

---

### 👁️ Visualizador

Permissões:

- Consultar dados
- Filtrar registros
- Visualizar gráficos
- Exportar CSV
- Imprimir relatórios
- Alterar a própria senha

Não pode modificar dados do sistema.

---

## 📅 Controle por períodos

Cada período possui:

- Caixa próprio
- Histórico independente
- Relatórios próprios
- Saldo individual

Ao criar um novo período o sistema transporta automaticamente os saldos pendentes dos técnicos.

---

## 💵 Registro de movimentações

Cada lançamento armazena:

- Data
- Horário
- Técnico
- Tipo
- Valor
- Observação
- Usuário que criou
- Usuário que editou

Todas as alterações ficam registradas para auditoria.

---

## 🚇 Transporte automático

Caso a observação contenha transportes entre parênteses, o sistema calcula automaticamente o valor.

Exemplo:

```text
Empresa > Cliente (ônibus metrô) > Empresa
```

O cálculo utiliza os valores cadastrados pelo administrador.

---

## 📊 Indicadores

O painel apresenta:

- Caixa do período
- Total gasto
- Total entregue aos técnicos
- Total com os técnicos
- Valor para devolução
- Saldo do caixa

Todos os indicadores são atualizados automaticamente.

---

## 📈 Relatórios

O sistema permite:

- Impressão da prestação de contas
- Impressão com gráficos
- Exportação para Excel (CSV)
- Comparativo entre períodos
- Histórico financeiro

---

## 💾 Backup

O backup gera um arquivo ZIP contendo todos os arquivos JSON do sistema.

A restauração pode ser feita substituindo os arquivos JSON pelos arquivos do backup.

---

## 🔒 Segurança

- Login obrigatório
- Sessões PHP
- Controle de permissões
- Auditoria de usuários
- Alteração individual de senha
- Proteção das funções administrativas

---

## 🎯 Objetivo

Facilitar o controle financeiro de equipes técnicas responsáveis por despesas operacionais, transporte e deslocamentos.

O projeto foi desenvolvido para ser:

- Simples
- Leve
- Rápido
- Portátil
- Fácil de instalar

---

## 📄 Licença

Projeto disponibilizado gratuitamente.

Caso utilize ou modifique este sistema, os créditos são sempre bem-vindos.

---

## 👨‍💻 Desenvolvedor

**Fernando Ferreira Alves**
