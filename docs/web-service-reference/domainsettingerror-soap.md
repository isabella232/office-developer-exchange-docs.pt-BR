---
title: DomainSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 48c3f7b5-2ee0-42ce-97a1-a881e2f60327
description: O elemento DomainSettingError representa um erro que ocorreu durante a recuperação de uma configuração de domínio. Isso representa um erro de uma solicitação de GetDomainSettings.
ms.openlocfilehash: 08b0a47acea8d35ec78efd701168a251771effac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751926"
---
# <a name="domainsettingerror-soap"></a>DomainSettingError (SOAP)

O elemento **DomainSettingError** representa um erro que ocorreu durante a recuperação de uma configuração de domínio. Isso representa um erro de uma solicitação de **GetDomainSettings** . 
  
```XML
<DomainSettingError>
   <ErrorCode/>
   <ErrorMessage/>
   <SettingName/>
</DomainSettingError>
```

 **DomainSettingError**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Identifica o código de erro que está associado à solicitação específica.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Contém a mensagem de erro que está associada à solicitação específica.  <br/> |
|[SettingName (SOAP)](settingname-soap.md) <br/> |Representa o nome da configuração.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DomainSettingErrors (SOAP)](domainsettingerrors-soap.md) <br/> |Contém informações de erro para as configurações que não puderam ser retornadas.  <br/> |
   
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

