---
title: Introdução ao Microsoft colaborar
description: Visão geral do Portal de colaboração da Microsoft, incluindo recursos disponíveis e conceituais informações sobre como usar o sistema.  MS Collaborate permite o compartilhamento de engenharia itens de trabalho do sistema (bugs, solicitações de recursos), distribuição de conteúdo (compilações, documentos, especificações) e o gerenciamento de usuários, substituindo o Microsoft Connect e o portal de gerenciamento de comentários SysDev.
author: chriskleinke
ms.author: chriskl
ms.date: 09/01/2017
keywords: especificações de comentários de parceiros, downloads de compilação, baixando, bugs, Microsoft Connect, SysDev bugs, bugs de centro de desenvolvimento
ms.openlocfilehash: 319b4abf1cdbd23bdf240f88aa154c9804a20fb2
ms.sourcegitcommit: 8ae2ead732e03d8a9865797bb9f40818780036e9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2018
ms.locfileid: "43054690"
---
# <a name="introduction-to-microsoft-collaborate"></a>Introdução ao Microsoft colaborar

O portal do Microsoft Collaborate (Collaborate MS) fornece ferramentas e serviços para simplificar a colaboração de engenharia dentro do ecossistema da Microsoft.  

Habilita Collaborate MS:
- O compartilhamento de engenharia de itens de trabalho do sistema (bugs, solicitações de recursos, etc.);
- Distribuição de conteúdo (compilações, documentos, ferramentas, especificações);  
- Capacidade de gerenciar usuários do sistema. 

Disponível por meio de [painel do Microsoft Dev Center](//developer.microsoft.com/dashboard/collaborate), o novo portal de MS Collaborate fornece um único local usando um único conjunto de credenciais para ver seus itens de trabalho e o conteúdo.  Esse novo sistema substitui o portal do Microsoft Connect, bem como o portal de gerenciamento de comentários SysDev. 

Você pode acessar Collaborate MS usando o link amigável: [ https://aka.ms/collaborate ](https://aka.ms/collaborate).

Entrar usando suas credenciais do Centro de desenvolvimento, como qualquer indivíduo ou como um membro de uma empresa ou organização.  Antes de usar Collaborate MS, você precisará se registrar para o Centro de desenvolvimento. Para obter mais informações, consulte [registrar com o Microsoft Collaborate](registration.md).

## <a name="programs-and-engagements"></a>Programas e contratos

O sistema do MS Collaborate usa o conceito de **programas** e **contratos** como blocos de construção principais para o sistema. Programas fornecem a estrutura e facilitam o gerenciamento de contratos. Contratos têm apenas um programa de pai e eles herdam formulários de comentários, consultas e modelos de publicação definidos no nível do programa.  Contratos podem ser personalizados e eles definem conjuntos de usuários que podem interagir com o conteúdo e os comentários associados ao contrato. Os proprietários de programa são usuários da Microsoft que têm permissões para:
- definir metadados de programa, incluindo páginas de aterrissagem do programa
- Definir formas de comentários padrão
- definir modelos de publicação para facilitar a publicação de pacotes para vários contratos
- Identifique os gerentes de contrato que tem permissões para criar contratos sob o programa.

Quando você fizer logon no MS Collaborate, você verá os programas e os contratos que pertencem a. É possível que você for um membro de apenas um contrato ou de muitos compromissos dentro de um programa.  A funcionalidade que você vê no MS Collaborate também depende de sua função dentro de cada contrato. Participante os usuários podem baixar o conteúdo e enviar/editar comentários.  Se você tiver permissões administrativas, você também verá ícones Editar itens, que você terá permissão para exibir e editar.  Você pode ser um partcipant em um contrato e um usuário avançado em outro.

Para obter mais informações, consulte [programas e contratos](programs.md)

### <a name="engagement-management"></a>Gerenciamento de contratos

Um contrato define quais usuários estão habilitados para ver e interagir com conteúdo específico ou associados a esse contrato de itens de trabalho. A menos que um usuário é membro de um contrato, os usuários não vê nada relacionado ao contrato.

Os contratos são semelhantes a um grupo de segurança virtual, permitindo que os proprietários de envolvimento identificar quais usuários podem ver e trabalhar com os artefatos associados a esse contrato.  Há alguns tipos diferentes de determinado pelo número de organizações/usuários dentro do contrato e tipos de contratos:
- colaboração entre uma única empresa/organização e uma única organização da Microsoft,
- colaboração entre várias organizações nomeadas (por exemplo, usuários do Microsoft team 1, os usuários de uma empresa e usuários da empresa B), e
- colaboração com os usuários de qualquer organização.

Cada contrato está associado com o padrão MS Collaborate [termos de uso](https://go.microsoft.com/fwlink/?linkid=849107) ou um contrato legal personalizado entre as partes no contrato. Usuários participantes devem visitar a página do contrato e consulte a descrição e o contrato que se aplica a cada contrato específico.  Para obter mais informações sobre como ver o contrato legal para um contrato, consulte [como exibir seus compromissos](view-engagements.md).

Os proprietários de contrato são usuários da Microsoft que gerenciam o engagement no Collaborate MS.  Os usuários com permissões de proprietário do contrato podem: 
- Criar novo colaborações no sistema como um contrato nomeado que mapeará a conteúdo ou comentários aos usuários, 
- associar usuários com várias funções no sistema (incluindo a adição de administradores da organização como usuários avançados,
- Gerenciar formulários de comentários para o projeto, e 
- publica conteúdo para os usuários do engagement.

Administradores da organização (usuários avançados) podem gerenciar automaticamente os usuários de sua organização dentro de um contrato, incluindo a capacidade de:
- Adicionar ou remover contas de usuário da organização como usuários participantes em um contrato, e
- Adicionar ou remover outra usuários avançados da organização.

Para obter informações, consulte [gerenciamento de usuários da organização](managing-org-users.md).

### <a name="content-sharing"></a>Compartilhamento de conteúdo 

Compartilhamento de conteúdo é realizado pela publicação de "pacotes" de arquivos (documentos, binários, compilações, ferramentas, etc.) no Collaborate MS.  Editores de conteúdo podem direcionar contratos específicos ou todos os contratos dentro de um programa ao publicar um pacote para que ele está disponível para os usuários de contratos de destino. Quando publicado, os pacotes são associados com os compromissos, descrições e palavras-chave para facilitar a localizar os pacotes corretos com facilidade.  Dentro do MS Collaborate, participantes que os usuários podem pesquisar e baixar arquivos dentro de um pacote.  

Collaborate MS também fornece um Gerenciador de distribuição para facilitar o download de pacotes grandes ou vários arquivos.  O Gerenciador de distribuição é um aplicativo de cliente do ClickOnce pode ser acessado de dentro das páginas de baixar o pacote MS colaborar.  

Para obter mais informações, consulte [trabalhando com Downloads de pacote](package-downloads.md).

### <a name="feedback-work-item-exchange"></a>Troca de Item de trabalho de comentários

Comentários, ou Exchange de Item de trabalho, o sistema dentro do MS Collaborate permite o compartilhamento de comentários sobre itens de trabalho (bugs, recursos, etc.) no portal da MS Collaborate ou por meio de uma API diretamente para o sistema de engenharia de uma organização.  Cada item de trabalho está associado um contrato, que determina quais usuários ou organizações são as permissões para ver e interagir com o item de trabalho. 

Cada programa e/ou o contrato pode determinar como cada formulário de comentários será compartilhado e quais campos estarão disponíveis - as decisões e a configuração serão de responsabilidade do proprietário do contrato.  Além disso, os proprietários do engagement podem personalizar ainda mais cada formulário de comentários para ajudar a facilitar e simplificar o processo para o compartilhamento de itens de trabalho. Dependendo de como o contrato é configurado, os itens de trabalho podem ser criados por qualquer um dos usuários participante da Microsoft para o endereço ou por usuários da Microsoft para organizações de parceiros ao endereço.  Formulários de comentários também podem ser habilitados para compartilhar os anexos para o formulário de comentários.

As páginas de comentários de colaborar MS fornecem os modos de exibição de todos os seus itens de comentários, a pesquisa para identificar os comentários específicos e a capacidade de salvar e compartilhar consultas avançada.  Novo no MS Collaborate é a capacidade de compartilharam consultas disponíveis para todos os usuários dentro de um contrato ou programa.  Essas consultas podem ser configuradas para corresponder consultas usadas por usuários da Microsoft para facilitar a ter a mesma lista de bugs para revisão.

Collaborate MS também traz nova funcionalidade, permitindo que várias partes compartilhar o mesmo item de trabalho. Se o engagement contiver várias partes, podem ver todos os membros do contrato, editar e colaborar com os mesmos itens de trabalho.  Colaboração de comentários de várias partes exigem contratos legais apropriados entre as partes.

Por causa da nova funcionalidade de compartilhamento com vários participante, MS Collaborate introduz uma nova ID Universal que torna possível para todas as partes usando a mesma ID para se referir a itens de trabalho.  Compromissos específicos podem ser configurados para compartilhar também campos adicionais para ajudar os membros de um compromisso colaborar, por exemplo, um proprietário do contrato pode optar por incluir também um campo mostrando o específico interno Microsoft ID do sistema.

O portal do MS Collaborate pode ser usado para colaborar em itens de trabalho de comentários. O serviço de troca de Item de trabalho também pode se conectar a diferentes tipos de sistemas de engenharia. Existem agentes para possibilitar a instâncias do VSTS está se conectando por meio de configurações simples – nenhum código é necessário.  As organizações parceiras podem se conectar a WITEX diretamente em seu próprio sistema de engenharia por trás de seu firewall, incluindo os seguintes recursos: 
- Formulários de comentários: formulários de comentários personalizado estará disponíveis para cada contrato para ajudar a agilizar e simplificar o compartilhamento de informações.
- Comentários compartilhados: contratos podem ter tradicional de compartilhamento de 1-1 dos formulários de comentários entre duas organizações. Além disso, eles podem ter os formulários de comentários que são compartilhados entre várias organizações.

Para obter mais informações, consulte [trabalhando com itens de trabalho de comentários](feedback-items.md).

### <a name="notifications-and-invitations"></a>Notificações e convites

Os usuários poderão receber notificações quando ações específicas ou eventos que ocorrem dentro do sistema.  Não haverá notificações padrão (convites para novos contratos, novos pacotes disponíveis para fazer o download, itens de trabalho de comentários, essa alteração de estado, etc.) que estão disponíveis para todos os usuários.  Em futuras versões, os usuários poderão assinar e personalizar as notificações que eles recebem. 

Para receber notificações, cada usuário deve verificar que um endereço de email apropriado é fornecido na seção de notificações no Centro de desenvolvimento.  MS Collaborate usa suas informações de conta do Centro de desenvolvimento para notificações e permissões dentro do sistema.

### <a name="reporting-and-analytics"></a>Relatórios e análises

Relatórios a partir de Collaborate MS portal estará disponível para os usuários.  Os relatórios disponíveis é determinada pela sua função de associação dentro de contratos.  Relatórios predefinidos que indica as estatísticas de uso e a integridade geral do sistema estarão disponíveis, bem como a capacidade de usar o Power BI para analisar os dados. 

## <a name="how-does-ms-collaborate-differ-from-microsoft-connect"></a>Como o MS Collaborate difere do Microsoft Connect 

Microsoft Connect foi lançado em julho de 2005 e foi usado por milhões de usuários para fornecer comentários e baixar o conteúdo. Microsoft Connect permitiu que os usuários: 
- Encontrar produtos da Microsoft atualmente abertos ao recebimento comentários da comunidade; 
- Participar dos programas de comentários gerenciados pelas equipes de produtos da Microsoft;
- Baixar e testar produtos beta;
- Enviar bugs e sugestões para futuras versões;
- Votar, comentar e validar os comentários de outras pessoas.

MS Collaborate substitui Microsoft Connect, incluindo uma aparência diferente e novas funcionalidades para facilitar a colaboração. 

| Conectar-se de conceito | Conceito de portal Collaborate MS |
| ------- | -------- |
| Sites | N/D |
| Programas | Programas |
| Grupos de segurança | Contratos (definir usuários e permissões) |
| Downloads | Pacotes (coleções de arquivos) |
| Comentários | Comentários (bugs, recursos e outros itens de trabalho) |
| Administrador do programa (PA) | Proprietário do programa e os proprietários do Engagement|
| Chaves do produto | N/d - não está mais disponível |

### <a name="new-concepts-in-ms-collaborate"></a>Novos conceitos no MS Collaborate

Ao migrar do MS Connect para Collaborate MS, é importante entender como programas e contratos funcionam e como eles são usados para direcionar o acesso do usuário a e colaboração no conteúdo e comentários.  

- *As organizações*: MS Collaborate integra-se com o sistema de gerenciamento de conta no Centro de desenvolvimento, que usa Accounts da Microsoft (MSAs) e o Azure Active Directory.  Adicionando o Active Directory, MS Collaborate pode tirar proveito do conceito do Centro de desenvolvimento de organizações ou empresas; os usuários são membros das organizações que usam uma conta corporativa ou eles são indivíduos com uma MSA (único logon conta da Microsoft).
- *Proprietário do contrato*: administrador do projeto, capaz de configurar o projeto, modificar usuários; herda todos os outras potências de função de usuário para o contrato (publicação, configuração de comentários, etc.).
- *Gerenciador de conteúdo*: possam publicar e editar pacotes para um contrato ou programa.
- Nomes de programa e engajamento são visíveis a todos os usuários.  Contratos com organiations definido ou empresas identificam claramente as organizações que têm permissões para o contrato na página do contrato.  O contrato legal para o contrato também está disponível para todos os usuários que são membros do contrato.

Ao migrar do sistema mais antigo para o novo Collaborate MS com base no Centro de desenvolvimento, a maior alteração está migrando as contas de usuário para o Centro de desenvolvimento.  Centro de desenvolvimento identifica um "Dev Center Admin" quem é responsável por gerenciar as contas do Centro de desenvolvimento para a empresa.  Você precisará saber quem é seu administrador e se sua empresa usa o Active Directory ou não.  
   
