CRIANDO UM GRUPO DE RECURSOS 
No painel esquerdo do portal, clique em "Grupos de recursos". 
Na nova janela, clique em "+ Adicionar". 

Preencha os detalhes do grupo de recursos: 
• Assinatura: Selecione a assinatura na qual deseja criar o grupo de recursos. • Grupo de recursos: Escolha um nome único para o grupo de recursos. 
• Região: Selecione a região geográfica onde deseja hospedar os recursos do grupo. Clique em "Revisar + criar". 
Após revisar os detalhes, clique em "Criar". 

CRIANDO UMA REDE VIRTUAL 
No painel esquerdo do portal, clique em "Redes". 

Em seguida, clique em "Redes virtuais". 
Clique em "+ Adicionar" na parte superior da página. 
Preencha os detalhes básicos da rede virtual: 
• Assinatura: Selecione a assinatura que deseja usar. 
• Grupo de recursos: Escolha um grupo de recursos existente ou crie um novo. • Nome da rede virtual: Forneça um nome exclusivo para a sua rede virtual. 
• Região: Escolha a região onde deseja criar a rede virtual. 
Na seção "Faixa de endereços IPv4", defina a faixa de endereços IP para a sua rede. Isso é importante para definir a quantidade de endereços IP disponíveis para os recursos que serão conectados à rede virtual. 

Configure outras opções conforme necessário, como sub-redes, opções de segurança e conectividade. Clique em "Revisar + criar" e, em seguida, em "Criar" para criar a rede virtual. 
  
CRIANDO UMA MÁQUINA VIRTUAL 
No painel esquerdo do portal, clique em "Máquinas Virtuais". 

Em seguida, clique em "+ Adicionar" na parte superior da página. 
Passo 3: Configuração Básica 
Selecione a assinatura e o grupo de recursos onde deseja criar a VM. 

Forneça um nome para a VM. 
Escolha a região onde a VM será hospedada. 
Escolha a versão do Windows ou do Linux que deseja usar. 
Escolha uma imagem de sistema operacional pré-configurada ou uma imagem personalizada.
Passo 4: Configuração da Máquina Virtual 
Escolha o tamanho da máquina virtual. Isso determina a quantidade de CPU, memória RAM, 
armazenamento e  desempenho da VM. 

Configure as opções de autenticação: 
 Usuário e senha: Forneça um nome de usuário e uma senha para acessar a VM. 
 Chave SSH (para VMs Linux): Selecione ou crie uma chave SSH para autenticação. 
Escolha se deseja permitir ou não a conexão de entrada de porta RDP (para VMs Windows) ou SSH (para VMs  Linux). 
Passo 5: Configuração de Rede 

Escolha uma rede virtual existente ou crie uma nova. 
Escolha uma sub-rede para a VM. 
Configure as opções de IP público, se necessário. 
Passo 6: Configuração de Discos 
Configure o tipo de disco (HDD ou SSD). 
Escolha um modelo de conta de armazenamento. 
Configure a capacidade do disco. 

Passo 7: Revisão e Criação 
Revise todas as configurações da VM e, quando estiver pronto, clique em "Revisar + criar". 
Passo 8: Criação da Máquina Virtual 
Após revisar, clique em "Criar" para iniciar a criação da VM. O processo pode levar alguns minutos,  dependendo da configuração selecionada. 
Passo 10: Acesso à Máquina Virtual 
Após a criação, você poderá acessar sua máquina virtual por meio de uma conexão RDP (para Windows) ou  SSH (para Linux) usando as credenciais fornecidas durante a configuração. 
CRIAÇÃO DE UM RECOVERY SERVICE VAULT 
Passo 1: Inicie a Criação do Recovery Services Vault 
No painel esquerdo do portal, clique em "Recuperação de Serviços". 
Em seguida, clique em "+ Adicionar" na parte superior da página.

Passo 2: Configuração Básica 
Selecione a assinatura e o grupo de recursos onde deseja criar o Recovery Services Vault. Forneça um nome exclusivo para o Recovery Services Vault. 
Escolha a região onde deseja hospedar o vault. 
Passo 3: Configuração de Backup 
Selecione "Backup" como a finalidade do Recovery Services Vault. 
Escolha o tipo de redundância para o vault: armazenamento com redundância local (LRS) ou 
armazenamento  com redundância geográfica (GRS). 

Clique em "Revisar + criar". 
Passo 4: Revisão e Criação 
Revise todas as configurações do Recovery Services Vault e clique em "Criar" para iniciar o processo de  criação. 
Passo 5: Conclusão 
Aguarde alguns minutos até que o Recovery Services Vault seja criado. Depois de criado, você pode configurar  políticas de backup para proteger seus recursos, como máquinas virtuais, bancos de dados e arquivos, no  Azure. 
CONFIGURANDO POLÍTICAS DE BACKUP 
No portal do Azure, vá para o Recovery Services Vault que você criou. 
Clique em "Backup" no menu esquerdo. 
Clique em "+ Backup" para iniciar o assistente de configuração de backup.


Siga as instruções do assistente para selecionar os recursos que deseja proteger, configurar a frequência de  backup, retenção de backups, entre outras opções. 
Depois de configurar o backup, o Recovery Services Vault começará a proteger seus recursos de acordo com  as configurações especificadas. 
Certifique-se de revisar e ajustar as configurações de backup conforme necessário para atender aos requisitos  de recuperação de desastres e retenção de dados da sua organização. 
INICIAR BACKUP MANUALMENTE 
• No Recovery Services Vault, selecione 'Backup Items'. 
• Encontre a VM e clique em 'Backup Now'. 

• Especifique as configurações de retenção para este backup e inicie o processo. 
RESTAURAÇÃO DO BACKUP 
• No Recovery Services Vault, vá até 'Restored Items'. 
• Selecione o backup que deseja restaurar. 
• Siga as instruções para iniciar o processo de restauração.