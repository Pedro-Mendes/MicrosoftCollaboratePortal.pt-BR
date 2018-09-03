---
title: Trabalhando com itens de trabalho de comentários
description: Itens de comentários à Microsoft colaborar podem ser bugs, solicitações de recursos ou todas as tarefas associadas com um contrato. Formulários de comentários podem ser personalizados com base em cada contrato.
author: ikhapova
ms.author: ikhapova
ms.date: 12/12/2017
keywords: comentários, contratos, itens de trabalho, bugs, solicitações de recursos, permissões colaborar, Microsoft Connect, SysDev bugs, bugs de centro de desenvolvimento
ms.openlocfilehash: 3dc28bda45c7209688188442928b1777a8ac3a84
ms.sourcegitcommit: 8ae2ead732e03d8a9865797bb9f40818780036e9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2018
ms.locfileid: "43055092"
---
# <a name="feedback"></a>Comentários

## <a name="overview"></a>Visão geral
O [Hub de comentários](https://support.microsoft.com/en-us/help/4021566/windows-10-send-feedback-to-microsoft-with-feedback-hub-app) é um mecanismo comum para enviar bugs, problemas e sugestões à Microsoft.  Para organizações que estão colaborando com a Microsoft, MS Collaborate fornece funcionalidade adicional que permite que organizações e os usuários colaborem em itens de trabalho de comentários. Comentários podem ser configurado de maneiras diferentes para habilitar a funcionalidade necessária para dar suporte à colaboração cada específica.  

Os comentários de colaborar MS "itens de trabalho" são normalmente bugs e solicitações de recursos que você enviar à Microsoft, mas os itens de trabalho podem ser qualquer tipo de dados que podem ser compartilhados em um formulário (por exemplo, pesquisas, incidentes, etc.). Cada proprietário do contrato MS colaborar define as formas de comentários e como os dados são sincronizados para um sistema de engenharia de equipe interno do Microsoft (como VSTS). Os proprietários do Engagement também configurar o roteamento para sistemas internos para garantir que seus comentários cheguem às equipes de recursos à direita.

Além de usar o portal Collaborate MS, algumas organizações optam por integrar o sistema Collaborate MS em seu próprio sistema de engenharia interno protegida pelo firewall do parceiro de engenharia conjunta. Isso permite que os engenheiros da organização parceira trabalhar em seu próprio sistema ao compartilhamento de dados com os engenheiros da Microsoft, mas requer trabalho adicional pela organização para carregar no Collaborate MS.

## <a name="engagement-types"></a>Tipos de contrato

No portal do MS Collaborate, cada item de trabalho de comentários é associado com um único contrato para garantir que somente os usuários certos e sistemas têm acesso ao item de trabalho. Contratos podem ser entre uma organização da Microsoft e uma outra organização (um compromisso de organização único) ou o contrato pode ser entre várias organizações (contratos de várias partes) - por exemplo, um OEM, um ODM, além de uma organização do Microsoft e um parceiro IHV trabalhando em um dispositivo específico.  Para obter mais informações sobre contratos, consulte [programas e contratos](intro-to-mscollaborate.md#programs-and-engagements).

- Na **contratos único de terceiros**, somente a organização específica da Microsoft e a uma organização nomeada podem ver os comentários associados ao contrato de itens de trabalho. Ambos os usuários da organização podem criar um novo e colabore em itens de trabalho existentes no contrato. Outras organizações ou usuários não associados ao contrato podem ver o item de trabalho. 

- Na **contratos com vários participantes**, todas as organizações chamadas no engagement podem ver e editar os mesmos itens de trabalho compartilhada.  Outras organizações ou usuários não associados ao contrato podem ver o item de trabalho.

- Na **contratos qualquer organização**, os usuários são adicionados como indivíduos e não como as organizações. Esse estilo de engagement normalmente é usado para comentários de entrada apenas.   

## <a name="legal-agreement"></a>Contrato legal 

Quando você carregar Collaborate MS, aceite os termos de uso que abrangem os comentários para os compromissos você pertence. Você poderá sempre examinar padrão aqui os termos: MS Collaborate [termos de uso](https://go.microsoft.com/fwlink/?linkid=849107).

Contratos de colaboração em um contrato legal deve existir entre as partes em ordem para que eles colaborar. Você pode ser solicitado a aceitar um contrato legal ou termos de uso antes de acessar o engagement pela primeira vez.  Como um membro do contrato, você será capaz de ver as outras organizações que participam na colaboração. Os usuários podem atribuir o bug para uma organização específica para indicar o "parceiro no ponto".  No entanto, os usuários verão apenas os nomes de outros usuários em sua organização.  Outras organizações não terá acesso à lista de usuários.

## <a name="universal-partner-id"></a>ID de parceiro universal

A ID de parceiro Universal é uma ID fornecida pelo sistema de comentários do MS Collaborate e é compartilhada com todos os usuários que têm acesso ao item de trabalho. Essa ID é a ID dentro do sistema Collaborate MS e não é a ID específica de qualquer sistema de engenharia de equipe do recurso. Essa nova ID universal facilita colaborações com vários participantes para que haja uma ID comum usada por todas as partes.

> Proprietário do contrato pode decidir também incluem campos adicionais que mostra a ID específica no sistema de engenharia (por exemplo, uma ID do VSTS). 
