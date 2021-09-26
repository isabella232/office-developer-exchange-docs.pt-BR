---
title: DirectReports
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ab88739f-9018-4887-ae46-f1471242628c
description: O elemento DirectReports contém informações SMTP que identificam os relatórios diretos de um contato.
ms.openlocfilehash: a84e37836b645ec679208094ed893d04793f01d2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542348"
---
# <a name="directreports"></a>DirectReports

O **elemento DirectReports** contém informações SMTP que identificam os relatórios diretos de um contato. 
  
```XML
<DirectReports>
   <Mailbox/>
</DirectReports>
```

 **SingleRecipientType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixa de Correio](mailbox.md) <br/> |Identifica um objeto de serviço de diretório do Active Directory habilitado para email.  <br/> |
     
### <a name="parent-elements"></a>Elementos pai

|**Nome do elemento**|**Descrição**|
|:-----|:-----|
|[Contato](contact.md) <br/> |Representa o item de contato no Exchange store.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
Este elemento foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Criando contatos (Exchange Web Services)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

