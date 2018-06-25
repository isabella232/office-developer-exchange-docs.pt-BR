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
ms.openlocfilehash: cf213fc3d7be02c411e9c2e83a4ff153dbefe098
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751195"
---
# <a name="appstatus"></a>AppStatus

O valor do elemento **AppStatus** indica o status do aplicativo de email. 
  
```XML
<AppStatus/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Metadados](metadata-ex15websvcsotherref.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **AppStatus** indica o status do aplicativo de email. Se o usuário pode corrigir um problema relacionado ao status do aplicativo de email, o elemento [ActionUrl](actionurl.md) fornece a URL para executar a correção. 
  
**Tabela 1. Valores de AppStatus**

|**Valor**|**Descrição**|
|:-----|:-----|
|NULL ou 0  <br/> |O aplicativo de email tem um status Íntegro.  <br/> |
|1.0  <br/> |O aplicativo de email não pôde ser atualizado automaticamente. O aplicativo de email deve ser reinstalado da Office Store.  <br/> |
|1.1  <br/> |O aplicativo de email não pôde ser atualizado automaticamente. O aplicativo de email requer permissões de aumento, e isso requer sua confirmação para instalar e revisão.  <br/> |
|1.2  <br/> |O aplicativo de email não pôde ser atualizado automaticamente. A licença atual expirou ou é inválida. Atualize o aplicativo de email da Office Store.  <br/> |
|2.0  <br/> |A licença de aplicativo de email não pôde ser atualizada automaticamente. A licença para o aplicativo de email precisa ser recuperado da Office Store.  <br/> |
|2.1  <br/> |A licença de aplicativo de email não pôde ser atualizada automaticamente. A licença atual expirou. Uma nova licença para esse aplicativo precisa ser instalado da Office Store.  <br/> |
|3.0  <br/> |O status da Office Store para o aplicativo de email foi alterada. Isso pode indicar que há um problema com o aplicativo de email. Vá para a página de aplicativo de email no Office Store para obter mais informações.  <br/> |
|3.1  <br/> |O aplicativo de email foi removido da Office Store.  <br/> |
|3.2  <br/> |Um problema foi descoberto com o aplicativo de email e temporariamente tiver sido retirado da Office Store.  <br/> |
|3.3  <br/> |O aplicativo de email será removido da Office Store dentro de 30 dias.  <br/> |
|4.0  <br/> |O aplicativo de email foi desabilitado automaticamente pelo seu cliente de email.  <br/> |
|4.1  <br/> |O aplicativo de email foi desabilitado pelo Outlook por motivos de desempenho.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> | http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Não aplicável  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Metadados](metadata-ex15websvcsotherref.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

