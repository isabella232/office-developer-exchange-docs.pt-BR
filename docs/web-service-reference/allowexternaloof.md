---
title: AllowExternalOof
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AllowExternalOof
api_type:
- schema
ms.assetid: e5387172-5b92-4bb1-8394-180e9c7ff771
description: O elemento AllowExternalOof contém um valor que identifica a quem mensagens externas fora do Office (OOF) são enviadas.
ms.openlocfilehash: 7d2e34797af8a9e9d11570a5ea2e618db7630f0c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523220"
---
# <a name="allowexternaloof"></a>AllowExternalOof

O **elemento AllowExternalOof** contém um valor que identifica a quem mensagens externas fora do Office (OOF) são enviadas. 
  
- [GetUserOofSettingsResponse](getuseroofsettingsresponse.md)
  
- [AllowExternalOof](allowexternaloof.md)
  
```xml
<AllowExternalOof>None or Known or All</AllowExternalOof>
```

 **ExternalAudience**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Contém os resultados da resposta e as configurações OOF para um usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário para esse elemento. A tabela a seguir lista os valores possíveis para esse elemento.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|**Nenhum** <br/> |Os destinatários de email fora da organização do usuário da caixa de correio que enviam mensagens para o usuário não receberão uma resposta de mensagem OOF externa.  <br/> |
|**Known** <br/> |Os remetentes de email fora da organização do usuário da caixa de correio que enviam mensagens para o usuário receberão apenas uma resposta de mensagem OOF externa se o remetente estiver na lista de contatos do Exchange store do usuário.  <br/> |
|**Tudo** <br/> |Os destinatários de email fora da organização do usuário da caixa de correio que enviam mensagens para o usuário receberão uma resposta de mensagem OOF externa.  <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento compartilha o mesmo tipo que o [elemento ExternalAudience.](externalaudience.md) 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserOofSettings](getuseroofsettings-operation.md) 
- [Operação SetUserOofSettings](setuseroofsettings-operation.md)

