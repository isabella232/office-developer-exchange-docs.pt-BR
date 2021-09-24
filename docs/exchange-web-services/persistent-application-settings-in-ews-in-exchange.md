---
title: Configurações de aplicativo persistente no EWS em Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 394d4e70-8517-4073-809a-5b61780ff923
description: Saiba mais sobre as diferentes opções que sua API Gerenciada do EWS ou aplicativo EWS pode usar para criar configurações de aplicativo personalizado persistente no Exchange.
ms.openlocfilehash: 3fdc7ad3d5acabf6b498743afe8d93f0eff048c3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516135"
---
# <a name="persistent-application-settings-in-ews-in-exchange"></a>Configurações de aplicativo persistente no EWS em Exchange

Saiba mais sobre as diferentes opções que sua API Gerenciada do EWS ou aplicativo EWS pode usar para criar configurações de aplicativo personalizado persistente no Exchange.
  

  
A maneira mais fácil de manter as configurações de cliente personalizadas em sincronia para uma caixa de correio, ou pastas e itens em uma caixa de correio, é armazenar configurações de aplicativo em um servidor Exchange servidor. Você pode garantir que essas configurações persistam para uma caixa de correio usando uma das seguintes: 
  
- Objetos de configuração do usuário
    
- Propriedades estendidas
    
- Itens personalizados
    
## <a name="what-are-my-options-for-creating-persistent-application-settings"></a>Quais são as minhas opções para criar configurações de aplicativos persistentes?
<a name="Options"> </a>

Os objetos de configuração do usuário são a melhor opção para armazenar as configurações dos aplicativos cliente EWS. Você também pode usar propriedades de extensão ou itens personalizados ou uma combinação de todos os três. Escolha sua opção com base no escopo de suas configurações e se suas configurações precisam estar disponíveis para outros aplicativos.
  
**Tabela 1. Opções recomendadas para criar configurações de aplicativo persistentes com base no escopo**

|**Definindo escopo**|**Use...**|**Acessado por**|
|:-----|:-----|:-----|
|Item  <br/> |Uma propriedade estendida em um item existente.  <br/> |Qualquer aplicativo EWS. Somente clientes EWS que conhecem o identificador de propriedade podem acessar uma propriedade estendida.  <br/> |
|Folder  <br/> |Um objeto de configuração do usuário na pasta de destino. Essa é uma boa maneira de salvar as configurações de exibição de uma pasta.  <br/> |Qualquer aplicativo EWS.  <br/> |
|Mailbox  <br/> |Um objeto de configuração do usuário na pasta padrão msgrootfolder.  <br/> |Qualquer aplicativo EWS.  <br/> |
   
### <a name="user-configuration-objects"></a>Objetos de configuração do usuário
<a name="UserConfig"> </a>

Os objetos de configuração do usuário são itens especiais associados a pastas em uma caixa de correio. Os objetos de configuração do usuário, também conhecidos como itens associados à pasta, geralmente são a melhor opção para manter as configurações do aplicativo, especialmente se as informações de configuração estão associadas a uma pasta ou uma caixa de correio. Normalmente, eles não são ativos para usuários finais. Como eles podem armazenar nações fluxos de dados e dicionários de dados, eles são ideais para armazenar informações de configuração. A melhor maneira de usar objetos de configuração do usuário é armazenar um conjunto de configurações em um documento XML e salvar essas informações em uma das propriedades de fluxo de configuração do usuário.
  
Os objetos de configuração do usuário são acessados de forma diferente dos outros tipos de item armazenados em uma caixa de correio. Você pode usar o [método Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=EXCHG.80%29.aspx) EWS Managed API ou a operação [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)  EWS para encontrar todos os itens, mas você deve usar a opção de pesquisa associada para encontrar objetos de configuração do usuário. A **pesquisa associada indica** que os resultados da pesquisa devem conter apenas objetos de configuração do usuário. O EWS inclui um conjunto de operações que são específicas dos objetos de configuração do usuário. 
  
**Tabela 1. Operações EWS e métodos de API Gerenciada do EWS para trabalhar com objetos de configuração do usuário**

|**Para...**|**Usar essa operação EWS**|**Usar este método de API Gerenciada do EWS**|
|:-----|:-----|:-----|
|Criar um objeto de configuração do usuário  <br/> |[Operação CreateUserConfiguration](https://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) <br/> |[UserConfiguration.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) <br/> |
|Obter um objeto de configuração do usuário  <br/> |[Operação GetUserConfiguration](https://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |[UserConfiguration.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) <br/> [UserConfiguration.Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.load%28v=exchg.80%29.aspx) <br/> |
|Atualizar um objeto de configuração do usuário  <br/> |[Operação UpdateUserConfiguration](https://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) <br/> |[UserConfiguration.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) <br/> |
|Excluir um objeto de configuração do usuário  <br/> |[Operação DeleteUserConfiguration](https://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) <br/> |[UserConfiguration.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) <br/> |
   
> [!NOTE]
> Os objetos de configuração do usuário criados usando o EWS têm um [prefixo ItemClass](https://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) que começa com "IPM. Configuration.". A **ItemClass** de um objeto de configuração do usuário é o prefixo do objeto de configuração do usuário e o nome do objeto de configuração do usuário. Você pode usar a propriedade da API Gerenciada [Item.ItemClass](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) EWS ou o **elemento EWS ItemClass** para pesquisar objetos de configuração do usuário que você definiu. 
  
### <a name="extended-properties"></a>Propriedades estendidas
<a name="ExtendedProperties"> </a>

Use [propriedades estendidas](properties-and-extended-properties-in-ews-in-exchange.md) se quiser armazenar informações de configuração em itens. O EWS, diferentemente de MAPI, não retorna um pacote de propriedades para itens. Isso significa que um cliente EWS deve conhecer o identificador de propriedade estendida para encontrar e acessar a propriedade estendida. Se você precisar armazenar informações de configuração em itens que não sejam objetos de configuração do usuário, usar propriedades estendidas para criar propriedades personalizadas pode ser a solução para você. As propriedades estendidas permitem que você acesse e armazene informações sobre propriedades que não fazem parte do conjunto de propriedades padrão de um item. 
  
> [!IMPORTANT]
> O Exchange de banco de dados tem um número finito de propriedades. O número máximo de identificadores de propriedade para um banco de dados Exchange é 32.767. Se você estiver usando propriedades estendidas para armazenar muitas configurações, sugerimos que você use uma única propriedade estendida para armazenar essas configurações para que você não exceda esse máximo. 
  
Você pode usar o método Da API Gerenciada [Item.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=EXCHG.80%29.aspx) EWS ou a operação [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS para definir propriedades estendidas em objetos de configuração do usuário. 
  
### <a name="custom-items"></a>Itens personalizados
<a name="CustomItems"> </a>

Itens personalizados também podem ser usados para armazenar informações. As propriedades de item existentes podem ser repurpostas para conter informações de configuração. Ou você pode usar propriedades estendidas para definir suas próprias propriedades para seu aplicativo. O uso de itens personalizados para armazenar a configuração oferece os seguintes benefícios: 
  
- Eles funcionam para todas as versões de Exchange que suportam o EWS.
    
- Se você não usar propriedades estendidas no item, o orçamento Exchange propriedades não será cobrado.
    
## <a name="where-should-i-store-my-application-settings"></a>Onde devo armazenar minhas configurações de aplicativo?
<a name="ApplicationSettingsLocation"> </a>

As pastas de caixa de correio e os itens dentro delas estão localizados na pasta de mensagem raiz. Essa pasta é identificada pelo [valor WellKnownFolderName.msgfolderroot](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) na API Gerenciada do EWS. Em termos MAPI, isso é o equivalente à subárvore IPM de uma caixa de correio. Os objetos de configuração do usuário geralmente são usados para criar configurações baseadas na interface do usuário, para que um aplicativo possa renderizar as configurações de exibição com base na pasta que um usuário está acessando. As configurações de exibição baseadas em pasta geralmente são definidas em um objeto de configuração do usuário associado à pasta. Mas, às vezes, talvez você queira tornar suas configurações globais para seu aplicativo. Nesse caso, você pode armazenar suas configurações na pasta de mensagem raiz. 
  
A maioria dos usuários não está ciente e normalmente não acessa a pasta de caixa de correio raiz. Essa pasta é identificada pelo [valor WellKnownFolderName.root](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) na API Gerenciada do EWS. Em termos MAPI, isso é o equivalente à subárvore não IPM de uma caixa de correio. As informações que os usuários finais não acessam diretamente são armazenadas na pasta de caixa de correio raiz. Talvez você queira armazenar a configuração do aplicativo nessa pasta porque os aplicativos cliente normalmente não o acessam. 
  
## <a name="version-differences"></a>Diferenças de versão
<a name="VersionDifferences"> </a>

Os objetos de configuração do usuário estão disponíveis no Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange a partir do Exchange 2010.
  
## <a name="see-also"></a>Confira também


- [Gerenciar configurações de aplicativo persistente usando o EWS no Exchange](how-to-manage-persistent-application-settings-by-using-ews-in-exchange.md)
    
- [Visão geral de design do cliente EWS para o Exchange](ews-client-design-overview-for-exchange.md)
    
- [Propriedades e propriedades estendidas no EWS no Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Trabalhar com pastas usando o EWS no Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Trabalhar com Exchange de caixa de correio usando o EWS no Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)
    

