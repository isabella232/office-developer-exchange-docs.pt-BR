---
title: Gerar uma lista de pontos de extremidade de descoberta automática
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 82394d3c-9fc7-4b3c-b48d-1fe983c198f7
description: Descubra como gerar uma lista de prioridades de pontos de extremidade de descoberta automática.
ms.openlocfilehash: ccecacc9c8beef464727efbc9d1fced7a81f9b7c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750726"
---
# <a name="generate-a-list-of-autodiscover-endpoints"></a>Gerar uma lista de pontos de extremidade de descoberta automática

Descubra como gerar uma lista de prioridades de pontos de extremidade de descoberta automática.
  
A primeira tarefa no [processo de descoberta automática](autodiscover-for-exchange.md) é gerar uma lista de pontos de extremidade de descoberta automática para seu aplicativo de teste. Esses pontos de extremidade de descoberta automática podem ser provenientes de uma [pesquisa de SCP](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) ou podem ser derivados do endereço de email do usuário. No final, você pode terminar com um grande número de pontos de extremidade. Vamos analisar como você pode organizá-los por prioridade. 
  
## <a name="start-with-scp-lookup"></a>Comece com a pesquisa do SCP
<a name="bk_StartWithScp"> </a>

Pontos de extremidade de descoberta automática que vêm de uma [pesquisa de SCP](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) devem ter prioridade mais alta na sua lista. Os administradores podem configurar os objetos de SCP para rotear seu cliente à empresa de descoberta automática mais próximos ou mais eficiente, portanto, é uma boa ideia iniciar com esses pontos de extremidade. Como o processo de pesquisa do SCP tem seu próprio esquema priorização, os resultados da pesquisa SCP são já priorizados, da seguinte maneira: 
  
1. Pontos de extremidade de descoberta automática de objetos SCP no escopo do site do Active Directory ao qual pertence o computador cliente.
    
2. Pontos de extremidade de descoberta automática de objetos SCP não escopo qualquer site do Active Directory.
    
3. Pontos de extremidade de descoberta automática de objetos SCP com escopo para um site diferente do Active Directory que o site ao qual pertence o computador cliente.
    
Depois que os resultados do processo de pesquisa de SCP, você pode adicionar pontos de extremidade que derivam do endereço de email do usuário. Eles podem servir como definir um padrão de pontos de extremidade e de fallback, caso nenhum resultado SCP ou os pontos de extremidade retornados da pesquisa SCP não são suficientes.
  
## <a name="add-endpoints-derived-from-the-users-email-address"></a>Adicionar pontos de extremidade derivados do endereço de email do usuário
<a name="bk_AddDerivedEndpoints"> </a>

Quando a pesquisa do SCP não funciona ou os pontos de extremidade retornados pela pesquisa SCP não retornam uma resposta bem-sucedida, você pode derivar um conjunto de pontos de extremidade de descoberta automática de padrão de endereço de email do usuário. Esses pontos de extremidade devem ser uma prioridade mais baixa que qualquer um que vêm de uma pesquisa de SCP, mas você pode precisá-los se a pesquisa de SCP não foi bem-sucedida.
  
### <a name="to-derive-autodiscover-endpoints"></a>Para derivar os pontos de extremidade de descoberta automática

1. Extraia o nome de domínio do endereço de email do usuário. Por exemplo, se o endereço de email do usuário for Sadie.Daniels@contoso.com, o nome de domínio seria contoso.com.
    
2. Construa URLs de ponto de extremidade sem extensões de arquivo nos seguintes formatos:
    
  - "https://" + domínio + "/ autodiscover/autodiscover"
    
  - "https://autodiscover." + domínio + "/ autodiscover/autodiscover"
    
Após compilar a lista de URLs de ponto de extremidade que derive de pesquisa do SCP e o endereço de email do usuário, você pode precisar revisar as extensões de nome de arquivo dessas URLs, dependendo se você estiver usando o [serviço web de descoberta automática do SOAP](http://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx) ou o [POX Serviço web de descoberta automática](http://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx).
  
## <a name="add-or-replace-file-name-extensions-in-endpoint-urls"></a>Adicione ou substitua as extensões de nome de arquivo no ponto de extremidade URLs
<a name="bk_FileExtensions"> </a>

Você pode acessar o serviço Descoberta automática usando o serviço web de descoberta automática do SOAP ou o serviço web de descoberta automática de POX. Cada serviço usa URLs semelhantes de ponto de extremidade, com a única diferença é a extensão de nome de arquivo. O serviço web de descoberta automática do SOAP usa a extensão de nome de arquivo ". svc" e o serviço web de descoberta automática de POX usa a extensão de nome de arquivo ". xml".
  
Por padrão, o ponto de extremidade de descoberta automática URLs retornados de uma pesquisa de SCP são POX URLs. No entanto, se você estiver usando a descoberta automática do SOAP, você pode simplesmente alterar a extensão de nome de arquivo de ". xml" para ". svc" e tente uma solicitação SOAP.
  
Para os URLs derivados de ponto de extremidade de descoberta automática, a extensão de arquivo é omitida. Adicione a extensão de arquivo apropriado para o serviço web de descoberta automática que estiver usando antes de tentar a URL.
  
## <a name="example-generating-a-list-of-autodiscover-endpoints"></a>Exemplo: Gerar uma lista de pontos de extremidade de descoberta automática
<a name="bk_Example"> </a>

Vamos dar uma olhada em um exemplo. Sadie Daniels (Sadie.Daniels@contoso.com) está usando um aplicativo de serviços Web do Exchange (EWS) pela primeira vez. O aplicativo usa a descoberta automática para configurar em si. Computador de Sadie está unido ao domínio contoso.com e está no site do Active Directory de Redmond. O aplicativo gera a lista de pontos de extremidade de descoberta automática mostrado na Figura 1.
  
**Figura 1: Lista de amostra de pontos de extremidade de descoberta automática**

![Uma exemplo de lista de pontos de extremidade de Descoberta Automática, mostrando pontos de extremidade obtidos por meio da pesquisa SCP como tendo maior prioridade do que pontos de extremidade derivados.](media/Ex15_Autodiscover_GenerateList_Example.png)
  
Os aplicativos do EWS neste exemplo prefere o serviço web de descoberta automática do SOAP, para que ele altera a extensão de nome de arquivo para os resultados do SCP para ". svc" antes de enviar solicitações SOAP para acessá-los.
  
## <a name="next-steps"></a>Próximas etapas
<a name="bk_NextSteps"> </a>

Depois que você gera uma lista de pontos de extremidade de descoberta automática, tente-los ao [Enviar solicitações para os pontos de extremidade](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).
  
## <a name="see-also"></a>Confira também


- [Descoberta Automática do Exchange](autodiscover-for-exchange.md)
    
- [Encontrar os pontos de extremidade de descoberta automática usando pesquisa do SCP no Exchange](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [Manipulação de mensagens de erro de descoberta automática](handling-autodiscover-error-messages.md)
    

