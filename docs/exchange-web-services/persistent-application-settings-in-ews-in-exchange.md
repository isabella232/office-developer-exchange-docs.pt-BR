---
title: Configurações de aplicativo persistente no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 394d4e70-8517-4073-809a-5b61780ff923
description: Saiba mais sobre as diferentes opções que a API gerenciada do EWS ou o aplicativo EWS pode usar para criar configurações de aplicativo personalizadas persistentes no Exchange.
ms.openlocfilehash: b1faa057e5a0c1a96498efcc23738c83d25ae986
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457400"
---
# <a name="persistent-application-settings-in-ews-in-exchange"></a>Configurações de aplicativo persistente no EWS no Exchange

Saiba mais sobre as diferentes opções que a API gerenciada do EWS ou o aplicativo EWS pode usar para criar configurações de aplicativo personalizadas persistentes no Exchange.
  

  
A maneira mais fácil de manter as configurações de cliente personalizadas em sincronia para uma caixa de correio, ou pastas e itens em uma caixa de correio, é armazenar as configurações de aplicativo em um servidor Exchange. Você pode garantir que essas configurações persistam para uma caixa de correio usando uma das seguintes opções: 
  
- Objetos de configuração do usuário
    
- Propriedades estendidas
    
- Itens personalizados
    
## <a name="what-are-my-options-for-creating-persistent-application-settings"></a>Quais são as opções para a criação de configurações de aplicativos persistentes?
<a name="Options"> </a>

Os objetos de configuração do usuário são a melhor opção para armazenar definições de configuração para seus aplicativos cliente do EWS. Você também pode usar propriedades estendidas ou itens personalizados, ou uma combinação de todos os três. Escolha sua opção com base no escopo das suas configurações e se suas configurações precisam estar disponíveis para outros aplicativos.
  
**Tabela 1. Opções recomendadas para a criação de configurações de aplicativos persistentes com base no escopo**

|**Definindo o escopo**|**Use...**|**Acessado por**|
|:-----|:-----|:-----|
|Item  <br/> |Uma propriedade estendida em um item existente.  <br/> |Qualquer aplicativo EWS. Somente os clientes EWS que conhecem o identificador de propriedade podem acessar uma propriedade estendida.  <br/> |
|Folder  <br/> |Um objeto de configuração do usuário na pasta de destino. Essa é uma boa maneira de salvar as configurações de exibição de uma pasta.  <br/> |Qualquer aplicativo EWS.  <br/> |
|Caixa de correio  <br/> |Um objeto de configuração do usuário na pasta padrão do msgrootfolder  <br/> |Qualquer aplicativo EWS.  <br/> |
   
### <a name="user-configuration-objects"></a>Objetos de configuração do usuário
<a name="UserConfig"> </a>

Os objetos de configuração do usuário são itens especiais que são associados a pastas em uma caixa de correio. Os objetos de configuração do usuário, também conhecidos como itens associados à pasta, normalmente são a melhor opção para persistir as configurações do aplicativo, especialmente se as informações de configuração estiverem associadas a uma pasta ou uma caixa de correio. Normalmente, eles não são exibidos para usuários finais. Como eles podem armazenar de forma nativa os fluxos de dados e os dicionários de dados, eles são ideais para o armazenamento de informações de configuração. A melhor maneira de usar objetos de configuração do usuário é armazenar um conjunto de configurações em um documento XML e, em seguida, salvar essas informações em uma das propriedades do fluxo de configuração do usuário.
  
Os objetos de configuração do usuário são acessados de forma diferente dos outros tipos de itens armazenados em uma caixa de correio. Você pode usar o método [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=EXCHG.80%29.aspx) EWS Managed API ou a operação do EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) para localizar todos os itens, mas você deve usar a opção de travessia de pesquisa **associada** para localizar objetos de configuração do usuário. A passagem de pesquisa **associada** indica que os resultados da pesquisa devem conter somente objetos de configuração do usuário. O EWS inclui um conjunto de operações específicas para os objetos de configuração do usuário. 
  
**Tabela 1. Operações do EWS e métodos da API gerenciada do EWS para trabalhar com objetos de configuração do usuário**

|**Para...**|**Use esta operação do EWS**|**Usar este método de API gerenciada do EWS**|
|:-----|:-----|:-----|
|Criar um objeto de configuração do usuário  <br/> |[Operação CreateUserConfiguration](https://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) <br/> |[Userconfiguration. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) <br/> |
|Obter um objeto de configuração do usuário  <br/> |[Operação GetUserConfiguration](https://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |[Userconfiguration. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) <br/> [Userconfiguration. Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.load%28v=exchg.80%29.aspx) <br/> |
|Atualizar um objeto de configuração do usuário  <br/> |[Operação UpdateUserConfiguration](https://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) <br/> |[Userconfiguration. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) <br/> |
|Excluir um objeto de configuração do usuário  <br/> |[Operação DeleteUserConfiguration](https://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) <br/> |[Userconfiguration. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) <br/> |
   
> [!NOTE]
> Os objetos de configuração do usuário criados usando o EWS têm um prefixo de [categoria](https://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) que começa com "IPM. Configuração. ". A **pseudoclasse** de um objeto de configuração do usuário é o prefixo do objeto de configuração do usuário e o nome do objeto de configuração do usuário. Você pode usar a propriedade [Item.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) ItemProperty EWS Managed API ou o elemento @ @ @ @ **Class** do EWS para pesquisar objetos de configuração do usuário que você definiu. 
  
### <a name="extended-properties"></a>Propriedades estendidas
<a name="ExtendedProperties"> </a>

Use [Propriedades estendidas](properties-and-extended-properties-in-ews-in-exchange.md) se quiser armazenar informações de configuração em itens. O EWS, diferentemente de MAPI, não retorna um recipiente de propriedades para itens. Isso significa que um cliente do EWS deve saber o identificador de propriedade estendida para encontrar e acessar a propriedade estendida. Se você precisar armazenar informações de configuração em itens diferentes dos objetos de configuração do usuário, usar propriedades estendidas para criar propriedades personalizadas pode ser a solução para você. Propriedades estendidas permitem que você acesse e armazene informações sobre propriedades que não fazem parte do conjunto de propriedades padrão para um item. 
  
> [!IMPORTANT]
> O esquema do banco de dados do Exchange tem um número finito de propriedades. O número máximo de identificadores de propriedade para um banco de dados do Exchange é 32.767. Se você estiver usando propriedades estendidas para armazenar muitas configurações, sugerimos que você use uma única propriedade estendida para armazenar essas configurações, para que você não exceda o máximo. 
  
Você pode usar o método [Item. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=EXCHG.80%29.aspx) a API gerenciada do EWS ou a operação [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS para definir propriedades estendidas nos objetos de configuração do usuário. 
  
### <a name="custom-items"></a>Itens personalizados
<a name="CustomItems"> </a>

Itens personalizados também podem ser usados para armazenar informações. As propriedades de item existentes podem ser realocadas para que contenham informações de configuração. Ou você pode usar propriedades estendidas para definir suas próprias propriedades para seu aplicativo. O uso de itens personalizados para armazenar a configuração fornece os seguintes benefícios: 
  
- Eles funcionam para todas as versões do Exchange que dão suporte ao EWS.
    
- Se você não usar propriedades estendidas no item, o orçamento das propriedades do Exchange não será cobrado.
    
## <a name="where-should-i-store-my-application-settings"></a>Onde devo armazenar minhas configurações de aplicativo?
<a name="ApplicationSettingsLocation"> </a>

Pastas de caixa de correio e os itens dentro delas estão localizados na pasta de mensagens raiz. Essa pasta é identificada pelo valor [WellKnownFolderName. msgfolderroot](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) na API gerenciada do EWS. Em termos MAPI, este é o equivalente da sub-árvore IPM de uma caixa de correio. Os objetos de configuração do usuário são frequentemente usados para criar configurações baseadas na interface do usuário, para que um aplicativo possa renderizar configurações de exibição com base na pasta que um usuário está acessando. As configurações de exibição com base em pasta normalmente são definidas em um objeto de configuração de usuário que está associado à pasta. Mas, às vezes, você pode querer tornar suas configurações globais para seu aplicativo. Nesse caso, você pode armazenar suas configurações na pasta de mensagens raiz. 
  
A maioria dos usuários não está ciente e normalmente não acessa a pasta raiz da caixa de correio. Essa pasta é identificada pelo valor [WellKnownFolderName. root](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) na API gerenciada do EWS. Em termos MAPI, este é o equivalente da sub-árvore não-IPM de uma caixa de correio. As informações que os usuários finais não acessam diretamente são armazenadas na pasta raiz da caixa de correio. Você pode querer armazenar sua configuração de aplicativo nessa pasta porque os aplicativos cliente não costuma acessá-lo. 
  
## <a name="version-differences"></a>Diferenças de versão
<a name="VersionDifferences"> </a>

Os objetos de configuração do usuário estão disponíveis no Exchange Online, no Exchange Online como parte do Office 365 e versões do Exchange a partir do Exchange 2010.
  
## <a name="see-also"></a>Também consulte


- [Gerenciar configurações de aplicativos persistentes usando o EWS no Exchange](how-to-manage-persistent-application-settings-by-using-ews-in-exchange.md)
    
- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)
    
- [Propriedades e propriedades estendidas no EWS no Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Trabalhar com pastas usando o EWS no Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)
    

