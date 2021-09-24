---
title: DomainSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 48c3f7b5-2ee0-42ce-97a1-a881e2f60327
description: O elemento DomainSettingError representa um erro que ocorreu durante a recuperação de uma configuração de domínio. Isso representa um erro de uma solicitação GetDomainSettings.
ms.openlocfilehash: d2d7e1fc1509ade88de0013cb9e4ff54712d0f56
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530144"
---
# <a name="domainsettingerror-soap"></a>DomainSettingError (SOAP)

O **elemento DomainSettingError** representa um erro que ocorreu durante a recuperação de uma configuração de domínio. Isso representa um erro de uma **solicitação GetDomainSettings.** 
  
```XML
<DomainSettingError>
   <ErrorCode/>
   <ErrorMessage/>
   <SettingName/>
</DomainSettingError>
```

 **DomainSettingError**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Identifica o código de erro associado à solicitação específica.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Contém a mensagem de erro associada à solicitação específica.  <br/> |
|[SettingName (SOAP)](settingname-soap.md) <br/> |Representa o nome da configuração.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DomainSettingErrors (SOAP)](domainsettingerrors-soap.md) <br/> |Contém informações de erro para configurações que não puderam ser retornadas.  <br/> |
   
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

