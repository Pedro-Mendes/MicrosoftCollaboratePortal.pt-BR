---
title: Downloads para trabalhar com o pacote
description: Microsoft Collaborate pacotes contêm arquivos disponíveis para download e estão associados com contratos. O Gerenciador de distribuição está disponível para realizar downloads em massa ou de vários arquivos.
author: ikhapova
ms.author: ikhapova
ms.date: 12/12/2017
keywords: pacotes, contratos, pacote baixa, baixa, compilações, permissões colaborar, Microsoft Connect
ms.openlocfilehash: 25a89feaf8d71be3cde4393042f1bf0e8047c765
ms.sourcegitcommit: 8ae2ead732e03d8a9865797bb9f40818780036e9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2018
ms.locfileid: "43055203"
---
# <a name="working-with-packages-to-download-content"></a>Trabalhando com pacotes para baixar conteúdo

No Microsoft Collaborate (MS Collaborate), o conteúdo para download está disponível como *pacotes* que contêm os arquivos para baixar.  Pacotes têm metadados associados a eles para facilitar a localizar os pacotes corretos, como uma descrição, tipo de pacote, palavras-chave e data de publicação.   

Depende de quais pacotes você pode baixar os compromissos você pertence.  Durante a publicação, editores de conteúdo direcionar contratos específicos para o pacote. Se você for um membro participante de compromisso, você poderá ver os pacotes para esse contrato.  Isso significa que os usuários podem ver apenas os pacotes associados a contratos que pertencem a.

MS Collaborate fornece dois mecanismos para baixar pacotes de conteúdo:
1. MS Collaborate **página de pacotes no portal** permite que você localizar pacotes e baixar arquivos individuais de um pacote. 
2. MS Collaborate **Gerenciador de distribuição** pode ser instalado em seu computador local para baixar vários arquivos e pacotes de uma só vez.

Independentemente do mecanismo de download usado, os usuários verão os mesmos pacotes no portal como o Gerenciador de distribuição.

Editor do conteúdo é uma função de permissões no Collaborate MS associados com os compromissos.  Neste momento, somente os usuários da Microsoft podem publicar os compromissos. Os proprietários de Engagement definir quais usuários têm permissões de Editor do conteúdo.

## <a name="finding-packages-in-the-ms-collaborate-portal"></a>Localizando os pacotes no portal do MS Collaborate

Sobre o **pacotes** página, você pode filtrar e pesquisar pacotes com base em vários critérios, incluindo:
- palavras no nome, 
- o programa ou o contrato que o pacote pertence 
- Quando o pacote foi publicado, 
- o tipo dos arquivos no pacote, e
- usando palavras-chave.

Por exemplo, se você estiver procurando por um pacote específico do serviço de compilação do Windows e você souber o número de compilação, você poderia digitá-lo como um filtro. Cada caixa de filtro é cumulativa, portanto, você pode começar com menos filtros e adicionar mais licenças limitar o número de pacotes retornados até encontrar o que você está procurando. Você também pode classificar a lista de pacotes por coluna para ajudar a localizar os pacotes.

O Gerenciador de distribuição tem recursos de pesquisa/classificação básica, mas o portal fornece uma experiência de pesquisa/filtragem mais avançada.  Se você tiver muitos pacotes disponíveis para você, é recomendável que você use a pesquisa do portal para localizar o pacote correto e, em seguida, pesquise o nome do pacote no Gerenciador de distribuição.

## <a name="how-to-download-files-from-the-ms-collaborate-portal"></a>Como baixar arquivos do portal Collaborate MS

1. No painel, clique em "Pacotes" para obter o **pacotes** página, onde você verá uma lista de todos os pacotes disponíveis para download.

2. Pesquise ou utilize **filtros avançados** para localizar o pacote que você deseja baixar. Os filtros são cumulativos para ajudar a restringir a pesquisa. Use o botão "Limpar filtros" para remover todos os filtros.
    - Clique o **filtros avançados** ícone para alternar a exibição do filtro avançado "campos.
    ![Ícone de filtros avançado](images/package-advanced-filter.png)
3. Quando você localizar o pacote que você deseja fazer o download, clique para abrir o pacote. Você encontrará todos os detalhes sobre o pacote e uma lista de arquivos disponíveis para download.
    ![Janela de detalhes do pacote](images/package-details.png)

4. Clique em cada arquivo para iniciar o download. No portal do MS Collaborate, você pode baixar um arquivo por vez. 

## <a name="using-distribution-manager-for-multi-file-downloads"></a>Usando o Gerenciador de distribuição para downloads de vários arquivos

Se você quiser baixar um pacotes completos com vários arquivos ou pacotes grandes, é recomendável instalar o **Gerenciador de distribuição**.  O Gerenciador de distribuição é um aplicativo de cliente do ClickOnce que será atualizado conforme necessário.  

Esse aplicativo cliente conecta-se aos serviços do MS Collaborate usando as mesmas credenciais que você usa para fazer logon no portal do Collaborate MS. Todos os mesmos pacotes que você pode ver no portal do MS Collaborate aparecerão no Gerenciador de distribuição.

Além de baixar vários arquivos ao mesmo tempo, você pode enfileirar muitos pacotes para serem executados em segundo plano e você também pode personalizar as configurações de download para solucionar problemas de conexão.

### <a name="how-to-install-the-distribution-manager"></a>Como instalar o Gerenciador de distribuição

1. Dos **pacotes** , clique no **Gerenciador de distribuição** botão na parte superior da página. 
    ![Instalar o Gerenciador de distribuição na página pacotes](images/Distribution-Mgr-Launch.PNG)

2. Clique em **aberto** na mensagem e clique **instalar** na caixa de diálogo de instalação do aplicativo. 

Se você já estiver conectado ao centro de desenvolvimento, quando você clica no botão Distributuion Gerenciador, o Gerenciador de distribuição iniciará e conectá-lo com a mesma conta usada para fazer logon no Collaborate MS.

### <a name="how-to-log-in-to-distribution-manager"></a>Como fazer logon para o Gerenciador de distribuição

O Gerenciador de distribuição usa a mesma conta usada para Collaborate MS.  Se você iniciá-lo a partir do portal Collaborfate MS, você será ser conectado automaticamente.  Se você não ainda tiver entrado no MS Collaborate, ou se você estiver usando uma conta MSA para acessar o site, você precisa fazer logon para o Gerenciador de distribuição novamente. Isso usará a mesma conta e o processo usado para fazer logon no portal do Collaborate MS.

1.  Inicie o aplicativo Gerenciador de distribuição em seu computador selecionando o **Gerenciador de distribuição** botão a **pacotes** página no portal do MS Collaborate ou navegando até  **O Gerenciador de distribuição** na lista de aplicativos do seu computador.

2.  Você verá o mesmo log na tela que você vê quando você fizer logon no Centro de desenvolvimento ou Collaborate MS. Selecione a conta apropriada, insira sua senha e o Gerenciador de distribuição se conectarão à sua conta da MS Collaborate.

### <a name="how-to-download-packages-using-distribution-manager"></a>Como baixar pacotes usando o Gerenciador de distribuição

1.  No Gerenciador de distribuição, procure pacotes usando a funcionalidade de pesquisa ou ao rolar por meio de sua lista de pacotes.
2.  Você pode selecionar vários arquivos dentro de um pacote ou vários pacotes para baixar.  Até quatro pacotes podem baixar cada vez.
3.  Você pode selecionar a pasta que você gostaria de fazer o download usando o **procurar** botão.
4.  Clique em **baixar** para iniciar o download dos pacotes selecionados.
5.  Atualizar ícones para indicar o status para pacotes que estão na fila para download.

Você verá os arquivos que estão **baixando agora** , bem como pacotes que estão na fila para download.  Você pode clicar em **baixar agora** para ver apenas os arquivos que estão baixando.  

Você também pode navegar até **verificar se há Downloads agora** no Menu no Gerenciador de distribuição.

   ![Seleção de item de menu Downloads agora na página pacotes](images/check-for-downloads.png)

> [!NOTE]
> - Você pode **pausar o download** e, em seguida, continue para continuar o download.
> - Você pode forçar uma sincronização do Gerenciador de distribuição, clicando no item de menu e, em seguida, selecionando **verificar se há Downloads agora**.
> - Clicar em **configurações** no Menu permite que você faça as personalizações. 

### <a name="customizing-distribution-manager-settings"></a>Personalizando as configurações do Gerenciador de distribuição

No Gerenciador de distribuição, você pode acessar **configurações** no menu próximo a nome de login.  As configurações do Gerenciador de distribuição destinam-se a permitir que você personalize como os pacotes sejam baixados.  Você pode ajustar as configurações a seguir:
- Tamanho do bloco, 
- Baixe os Threads, e
- Velocidade máxima.

É recomendável que você apenas alterá-las se você estiver tendo problemas com o download que podem ser devido a uma conexão lenta ou não confiável.

![Personalizar as configurações do Gerenciador de distribuição](images/Distribution-Mgr-Settings.PNG)

