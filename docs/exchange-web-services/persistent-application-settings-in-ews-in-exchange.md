---
title: Configurações do aplicativo persistente no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 394d4e70-8517-4073-809a-5b61780ff923
description: Saiba mais sobre as diferentes opções que o seu aplicativo de EWS ou a API gerenciada de EWS pode usar para criar definições de aplicativo personalizado persistente no Exchange.
ms.openlocfilehash: b384fd5608dc647950d7cd31e861e24c12e3316f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750947"
---
# <a name="persistent-application-settings-in-ews-in-exchange"></a>Configurações do aplicativo persistente no EWS no Exchange

Saiba mais sobre as diferentes opções que o seu aplicativo de EWS ou a API gerenciada de EWS pode usar para criar definições de aplicativo personalizado persistente no Exchange.
  

  
A maneira mais fácil para manter as configurações de cliente personalizado em sincronização para uma caixa de correio ou pastas e itens em uma caixa de correio, é serão armazenadas as configurações de aplicativo em um servidor Exchange. Você pode garantir que essas configurações persistem para uma caixa de correio usando um destes procedimentos: 
  
- Objetos de configuração do usuário
    
- Propriedades estendidas
    
- Itens personalizados
    
## <a name="what-are-my-options-for-creating-persistent-application-settings"></a>Cite minhas opções para a criação de configurações do aplicativo persistente.
<a name="Options"> </a>

Objetos de configuração do usuário são a melhor opção para armazenar definições de configuração para seus aplicativos de cliente do EWS. Você também pode usar estender propriedades ou itens personalizados ou uma combinação dessas três. Escolha a opção com base no escopo de suas configurações e se as configurações precisam estar disponível para outros aplicativos.
  
**Tabela 1. Opções recomendadas para a criação de configurações de aplicativo persistente com base no escopo**

|**Definindo o escopo**|**Use …**|**Acessado por**|
|:-----|:-----|:-----|
|Item  <br/> |Uma propriedade estendida em um item existente.  <br/> |Qualquer aplicativo do EWS. Somente os clientes do EWS que saber o identificador de propriedade podem acessar uma propriedade estendida.  <br/> |
|Pasta  <br/> |Um objeto de configuração do usuário na pasta de destino. Isso é uma boa maneira de salvar configurações de exibição para uma pasta.  <br/> |Qualquer aplicativo do EWS.  <br/> |
|Mailbox  <br/> |Um objeto de configuração do usuário na pasta padrão msgrootfolder.  <br/> |Qualquer aplicativo do EWS.  <br/> |
   
### <a name="user-configuration-objects"></a>Objetos de configuração do usuário
<a name="UserConfig"> </a>

Objetos de configuração do usuário são especiais itens que estão associados a pastas em uma caixa de correio. Objetos de configuração do usuário, também conhecido como itens de pasta associada, geralmente são a melhor opção para mantendo configurações de aplicativo, especialmente se as informações de configuração são associadas a uma pasta ou uma caixa de correio. Eles geralmente não são exibidos aos usuários finais. Porque eles nativamente podem armazenar fluxos de dados e de dicionários de dados, eles são ideais para armazenar informações de configuração. A melhor maneira de usar os objetos de configuração do usuário é armazenar um conjunto de configurações em um documento XML e salve essas informações em uma das propriedades do fluxo de configuração do usuário.
  
Objetos de configuração do usuário são acessados de forma diferente de outros tipos de itens armazenados em uma caixa de correio. Você pode usar o método de API gerenciada de EWS [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=EXCHG.80%29.aspx) ou a operação [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS para localizar todos os itens, mas você deve usar a opção de passagem de pesquisa **associado** para localizar os objetos de configuração do usuário. A passagem de pesquisa **associado** indica que os resultados da pesquisa devem conter apenas os objetos de configuração do usuário. EWS inclui um conjunto de operações que são específicos para objetos de configuração do usuário. 
  
**Tabela 1. Operações do EWS e métodos de API gerenciada de EWS para trabalhar com objetos de configuração do usuário**

|**Para...**|**Use esta operação EWS**|**Use este método API gerenciada de EWS**|
|:-----|:-----|:-----|
|Criar um objeto de configuração do usuário  <br/> |[Operação CreateUserConfiguration](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) <br/> |[UserConfiguration.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) <br/> |
|Obter um objeto de configuração do usuário  <br/> |[Operação GetUserConfiguration](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |[UserConfiguration.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) <br/> [UserConfiguration.Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.load%28v=exchg.80%29.aspx) <br/> |
|Atualizar um objeto de configuração do usuário  <br/> |[Operação UpdateUserConfiguration](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) <br/> |[UserConfiguration.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) <br/> |
|Excluir um objeto de configuração do usuário  <br/> |[Operação DeleteUserConfiguration](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) <br/> |[UserConfiguration.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) <br/> |
   
> [!NOTE]
> Objetos de configuração do usuário criados usando o EWS têm um prefixo de [ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) que começa com "IPM. Configuração. ". O **ItemClass** de um objeto de configuração do usuário é o prefixo de objeto de configuração do usuário e seu nome de objeto de configuração do usuário. Você pode usar a propriedade da API gerenciada de EWS [Item.ItemClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) ou o elemento **ItemClass** EWS para procurar objetos de configuração do usuário que você definiu. 
  
### <a name="extended-properties"></a>Propriedades estendidas
<a name="ExtendedProperties"> </a>

Use [propriedades estendidas](properties-and-extended-properties-in-ews-in-exchange.md) , se você deseja armazenar informações de configuração nos itens. EWS, ao contrário de MAPI, não retorna um recipiente de propriedades de itens. Isso significa que um cliente do EWS precisa saber o identificador de propriedade estendida para localizar e acessar a propriedade estendida. Se você precisar armazenar as informações de configuração em itens que não sejam de objetos de configuração do usuário, usando as propriedades estendidas para criar propriedades personalizadas pode ser a solução para você. Propriedades estendidas permitem acessar e armazenar informações sobre propriedades que não fazem parte da propriedade standard definido para um item. 
  
> [!IMPORTANT]
> O esquema de banco de dados do Exchange tem um número finito das propriedades. O número máximo de identificadores de propriedade para um banco de dados do Exchange é 32,767. Se você estiver usando propriedades estendidas para armazenar várias configurações, sugerimos que você use uma única propriedade estendida para armazenar as definições para que você não exceder nesse máximo. 
  
Você pode usar o método de API gerenciada de EWS [Item.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=EXCHG.80%29.aspx) ou a operação de EWS [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) para definir as propriedades estendidas em objetos de configuração do usuário. 
  
### <a name="custom-items"></a>Itens personalizados
<a name="CustomItems"> </a>

Itens personalizados também podem ser usados para armazenar informações. As propriedades de item existentes podem ser redirecionadas para conter as informações de configuração. Ou então, você pode usar propriedades estendidas para definir suas próprias propriedades para seu aplicativo. Usando itens personalizados para armazenar configuração fornece os seguintes benefícios: 
  
- Eles funcionam para todas as versões do Exchange que suportam o EWS.
    
- Se você não usar propriedades estendidas no item, o orçamento das propriedades do Exchange não é cobrado.
    
## <a name="where-should-i-store-my-application-settings"></a>Onde posso deve armazenar configurações de meu aplicativo?
<a name="ApplicationSettingsLocation"> </a>

Pastas de caixa de correio e os itens dentro deles estão localizados na pasta raiz de mensagem. Essa pasta é identificada pelo valor [WellKnownFolderName.msgfolderroot](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) na API gerenciada do EWS. Em termos MAPI, isso é o equivalente da subárvore IPM de uma caixa de correio. Objetos de configuração do usuário geralmente são usados para criar configurações de interface do usuário, para que um aplicativo pode renderizar as configurações de exibição com base na pasta que um usuário está acessando. Configurações de modos de exibição baseados em pasta geralmente são definidas em um objeto de configuração do usuário que está associado à pasta. Mas, às vezes, talvez você queira fazer suas configurações globais para seu aplicativo. Nesse caso, você pode armazenar as configurações na pasta raiz de mensagem. 
  
A maioria dos usuários não estão cientes e geralmente não acessar a pasta de caixa de correio de raiz. Essa pasta é identificada pelo valor [WellKnownFolderName.root](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) na API gerenciada do EWS. Em termos MAPI, isso é o equivalente a subárvore não-IPM de uma caixa de correio. Informações que os usuários finais não acessar diretamente são armazenadas na pasta raiz da caixa de correio. Convém armazenar sua configuração de aplicativo nesta pasta porque aplicativos cliente não normalmente acessá-lo. 
  
## <a name="version-differences"></a>Diferenças de versão
<a name="VersionDifferences"> </a>

Objetos de configuração do usuário estão disponíveis no Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange, começando com o Exchange 2010.
  
## <a name="see-also"></a>Confira também


- [Gerenciar configurações de aplicativo persistente usando o EWS no Exchange](how-to-manage-persistent-application-settings-by-using-ews-in-exchange.md)
    
- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md)
    
- [Propriedades e as propriedades estendidas no EWS no Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Trabalhar com pastas usando o EWS no Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)
    

