---
title: Guia de solução de problemas
description: Como solucionar problemas comuns
author: ikhapova
ms.author: ikhapova
ms.date: 08/02/2018
keywords: troubeshooting, problemas, registro, acesso, contas, comentários
ms.openlocfilehash: 3661fe7f9e1f94befd1a1e581e90c477443b25ba
ms.sourcegitcommit: f474af990423033a94fd1c86101453a170523d4b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/23/2018
ms.locfileid: "43054658"
---
# <a name="how-to-troubleshoot-common-issues"></a>Como solucionar problemas comuns
Esta página fornece guias de solução de problemas para problemas comuns.

## <a name="sign-in"></a>Entrar

### <a name="microsoft-account-sign-in"></a>Entrada na conta da Microsoft
Se você não pode entrar no site da Microsoft Collaborate, tente estas sugestões: 
- Certifique-se de que você entrar usando seu endereço de email completo
- verificar o status do serviço de conta da Microsoft
- Certifique-se de que você inseriu sua senha corretamente. As senhas diferenciam maiusculas de minúsculas. Se você tiver esquecido sua senha, vá para a conta da Microsoft [redefinir sua senha](https://account.live.com/password/reset) página.
- Certifique-se de que seu navegador estiver configurado para permitir cookies. Se seu navegador não permitir cookies, você não pode entrar com sua conta da Microsoft.
- Tente limpar o cache do navegador, cookies, arquivos temporários e qualquer outro histórico de navegação que é armazenado. Feche seu navegador, em seguida, abra um sessão de navegação do InPrivate de novo.

### <a name="browser-hangs-or-shows-page-cant-be-displayed-error-when-signing-in-to-dev-center"></a>Navegador de responder ou mostra o erro "a página não pode ser exibida" ao entrar no Centro de desenvolvimento
Depois de indo até o Centro de desenvolvimento/colaborar e inserir seu nome de usuário e senha, você verá um desses problemas ou erros:
- seu navegador parece parar de responder ou parar de responder
- Você receberá um erro "a página não pode ser exibida"
- você receber um erro que diz "ERR_TOO_MANY_REDIRECTS"
- você receber um erro que diz "Humm, não é possível acessar essa página."
- Você aceita um email de convite do Centro de desenvolvimento e você receber esta mensagem:

> Você foi convidado para acessar o aplicativo como.......
> No entanto, não é possível criar esta conta corporativa ou de estudante porque... é um domínio federado com seu local AD.
> Entre em contato com seu administrador para garantir que estão configurados corretamente em suas instalações AD e você pode tentar novamente aceitar este convite.

#### <a name="why-this-is-happening"></a>Por que isso está acontecendo
Há uma boa chance de que isso está acontecendo porque seu endereço de email corporativo está vinculado a uma ID de MSA/Live pessoais (trabalho e contas pessoais compartilham o mesmo nome), que era uma prática comum com contas do Microsoft Connect. Essa prática não é mais suportada pela Microsoft e pode causar vários problemas. Consulte [esta postagem de blog](https://cloudblogs.microsoft.com/enterprisemobility/2016/09/15/cleaning-up-the-azure-ad-and-microsoft-account-overlap/) para obter mais detalhes.

#### <a name="fixesworkarounds"></a>Correções/soluções alternativas
A solução alternativa é renomear sua conta MSA pessoal. Ver [deste artigo](https://support.microsoft.com/en-us/help/11545/microsoft-account-rename-your-personal-account) para obter as etapas detalhadas.

## <a name="registration"></a>Registro

### <a name="account-registration"></a>Registro de conta

> Não foi possível validar sua identidade como um administrador global. Verifique se que você é capaz de entrar com uma conta de administrador global para o locatário do Azure AD que você deseja associar.

O erro indica que um usuário estiver conectado com uma conta de trabalho (AAD) que não tem privilégios de administrador. 

#### <a name="fixesworkarounds"></a>Correções/soluções alternativas
Siga as [instruções](https://docs.microsoft.com/en-us/collaborate/registration) registrar usando Account da Microsoft.

#### <a name="how-to-find-global-administrator-for-your-organization"></a>Como localizar um Administrador Global para sua organização
Localizando **Administrador Global** poderá haver uma tarefa difícil, especialmente se a organização é grande e escritórios estão localizados em vários países. 

##### <a name="using-azure-portal"></a>Usando o **Portal do Azure**:

>[!NOTE]
>
> Você deve entrar com sua conta organizacional para usar **Portal do Azure**. <br>
> Você não poderá usar **Portal do Azure** se sua organização decide restringir o acesso do usuário para não administradores.

1. Navegue até [Portal do Azure](https://portal.azure.com)
2. Selecione [Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Overview) no primeiro menu à esquerda
3. Selecione **funções e Administrtors** no segundo menu à esquerda
4. Encontre **Administrador Global** função na lista e clique para exibir membros

![Funções e os administradores](images/aad-global-admin.png)

Confira estes artigos para saber mais sobre **Administrador Global** função.
* [Noções básicas sobre soluções de identidade do Azure](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/understand-azure-identity-solutions#terms-to-know)
* [Exibir membros e as descrições das funções de administrador no Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/directory-manage-roles-portal)

##### <a name="using-powershell"></a>Usando o PowerShell

>[!NOTE]
>
> Você deve entrar com sua conta organizacional para se conectar ao AD do Azure usando o PowerShell.<br>

1.  Console de lançamento do Windows Powershell como administrador
2.  Se você nunca instalou o módulo do Azure AD para o Powershell, execute este comando <br>

```
    Install-Module AzureAD
```
3.  Execute estes comandos para exibir membros de **Administrador Global** função <br>

```  
    Connect-AzureAD  
    $role = Get-AzureADDirectoryRole | Where-Object {$_.displayName -eq 'Company Administrator'} 
    Get-AzureADDirectoryRoleMember -ObjectId $role.ObjectId | Where-Object {$_.ObjectType -eq 'User'} | Get-AzureADUser 
```

Confira estes artigos para saber mais sobre **PowerShell** e **módulo do Azure AD**.
* [Instalando o Windows PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-windows-powershell?view=powershell-6)
* [Instalando o módulo do AD do Azure ](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0#installing-the-azure-ad-module)

### <a name="invitations"></a>Convites
Se você foi convidado para ingressar o Centro de desenvolvimento, você precisará aceitar o convite antes de poder acessar o portal de colaborar. Se você vir uma mensagem de erro semelhante à mostrada abaixo, significa que você tem duas contas com a Microsoft usando o mesmo endereço de email. 

> Você foi convidado para acessar o aplicativo como.......<br> No entanto, não é possível criar esta conta corporativa ou de estudante porque... é um domínio federado com seu local AD.<br> Entre em contato com seu administrador para garantir que estão configurados corretamente em suas instalações AD e você pode tentar novamente aceitar este convite.<br>

As informações a seguir destina-se para lhe dar informações suficientes para desbloqueá-la.
Microsoft agora é limitar o uso de contas pessoais da Microsoft vinculada a um endereço de email ou de estudante, quando o domínio de email é configurado no Azure AD. Se os usuários tem configurado suas contas de trabalho, como nomes de entrada para a Microsoft conta MSA, em seguida, eles seriam ser impedidos de acessar o Portal de colaboração. Nesse cenário, os usuários terão que renomear sua conta pessoal da Microsoft, seguindo [essas etapas](http://windows.microsoft.com/en-US/Windows/rename-personal-microsoft-account/):

1. Entrar para o [página de informações do seu](https://account.microsoft.com/profile) de sua conta da Microsoft.
2. Selecione **gerenciar como você entra Microsoft**.
3. Veja abaixo os **alias de conta** seção.
  * Se você já tiver um endereço de email pessoal listado lá, você pode ignorar esta etapa.
  * Se sua empresa ou escola de email endereço é o único listado, insira seu endereço de email pessoal, ou obter um novo da Microsoft e selecione **adicionar email** ou **Adicionar número de telefone**.
 4. Se seu endereço de email pessoal não tem **(alias principal)** listado ao lado dele, selecione **tornar primário** para defini-lo como seu alias principal.
 5. Selecione **remover** ao lado de seu endereço de email de trabalho para removê-lo de sua conta.

No futuro, você vai entrar sua conta pessoal da Microsoft com seu endereço de email pessoal. Talvez você precise entrar novamente para alguns aplicativos e dispositivos do Windows.

Após a conclusão prosseguir com a aceitar os convites de colaborar que são enviados de [Invitations Microsoft](mailto:invites@microsoft.com) alias.  Para obter mais informações sobre a capacidade de criar uma nova usando um endereço de email ou de estudante da Microsoft pessoal de bloqueio estão disponíveis neste [artigo](https://cloudblogs.microsoft.com/enterprisemobility/2016/09/15/cleaning-up-the-azure-ad-and-microsoft-account-overlap/).

## <a name="access"></a>Acesso

### <a name="user-cannot-see-packages-andor-engagements-heshe-has-access-to"></a>Usuário não consegue ver os pacotes e/ou contratos que ele tem acesso ao
A maioria dos usuários pertencem a um único locatário do AAD e uma única conta dentro do DevCenter. Os usuários, que existem em vários locatários do AAD e/ou contas no DevCenter, podem precisar para manualmente selecionar locatário do AAD específico e/ou conta para obter acesso aos recursos.

#### <a name="how-to-select-an-aad-tenant"></a>Como selecionar um locatário do AAD
Clique no ícone de notificação no canto superior direito da tela. Você verá uma lista de locatários do AAD disponíveis, se existir em mais de um locatário do AAD. 

#### <a name="how-to-select-specific-account-for-an-aad-tenant"></a>Como selecionar a conta específica para um locatário do AAD
Nome da conta é mostrado no painel de navegação à esquerda, acima da lista de programas disponíveis para esta conta. Clique no nome da conta exibida atualmente para abrir uma lista de contas disponíveis para o locatário do AAD selecionado.

## <a name="distribution-manager"></a>Gerenciador de distribuição
Você pode receber uma mensagem de erro quando você usa o Gerenciador de distribuição. Este artigo contém informações para ajudá-lo a solucionar essas mensagens de erro.

### <a name="cannot-install-application"></a>Não é possível instalar o aplicativo

> Não é possível continuar.  O aplicativo está formatado incorretamente. <br>
> Para obter assistência, entre em contato com o fornecedor do aplicativo. <br>

Esse erro indica que [Microsoft .NET Framework 4.6.1 (x86 x64)](https://www.microsoft.com/en-us/download/details.aspx?id=49981) exigido pelo Gerenciador de distribuição não está instalado no seu computador. Todos os aplicativos ClickOnce exigem que a versão correta do .NET Framework está instalada antes que eles possam ser executados.

Clique no link para instalar [Microsoft .NET Framework 4.6.1 (x86 x64)](https://www.microsoft.com/en-us/download/details.aspx?id=49981).

### <a name="cannot-launch-application"></a>Não é possível iniciar o aplicativo 

> Referência de objeto não definida para uma instância de um objeto. <br>

Você poderá receber esse erro se você atualizou recentemente de uma versão mais antiga do aplicativo.

#### <a name="fixesworkarounds"></a>Correções/soluções alternativas
A solução alternativa é excluir o clique-uma vez os dados de aplicativo.


O caminho exato pode ser determinado pelas seguintes etapas:
1. Pressionar **Ctrl + Alt + Del** no teclado e selecionar o Gerenciador de tarefas
2. Localizar **Microsoft colaborar - Gerenciador de distribuição**
3. Clique com botão direito e selecione **abrir local do arquivo** na lista de opções

![Gerenciador de tarefas](images/TaskManager.png)

4. Você deve levar a uma pasta, como:
> % LOCALAPPDATA%\Apps\2.0\Data\xxxxxxxx.xxx\xxxxxxxx.xxx\dist... tion_xxxxxxxxxxxxxxxx_0000.0000_xxxxxxxxxxxxxxxx\Data

![Pasta do Gerenciador de distribuição](images/DistributionManagerLocation.png)

5. Agora vá para o caminho de dados (% LOCALAPPDATA%\Apps\2.0\Data) e procure uma pasta com o mesmo nome 
> DIST. tion_xxxxxxxxxxxxxxxx_0000.0000_xxxxxxxxxxxxxxxx\Data

![Pasta do Gerenciador de distribuição](images/DistributionManagerDataLocation.png)

6.  Excluir o conteúdo da pasta
7.  Reinicie o aplicativo

