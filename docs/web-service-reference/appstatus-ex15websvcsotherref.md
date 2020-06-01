---
title: AppStatus
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f3ab8bf1-abc5-45cf-a2e1-d7602f2c24ec
description: O valor do elemento AppStatus indica o status do aplicativo de email.
ms.openlocfilehash: d833947fd62d500418f257829d241a2e0b3bca9c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464774"
---
# <a name="appstatus"></a>AppStatus

O valor do elemento **AppStatus** indica o status do aplicativo de email. 
  
```XML
<AppStatus/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Metadata](metadata-ex15websvcsotherref.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **AppStatus** indica o status do aplicativo de email. Se o usuário puder corrigir um problema relacionado ao status do aplicativo de email, o elemento [ActionUrl](actionurl.md) fornecerá a URL para executar a correção. 
  
**Tabela 1. Valores de AppStatus**

|**Valor**|**Descrição**|
|:-----|:-----|
|Nulo ou 0  <br/> |O aplicativo de email tem um status Íntegro.  <br/> |
|1.0  <br/> |O aplicativo de email não pôde ser atualizado automaticamente. O aplicativo de email precisa ser reinstalado da Office Store.  <br/> |
|1.1  <br/> |O aplicativo de email não pôde ser atualizado automaticamente. O aplicativo de email requer mais permissões, e isso exige que a revisão e a confirmação sejam instaladas.  <br/> |
|1.2  <br/> |O aplicativo de email não pôde ser atualizado automaticamente. A licença atual expirou ou é inválida. Atualize o aplicativo de email da Office Store.  <br/> |
|2.0  <br/> |A licença do aplicativo de email não pôde ser atualizada automaticamente. A licença do aplicativo de email precisa ser recuperada da Office Store.  <br/> |
|2.1  <br/> |A licença do aplicativo de email não pôde ser atualizada automaticamente. A licença atual expirou. Uma nova licença para este aplicativo precisa ser instalada da Office Store.  <br/> |
|3,0  <br/> |O status da Office Store para o aplicativo de email foi alterado. Isso pode indicar que há um problema com o aplicativo de email. Vá para a página aplicativo de email na Office Store para obter mais informações.  <br/> |
|3.1  <br/> |O aplicativo de email foi removido da Office Store.  <br/> |
|3.2  <br/> |Foi descoberto um problema com o aplicativo de email e foi temporariamente retirado da Office Store.  <br/> |
|3.3  <br/> |O aplicativo de email será removido da Office Store dentro de 30 dias.  <br/> |
|4,0  <br/> |O aplicativo de email foi desabilitado automaticamente pelo cliente de email.  <br/> |
|4.1  <br/> |O aplicativo de email foi desabilitado pelo Outlook por motivos de desempenho.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> | https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Não aplicável  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Metadata](metadata-ex15websvcsotherref.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

