---
title: Gerenciando usuários do engagement
description: Microsoft Collaborate permite que os usuários de organizações controlar a adição/remoção de usuários para a organização.  Durante a integração, proprietários do Engagement pode atribuir indivíduos de uma organização permissões de usuário avançado.  Usuários avançados só podem gerenciar usuários de sua própria organização.
author: ikhapova
ms.author: ikhapova
ms.date: 12/12/2017
keywords: contratos, adição de usuários, remoção de usuários, gerenciamento de usuários, segurança de colaborar, colaboram permissões, o Centro de desenvolvimento do Microsoft Connect, SysDev bugs, bugs
ms.openlocfilehash: 98d68accdb1279ef4b9d565eb9deeb05e7afcae2
ms.sourcegitcommit: 8ae2ead732e03d8a9865797bb9f40818780036e9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2018
ms.locfileid: "43055129"
---
# <a name="managing-users-in-ms-collaborate"></a>Gerenciamento de usuários em MS colaborar

Usa o sistema Microsoft Collaborate **contratos** para definir as permissões/funções para o portal.  Muito simplesmente, se você for um participante do contrato, consulte os metadados de contrato, conteúdo e os comentários associados ao contrato.  As permissões adicionais dentro do projeto são definidas como funções.  Se você for adicionado a uma função, você pode editar os aspectos específicos do programa/projeto.  Se você não for um membro do contrato, você não vir o contrato ou qualquer um de seus artefatos.

Neste momento, somente os usuários da Microsoft podem gerenciar programas e contratos.  Os usuários não-Microsoft podem ser participantes e usuários avançados.

MS Collaborate tem as seguintes funções de associação:

Função | Escopo das permissões | Descrição
---------------- | ------------------- | ---------------------------------
**participantes** | Contrato | Usuários do conteúdo e os comentários associados ao contrato. Capaz de exibir informações de contrato e a página de aterrissagem do programa de envolvimento faz parte do.  É possível baixar o conteúdo.  É possível exibir, editar itens de trabalho de comentários associados ao contrato.
**Usuário avançado** | Contrato | Administradores de empresa que são capazes de gerenciar os participantes para sua organização.  Uma organização pode ter vários usuários avançados identificado.  Somente os proprietários de programa da Microsoft pode adicionar os usuários avançados e usuários avançados só podem adicionar os participantes.
**Editor do conteúdo** | Contrato | Usuários podem publicar pacotes de conteúdo a serem baixados por participantes da Microsoft.  
**Proprietário do contrato** | Contrato | Microsoft usuários capazes de gerenciar o contrato, incluindo engaement metadados, associação, formulários de comentários e publicar modelos.  Os proprietários do Engagement também herdam a todas as outras permissões de função dentro do engagement, como publicação de pacote e permissões de usuário participante.  
**Gerente de relacionamento** | Programa  | Usuários com permissão para criar compromissos em um programa da Microsoft.  Os proprietários de programa podem adicionar/remover usuários dessa função para o programa.
**Proprietário do programa** | Programa | Usuários da Microsoft que podem gerenciar todos os aspectos do programa e todos os contratos sob o programa.  


## <a name="managing-user-memberships"></a>Gerenciando as associações de usuário

Proprietários de compromisso com o Microsoft configurará os compromissos no MS Collaborate e os usuários serão convidados a participar do contrato.

Adicionar usuários a um contrato requer que cada usuário a ser registrado no Centro de desenvolvimento com qualquer indivíduo ou da conta do Centro de desenvolvimento da empresa.  Se o usuário for um membro de uma empresa ou organização, o administrador do Centro de desenvolvimento precisa adicionar novos usuários à conta da empresa do Centro de desenvolvimento antes que eles podem ser adicionados a uma contratação Collaborate MS. Se a empresa ou organização ainda não existir no Centro de desenvolvimento, um representante da empresa precisa para criar uma nova conta da empresa no Centro de desenvolvimento e identificar um administrador de organização que pode adicionar outros usuários na conta do Centro de desenvolvimento da empresa.  

Ver [registrar com o Microsoft Collaborate](registration.md) para obter mais informações sobre como configurá-lo para usar Collaborate MS.

> [!NOTE]
> MS Collaborate usa a mesma conta do Centro de desenvolvimento como outros programas no Centro de desenvolvimento.  A empresa que você escolher será importante se sua empresa ou organização também serão registrados em programas do Centro de desenvolvimento que exigem contas bancárias ou informações de certificado.  

> Se sua organização usa o Azure Active Directory (AAD) no Centro de desenvolvimento, você precisa integrar os usuários ao centro de desenvolvimento em sua conta do AAD.

> Se você pertencer a várias organizações do Centro de desenvolvimento, você talvez precise alternar sua inscrição para a organização que é integrado ao compromisso do MS Collaborate que você deseja ver.

## <a name="how-to-add-users"></a>Como adicionar usuários

Depois que um usuário está registrado no Centro de desenvolvimento, ele fácil para o MS Collaborate *Engagement proprietários* ou da organização *(s) de energia* para um usuário para um compromisso de adicionar.  Os proprietários do Engagement podem adicionar os usuários avançados para uma organização.  Entre em contato com o MS colaborar proprietário do contrato a ser adicionado como um usuário avançado para a sua organização.

1. Navegue até o Engagement no qual você deseja adicionar ou remover usuários e clique em **Engagement editar** para abrir a página de gerenciamento do Engagement. Como uma organização, o usuário avançado, você só pode alterar as funções de associação para usuários em sua organização.  Todas as outras guias serão somente leitura.

2. Clique no **associação** e selecione o **grupo** que você deseja gerenciar.
    a. Os participantes podem interagir com os artefatos do engagement (comentários, pacotes).
    b. Usuários avançados podem adicionar ou remover usuários da organização.
    c. Observe que *os usuários avançados* precisam ser adicionados explicitamente como *participantes* se o usuário também precisa de acesso ao conteúdo e comentários para o contrato.

    ![Selecione um grupo](images/Membership-tab.PNG)

3.  Clique o **adicionar usuário** ícone na **membros** seção e, em seguida, no **pesquisar usuários** caixa de diálogo, a pesquisa para localizar o (s) que você deseja adicionar ao projeto.

4. Na lista de usuários retornados pela pesquisa, selecione os usuários que você deseja adicionar ao projeto. Você também pode usar **Selecionar tudo**.

    ![Adicionar um usuário](images/add-a-user.PNG)

5. Escolha se você gostaria de ter um email de convite enviado para o usuário com um link para o contrato.

Depois que o usuário é adicionado à lista, o usuário pode começar a acessar o conteúdo do compromisso e comentários.

## <a name="troubleshooting-users-missing-from-search"></a>Solucionando problemas de usuários ausente da pesquisa

Os usuários avançados de uma organização pode pesquisar somente para usuários na conta do Centro de desenvolvimento de sua própria organização.  Proprietários de contrato, se o engagement posicionou a organizações, a pesquisa para que os usuários serão limitada para usuários em organizações nomeados.

Se os usuários não são exibidas nos resultados da pesquisa para seu contrato:
- verificar se os usuários foram adicionados à conta da organização no Centro de desenvolvimento. Se não, trabalhe com a **administrador** da sua conta de organização para adicionar usuários ausentes. Ver [adicionar usuários à sua conta do Centro de desenvolvimento](https://docs.microsoft.com/en-us/windows/uwp/publish/add-users-groups-and-azure-ad-applications#add-users-to-your-dev-center-account) artigo para obter instruções detalhadas.
- É possível que a organização tem mais de uma conta de organização do Centro de desenvolvimento (ID do vendedor) no Centro de desenvolvimento.  Certifique-se de que foi adicionada na organização apropriada do contrato e se os usuários apropriados estão nessa organização.  Se a organização estiver incorreta, entre em contato com o proprietário do seu contrato de Microsoft.
    
## <a name="how-to-remove-users"></a>Como remover usuários

1.  Para remover um usuário, selecione o usuário na **membros** lista e clique no ícone Excluir.
 
    ![Remover um usuário](images/remove-a-user.png)

2.  Confirme que você deseja remover o usuário e o usuário não será um membro do grupo.

Observe que a remoção de um usuário de um contrato não afeta a conta do usuário no sistema de conta do Centro de desenvolvimento.  A conta de usuário permanecerão disponível para outros contratos e outros programas de centro de desenvolvimento.
