# 🌐 Criação de Instância Gerenciada de SQL no Azure

## 🧩 Objetivo
Documentar o processo de criação de uma Instância Gerenciada de SQL no Azure via portal, aplicando os conceitos aprendidos na prática.

---

## 🛠️ Etapas do Processo

### 1. Acessar o Azure Portal
- Entre em: [https://portal.azure.com](https://portal.azure.com)

### 2. Buscar o Serviço
- No campo de busca, digite: `Instância Gerenciada de SQL`
- Clique em **"Criar"**

### 3. Preencher Informações Básicas
- **Assinatura**: Selecione sua assinatura Azure ativa
- **Grupo de Recursos**: 
  - Crie um novo (ex: `rg-sql-lab`) ou 
  - Utilize um existente
- **Nome da Instância**: 
  - Exemplo: `sqlinstancia-dev`
- **Região**:
  - Escolha a região mais próxima de você (Ex: `Brazil South`)
- **Versão do SQL Server**:
  - Ex: `SQL Server 2019`

### 4. Configurar Recursos da Instância
- **Tamanho e Escalonamento**:
  - Escolha o plano que atenda seu cenário (Exemplo: `8 vCores`, `32GB RAM`)
- **Rede Virtual (VNet)**:
  - Pode ser necessário criar uma nova VNet ou associar a uma existente
  - Certifique-se de permitir o tráfego necessário

### 5. Configurar Administração
- **Usuário administrador**: Defina um nome de usuário (Ex: `adminsql`)
- **Senha**: Crie uma senha forte para acesso ao banco

### 6. Finalizar Criação
- Clique em **"Revisar + Criar"**
- Após a validação, clique em **"Criar"**

---

## 🧪 Pós-Criação
Após a criação ser concluída:
- Acesse a instância criada
- Obtenha o nome do host e credenciais
- Conecte-se via SSMS ou Azure Data Studio para iniciar a configuração do banco de dados

---

## 📂 Sugestão de Repositório GitHub

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/sql-azure-lab.git
cd sql-azure-lab

# Adicione o README.md com a documentação
git add README.md
git commit -m "Adiciona documentação da instância SQL no Azure"
git push origin main
