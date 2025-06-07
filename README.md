# Desafio-Dio-Criar-Vm

# 💻 Como Criar uma Máquina Virtual no Microsoft Azure

Este guia foi feito para iniciantes — mesmo que você nunca tenha criado uma VM ou usado o Azure antes.

---

## ✅ Pré-requisitos

- Conta no [Microsoft Azure](https://azure.microsoft.com/)
- Navegador com acesso à internet

---

## 🛠️ Passo a Passo

### 1. Acesse o Portal do Azure
- Acesse: [https://portal.azure.com](https://portal.azure.com)
- Faça login com sua conta Microsoft.

---

### 2. Crie uma nova máquina virtual
1. No menu à esquerda, clique em **"Máquinas Virtuais"**.
2. Clique em **"+ Criar"** > **"Máquina virtual"**.

---

### 3. Preencha as informações básicas

| Campo                | Exemplo ou Valor sugerido             |
|----------------------|----------------------------------------|
| **Assinatura**       | Use a que estiver disponível           |
| **Grupo de recursos**| Crie um novo, ex: `vm-teste-grupo`     |
| **Nome da máquina**  | `vm-teste`                             |
| **Região**           | `Brazil South` ou a mais próxima       |
| **Imagem**           | `Ubuntu 20.04 LTS` (ou `Windows 11`)   |
| **Tamanho**          | `Standard B1s` (baixo custo)           |
| **Usuário**          | Nome de login para a VM                |
| **Senha/Chave SSH**  | Escolha uma forma de autenticação      |

---

### 4. Configurações de disco
- Use a opção padrão (`SSD` ou `HDD`) — escolha o gratuito se estiver disponível.

---

### 5. Configuração de rede
- Deixe a configuração padrão.
- Habilite a **porta 22 (SSH)** para Linux ou **porta 3389 (RDP)** para Windows.

---

### 6. Revisar e criar
- Clique em **"Revisar + criar"**.
- Se tudo estiver certo, clique em **"Criar"**.
- Aguarde o provisionamento.

---

### 7. Acesse sua VM

#### Se for Linux:
1. Copie o **endereço IP público** da VM.
2. No terminal, digite:
   ```bash
   ssh seu_usuario@ip_publico
### Se for Windows:
1. Copie o endereço IP público da VM.
2. Abra o aplicativo Área de Trabalho Remota (RDP).
3. Digite o IP e entre com o usuário e senha definidos.

🧹 Como excluir a VM depois
1. No portal, vá em "Máquinas Virtuais".
2. Selecione sua VM.
3. Clique em "Excluir".

📌 Dicas Finais
1. Desligue a VM quando não estiver usando para evitar cobranças.
2. Monitore o uso em: "Custos e faturamento" no menu do Azure.
3. Evite deixar portas abertas desnecessárias.

