---
title: Registre-se com MS colaborar
description: MS Collaborate utiliza o painel da Central de desenvolvedores que exigem uma conta da Microsoft individuais (MSA) ou uma organização com o Azure Active Directory configurada.
author: ikhapova
ms.author: ikhapova
ms.date: 12/12/2017
keywords: acesso de parceiros, permissões, registrar, registro, integração, comentários de parceiros, downloads de compilação, especificações do download, bugs, Microsoft Connect, SysDev bugs, bugs de centro de desenvolvimento
ms.openlocfilehash: 49bfb7ffd58719a61146b6c67f333481e55df44d
ms.sourcegitcommit: 7fd7eb31172da66cd9c7588fe0ee0d5c2068f02b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2018
ms.locfileid: "47454176"
---
# <a name="register-with-microsoft-collaborate"></a>Registre-se com a Microsoft colaboram

O programa Microsoft Collaborate exige registro. Se você tiver uma conta no Centro de desenvolvimento, você pode usá-lo para fazer logon e interagir com colaborar. Antes de baixar o conteúdo ou enviar comentários, você precisará ingressar um compromisso. Alguns compromissos exigem convite da Microsoft **proprietário do contrato** ou **usuário avançado** (quando sua organização já foi adicionada a um compromisso). Outros contratos são **abrir** para os usuários ingressar.

## <a name="the-account-signup-process"></a>O processo de inscrição de conta

1.  Navegue até a [ https://aka.ms/collaborate ](https://aka.ms/collaborate) página. 
2.  Se você ainda não entrou com uma conta da Microsoft, inscreva-se agora ou criar uma nova conta da Microsoft. Conta da Microsoft que você usa aqui será o que você usa para entrar Microsoft Collaborate.
3.  Se você não está registrados no Microsoft Collaborate o sistema automaticamente o redirecionará para o [página de registro](https://go.microsoft.com/fwlink/?linkid=851519).
4.  Selecione o país/região em que você mora ou onde sua empresa está localizada. Você não poderá alterar isso mais tarde.
5.  Selecione o tipo de conta (individuais ou empresa). Você não poderá alterá-lo mais tarde, portanto, certifique-se de escolher o tipo correto de conta.
6.  Insira o **nome de exibição do publicador** que você deseja usar (50 caracteres ou menos). Selecione esta opção com cuidado, pois esse nome será usado quando você interage com colaborar (baixar o conteúdo, enviar comentários e etc.). Para contas da empresa, certifique-se de usar o nome de negócios registrado ou o nome da sua organização. Observe que, se você inserir um nome que outra pessoa já selecionado, ou se parece que outra pessoa tem os direitos para usar esse nome, podemos não permitirá que você use esse nome. 

  > [!NOTE]
  > Verifique se que você tem os direitos para usar o nome inserido aqui. Se outra pessoa tem com a marca registrada ou protegidos por direitos autorais o nome escolhido por você, sua conta foi fechada. Se alguém está usando um nome de exibição do publicador para o qual você mantenha a marca comercial ou outro direito legal, [entre em contato com o Microsoft](http://go.microsoft.com/fwlink/p/?LinkId=233777).    

7.  Insira as informações de contato que você deseja usar para sua conta.

  > [!NOTE]
  > Vamos usar essas informações para contatar você sobre assuntos relacionados à conta. Por exemplo, você receberá uma mensagem de confirmação de email depois de concluir seu registro.

   Se você estiver registrando como uma empresa, também precisará inserir o nome, endereço de email e número de telefone da pessoa que aprovará conta da sua empresa.

8.  Analise suas informações de conta e confirme que tudo está correto. Em seguida, leia e aceite os termos e condições de [colaborar contrato](https://go.microsoft.com/fwlink/?linkid=849107). Marque a caixa para indicar que você leu e aceitou os termos.

9.  Clique em **concluir** para confirmar seu registro.  

## <a name="additional-guidelines-for-company-accounts"></a>Diretrizes adicionais para contas da empresa

Ao criar uma conta da empresa, sugerimos que você siga essas diretrizes, especialmente se mais de uma pessoa precisar acessar a conta.

> [!IMPORTANT]
> Para permitir que vários usuários acessem sua conta do Centro de desenvolvimento, é recomendável usar o Azure Active Directory para atribuir funções a usuários individuais. Cada usuário pode acessar a conta do Centro de desenvolvimento ao entrar com sua pessoa credenciais do Azure AD. Para obter mais informações, consulte [gerenciar usuários de conta](/windows/uwp/publish/manage-account-users).

-   Criar sua conta da Microsoft usando um endereço de email que já não pertence a você ou outra pessoa, como MyCompany_DevCenter@outlook.com. Você pode não ser capaz de usar um endereço de email no domínio da sua empresa, especialmente se sua empresa já usa o Azure AD.
-   Se você planeja participe do programa do Windows para desenvolvimento de aplicativos no futuro e quiser reutilizar sua conta do Centro de desenvolvimento, em seguida, é recomendável que você deseja registrar no programa Windows primeiro e, em seguida, ingressar Collaborate Microsoft. Caso contrário, você terá que criar contas separadas para esses programas.
-   Adicione um número de telefone da empresa que não requer uma extensão e está acessível aos membros da equipe de chave.

## <a name="how-to-associate-your-dev-center-account-with-azure-active-directory-and-manage-users"></a>Como associar seu centro de desenvolvimento de conta com o Azure Active Directory e gerenciar usuários

Você pode usar o Azure Active Directory para adicionar e gerenciar usuários adicionais na sua conta do Centro de desenvolvimento. Você pode definir a função ou permissões personalizadas que cada usuário deve ter. 

Você primeiro deve associar sua conta do Centro de desenvolvimento da sua organização Active Directory do Azure para ser capaz de adicionar e gerenciar usuários. 

Esta seção descreve como fazer o seguinte:

-   [Associar o Active Directory do Azure à sua conta do Centro de desenvolvimento](/windows/uwp/publish/associate-azure-ad-with-dev-center)
-   [Adicionar usuários, grupos e aplicativos do Azure AD à sua conta do Centro de desenvolvimento](/windows/uwp/publish/add-users-groups-and-azure-ad-applications)
-   [Definir funções e permissões personalizadas para usuários de conta](/windows/uwp/publish/set-custom-permissions-for-account-users)

> [!TIP]
> Centro de desenvolvimento aproveita o Azure Active Directory para gerenciamento de vários usuários e a atribuição de funções. Se sua organização já usa o Office 365 ou outros serviços comerciais da Microsoft, você já tiver um AAD. Caso contrário, você pode criar um novo locatário do AAD no Centro de desenvolvimento sem nenhum custo adicional.

## <a name="how-to-log-in-to-the-ms-collaborate-portal"></a>Como fazer logon no portal do MS Collaborate

1. Navegue até MS colaborar: [ https://aka.ms/collaborate ](https://aka.ms/collaborate).

2.  Você será solicitado para credenciais para fazer logon. Isso é que suas credenciais de conta do Centro de desenvolvimento. Se você tiver mais de uma conta, selecione a conta apropriada que você usou para inscrever-se no Centro de desenvolvimento. Isso pode ser uma conta de alias da Microsoft (MSA) ou uma conta de organização do Active Directory. Se você não tiver conectado antes, você precisará inserir sua senha.

3. Depois de fazer logon, o painel Collaborate Microsoft será exibida, mostrando os contratos, pacotes e comentários, você estiver configurado para ver. Se você não for um membro de todos os programas ou contratos, as listas ficará em branco. Você precisa ser adicionado a um contrato para interagir com o conteúdo ou comentários. 

