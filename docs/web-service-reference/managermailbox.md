---
title: ManagerMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 70c324d5-2196-406d-a674-73323f8d8b92
description: O elemento ManagerMailbox contém informações SMTP que identificam a caixa de correio do gerente do contato.
ms.openlocfilehash: c30a343ad7071e92c826925407f8447ae6baccae
ms.sourcegitcommit: 63e48eaf2891a6db1a718b55cd69e3a0433c4a9c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2021
ms.locfileid: "58851111"
---
# <a name="managermailbox"></a>ManagerMailbox

O **elemento ManagerMailbox** contém informações SMTP que identificam a caixa de correio do gerente do contato. 
  
```XML
<ManagerMailbox>
   <Mailbox/>
</ManagerMailbox>
```

 **SingleRecipientType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixa de Correio](mailbox.md) <br/> |Identifica um objeto Active Directory habilitado para email que identifica o remetente.  <br/> |
  
### <a name="parent-elements"></a>Elementos pai

|**Nome do elemento**|**Descrição**|
|:-----|:-----|
|[Contato](contact.md) <br/> |Representa um item de contato no Exchange store.  <br/> |

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


[Criando contatos (Exchange Web Services)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

