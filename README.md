# 📘 GeradoDados Pro - Gerador de Dados de Teste

Este projeto é um **gerador de dados sintéticos avançado** para testes em sistemas brasileiros. Ele cria automaticamente dados válidos e diversificados para **Pessoa Física (PF)** e **Pessoa Jurídica (PJ)**, permitindo a cópia individual de cada campo e exportação em massa.

---

## 🚀 Funcionalidades
- **Geração Diversificada:**
  - **PF:** Nome completo (combinações reais), CPF válido, RG aleatório e E-mail dinâmico.
  - **PJ:** Razão Social, Nome Fantasia, CNPJ válido, Inscrição Estadual (IE) e E-mail corporativo.
- **Endereço Detalhado:**
  - CEP, Logradouro, Número, Bairro, Cidade e UF.
  - Possibilidade de copiar cada componente do endereço individualmente para sistemas sem busca automática por CEP.
- **Produtividade:**
  - **Geração em Massa:** Gere de 1 a 50 registros simultaneamente.
  - **Exportação:** Baixe os dados gerados em formatos **JSON** ou **CSV**.
  - **Histórico Local:** Acesso rápido às últimas 5 gerações realizadas.
- **Interface Moderna:**
  - Layout responsivo e limpo.
  - **Modo Escuro/Claro** com persistência de preferência.
  - Feedback visual via **Toast** ao copiar campos.

---

## 📂 Estrutura e Lógica
- `index.html` → Interface única com toda a lógica integrada.
- **Principais Funções JavaScript:**
  - `getCPF()` / `getCNPJ()` → Algoritmos de geração com cálculo de dígitos verificadores.
  - `generateEmail(nome)` → Cria e-mails baseados no nome gerado, removendo acentos e espaços.
  - `generateBatch()` → Orquestra a geração de múltiplos registros e atualiza a interface.
  - `exportData(format)` → Converte os dados atuais para o formato desejado e inicia o download.
  - `copy(txt)` → Copia o valor para a área de transferência com feedback visual.

---

## ⚙️ Como usar
1. Abra o arquivo `index.html` em qualquer navegador moderno.
2. Escolha entre **Pessoa Física** ou **Pessoa Jurídica** na barra lateral.
3. Defina a **Quantidade** de registros no painel superior.
4. Clique em **⚡ GERAR DADOS**.
5. Clique em qualquer campo (Nome, CPF, Logradouro, etc.) para **copiar** o valor instantaneamente.
6. Use os botões de **Exportar** para salvar os dados em sua máquina.

---

## 📡 Tecnologias Utilizadas
- **HTML5 & CSS3:** Layout moderno utilizando CSS Grid e Flexbox (sem dependências externas pesadas).
- **JavaScript Vanilla:** Lógica pura para máxima performance e portabilidade.
- **LocalStorage API:** Para persistência de tema e histórico de geração.

---

## 📜 Licença
Este projeto é livre para uso em testes, homologação e aprendizado.  
> **Aviso:** Os dados gerados são sintéticos e destinados exclusivamente a ambientes de desenvolvimento.
