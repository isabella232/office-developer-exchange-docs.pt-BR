---
title: DomainResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6aa319be-3a01-4044-8dfc-8fa1318524c3
description: O elemento DomainResponse contém as configurações solicitadas para o domínio especificado.
ms.openlocfilehash: c40f33a278b5032913329a7cd64346b572f5df2f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751917"
---
# <a name="domainresponse-soap"></a>DomainResponse (SOAP)

O elemento **DomainResponse** contém as configurações solicitadas para o domínio especificado. 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DomainSettingErrors (SOAP)](domainsettingerrors-soap.md) <br/> |Contém informações de erro para as configurações que não puderam ser retornadas.  <br/> |
|[DomainSettings (SOAP)](domainsettings-soap.md) <br/> |Representa as configurações de domínio que foram enviadas em uma solicitação de descoberta automática ou retornadas por uma resposta de descoberta automática.  <br/> |
|[RedirectTarget (SOAP)](redirecttarget-soap.md) <br/> |Identifica o destino do redirecionamento. O destino pode ser uma URL ou um endereço de email.  <br/> |
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Especifica o código de erro que está associado à solicitação específica.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Especifica a mensagem de erro que está associada à solicitação específica.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ArrayOfDomainResponse (SOAP)](arrayofdomainresponse-soap.md) <br/> |Contém uma matriz de elementos de **DomainResponse** . Cada elemento **DomainResponse** contém as configurações solicitadas para o usuário especificado.  <br/> |
|[DomainResponses (SOAP)](domainresponses-soap.md) <br/> |Contém as respostas para cada domínio.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

