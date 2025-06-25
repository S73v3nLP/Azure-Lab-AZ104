## Criação de Infraestrutura Básica para uma Máquina Virtual no AZURE

### CRIANDO UM _RESOURCE GROUP_

  No painel esquerdo do portal, clique em "Resource Group".
  ![ResourceGroup](https://github.com/user-attachments/assets/5dc14d14-8ed8-4909-a5b1-dc79993ac7a9)

  
Na nova janela, clique em "+ Create". 

Preencha os detalhes do grupo de recursos:

• **Subscription**: Selecione a assinatura na qual deseja criar o grupo de recursos.

• **Resource Group Name**: Escolha um nome único para o grupo de recursos. 

• **Region**: Selecione a região geográfica onde deseja hospedar os recursos do grupo. 

Clique em "Review and Create". 
![RG II](https://github.com/user-attachments/assets/fb240d02-52d9-426d-9c36-3ea8c667eea7)

Após revisar os detalhes, clique em "Create". 

### CRIANDO UMA REDE VIRTUAL 
No painel esquerdo do portal, clique em "Redes". 
![NetWrk](https://github.com/user-attachments/assets/0364f0d9-f0b3-4bd8-a164-3e136d87ce78)

Em seguida, clique em "Virtual Network". 

Clique em "+Create" na parte superior da página. 

Preencha os detalhes básicos da rede virtual: 

• **Subscription**: Selecione a assinatura que deseja usar. 

• **Grupo de recursos**: Escolha um grupo de recursos existente ou crie um novo. 

• **Virtual Network Name** : Forneça um nome exclusivo para a sua rede virtual. 

• **Region**: Escolha a região onde deseja criar a rede virtual. 


Na seção "IPv4 Adresses", defina a faixa de endereços IP para a sua rede. Isso é importante para definir a quantidade de endereços IP disponíveis para os recursos que serão conectados à rede virtual. 
![NetWrk II](https://github.com/user-attachments/assets/2ad5c2ce-401a-45b7-8aa0-4f3a699aecc1)
Configure outras opções conforme necessário, como sub-redes, opções de segurança e conectividade. Clique em "Review and Create" e, em seguida, em "Create" para criar a rede virtual. 
  
### CRIANDO UMA MÁQUINA VIRTUAL 
No painel esquerdo do portal, clique em "Virtual Machines". 
![VMs](https://github.com/user-attachments/assets/3493d904-bd6f-4fef-81e9-df4744504674)

Em seguida, clique em "+Create" na parte superior da página. 

-  Configuração Básica 
Selecione a assinatura e o _Resource Group_ onde deseja criar a VM. 
![VMs II](https://github.com/user-attachments/assets/623b7c55-3735-432e-a748-5a8795666006)

Forneça um nome para a VM.

Escolha a região onde a VM será hospedada.

Escolha a versão do Windows ou do Linux que deseja usar. 

Escolha uma imagem de sistema operacional pré-configurada ou uma imagem personalizada.

-  Configuração da Máquina Virtual 

Escolha o tamanho da máquina virtual. Isso determina a quantidade de CPU, memória RAM, 
armazenamento e  desempenho da VM. 
![VMs III](https://github.com/user-attachments/assets/8bb7cdd2-5cca-4da7-aa74-54e87f2cb3a9)

Configure as opções de autenticação: 
 
 Usuário e senha: Forneça um nome de usuário e uma senha para acessar a VM. 
 
 Chave SSH (para VMs Linux): Selecione ou crie uma chave SSH para autenticação. 

Escolha se deseja permitir ou não a conexão de entrada de porta RDP (para VMs Windows) ou SSH (para VMs  Linux). 

- Configuração de Rede 
![VMs IV](https://github.com/user-attachments/assets/482582c6-71ea-495b-9c2c-ac9a83f86d7c)

Escolha uma rede virtual existente ou crie uma nova. 

Escolha uma sub-rede para a VM. 

Configure as opções de IP público, se necessário. 

- Configuração de Discos 

Configure o tipo de disco (HDD ou SSD). 

Escolha um modelo de conta de armazenamento. 

Configure a capacidade do disco. 
![VMs V](https://github.com/user-attachments/assets/291e7b2d-76d4-4fbe-94fe-fca3affb0ca6)

- Revisão e Criação 

Revise todas as configurações da VM e, quando estiver pronto, clique em "Review and Create". 

- Criação da Máquina Virtual 

Após revisar, clique em "Create" para iniciar a criação da VM. O processo pode levar alguns minutos,  dependendo da configuração selecionada. 

- Acesso à Máquina Virtual 

Após a criação, você poderá acessar sua máquina virtual por meio de uma conexão RDP (para Windows) ou  SSH (para Linux) usando as credenciais fornecidas durante a configuração. 

### CRIAÇÃO DE UM RECOVERY SERVICE VAULT 

-  Inicie a Criação do Recovery Services Vault 

No painel esquerdo do portal, clique em "Recovery Services Vault". 

Em seguida, clique em "+Create" na parte superior da página.
![RecoverySV](https://github.com/user-attachments/assets/a5549581-c3e8-46ce-b8b5-f9acaafec7c6)

-  Configuração Básica 

Selecione a assinatura e o grupo de recursos onde deseja criar o Recovery Services Vault. Forneça um nome exclusivo para o Recovery Services Vault. 

Escolha a região onde deseja hospedar o vault. 
-  Configuração de Backup 

Selecione "Backup" como a finalidade do Recovery Services Vault. 

Escolha o tipo de redundância para o vault: armazenamento com redundância local (LRS) ou 
armazenamento  com redundância geográfica (GRS). 
![RecoverySV II](https://github.com/user-attachments/assets/c7727525-baf9-41d2-962b-a672f4090c0e)

Clique em "Review and Create". 

-  Revisão e Criação 

Revise todas as configurações do Recovery Services Vault e clique em "Create" para iniciar o processo de  criação. 

-  Finalizando 

Aguarde alguns minutos até que o Recovery Services Vault seja criado. Depois de criado, você pode configurar  políticas de backup para proteger seus recursos, como máquinas virtuais, bancos de dados e arquivos, no  Azure. 

### CONFIGURANDO POLÍTICAS DE BACKUP 

No portal do Azure, vá para o Recovery Services Vault que você criou. 

Clique em "Backup" no menu esquerdo. 

Clique em "+ Backup" para iniciar o assistente de configuração de backup.

![BK I](https://github.com/user-attachments/assets/e6da76b0-a563-4e9f-9d62-942c1191bd69)

Siga as instruções do assistente para selecionar os recursos que deseja proteger, configurar a frequência de  backup, retenção de backups, entre outras opções. 

Depois de configurar o backup, o Recovery Services Vault começará a proteger seus recursos de acordo com  as configurações especificadas. 

Certifique-se de revisar e ajustar as configurações de backup conforme necessário para atender aos requisitos  de recuperação de desastres e retenção de dados da sua organização. 

### INICIAR BACKUP MANUALMENTE 

• No Recovery Services Vault, selecione 'Backup Items'. 

• Encontre a VM e clique em 'Backup Now'. 
![BK II](https://github.com/user-attachments/assets/2f3ed212-9b2d-47b0-a8b7-f2f4e0b7692e)

• Especifique as configurações de retenção para este backup e inicie o processo. 

### RESTAURAÇÃO DO BACKUP 

• No Recovery Services Vault, vá até 'Restored Items'. 

• Selecione o backup que deseja restaurar. 
• Siga as instruções para iniciar o processo de restauração.
