---
title: DomainResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 6aa319be-3a01-4044-8dfc-8fa1318524c3
description: O elemento DomainResponse contém as configurações solicitadas para o domínio especificado.
ms.openlocfilehash: fb7288b55452d8499596ce09c3ada9cec4b88d5b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517200"
---
# <a name="domainresponse-soap"></a>DomainResponse (SOAP)

O **elemento DomainResponse** contém as configurações solicitadas para o domínio especificado. 
  
```XML
<DomainResponse>
   <DomainSettingErrors/>
   <DomainSettings/>
   <RedirectTarget/>
   <ErrorCode/>
   <ErrorMessage/>
</DomainResponse>
```

 **DomainResponse**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DomainSettingErrors (SOAP)](domainsettingerrors-soap.md) <br/> |Contém informações de erro para configurações que não puderam ser retornadas.  <br/> |
|[DomainSettings (SOAP)](domainsettings-soap.md) <br/> |Representa as configurações de domínio que foram enviadas em uma solicitação de Descoberta Automática ou retornadas por uma resposta de Descoberta Automática.  <br/> |
|[RedirectTarget (SOAP)](redirecttarget-soap.md) <br/> |Identifica o destino do redirecionamento. O destino pode ser uma URL ou um endereço de email.  <br/> |
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Especifica o código de erro associado à solicitação específica.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Especifica a mensagem de erro associada à solicitação específica.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ArrayOfDomainResponse (SOAP)](arrayofdomainresponse-soap.md) <br/> |Contém uma matriz de **elementos DomainResponse.** Cada **elemento DomainResponse** contém as configurações solicitadas para o usuário especificado.  <br/> |
|[DomainResponses (SOAP)](domainresponses-soap.md) <br/> |Contém as respostas para cada domínio.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

