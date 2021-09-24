---
title: Lidar com erros relacionados à delegação no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 631d364f-e324-4838-a92c-820286f771f8
description: Saiba como lidar com erros relacionados à delegação em aplicativos que você desenvolve usando a API Gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 17e4e7898f5cbed7a6dc524a84db6ba4080eab88
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512293"
---
# <a name="handling-delegation-related-errors-in-ews-in-exchange"></a>Lidar com erros relacionados à delegação no EWS no Exchange

Saiba como lidar com erros relacionados à delegação em aplicativos que você desenvolve usando a API Gerenciada do EWS ou o EWS no Exchange.
  
Se o aplicativo usa delegação ou adiciona ou remove representantes, talvez seja preciso lidar com erros relacionados à delegação. Você pode manipular esses erros em tempo de execução ou enquanto desenvolve seu aplicativo do EWS. Esses erros são definidos pela enumeração [ServiceError](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) da API Gerenciada EWS e pelo elemento [EWS ResponseCode.](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 
  
## <a name="delegation-related-errors"></a>Erros relacionados à delegação

|**Erro**|**Ocorre quando você tenta...**|**Manipulá-lo pelo …**|
|:-----|:-----|:-----|
|ErrorItemNotFound  <br/> ErrorFolderNotFound  <br/> |Execute uma operação em uma caixa de correio, pasta ou item ao que você não tem acesso.  <br/> |Atualizando as permissões do representante para permitir que eles acessem a pasta ou item chamando o método [UpdateDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) EWS Managed API ou a [operação UpdateDelegate](https://msdn.microsoft.com/library/03f618ac-ad1a-4772-9b81-c5bb0f12d6ab%28Office.15%29.aspx) EWS e, em seguida, tentando novamente a solicitação.  <br/> |
|ErrorAccessDenied  <br/> |Modifique um item que você não tem privilégios suficientes para modificar.  <br/> |Atualizando suas permissões de representante chamando o **método updateDelegate** EWS Managed API ou **a operação UpdateDelegate** EWS e, em seguida, tentando novamente a solicitação.  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |Tente adicionar o proprietário da caixa de correio como representante à sua própria caixa de correio.  <br/> |[Adicionando um usuário diferente como representante,](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)não o proprietário da caixa de correio.  <br/> |
|ErrorDelegateAlreadyExists  <br/> |Adicione o representante quando o representante já existir.  <br/> |Não fazendo nada, porque o representante já existe para o proprietário da caixa de correio. Ou, se você estiver tentando alterar as permissões de um representante existente, use o **método UpdateDelegates** ou a **operação UpdateDelegate.**  <br/> |
|ErrorNotDelegate  <br/> |Modificar permissões de representante para um usuário que não tem permissões de representante para a caixa de correio.  <br/> |[Adicionar o usuário como representante da](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) caixa de correio antes de tentar atualizar ou remover suas permissões.  <br/> |
|ErrorDelegateNoUser  <br/> |Modificar permissões de representante para um usuário que não está no Serviço de Domínio do Active Directory (AD DS).  <br/> |Criando o usuário no AD DS ou corrigindo as informações do representante na solicitação.  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |Use um representante para assinar notificações em nome do proprietário da caixa de correio.  <br/> |Assinatura de notificações como o proprietário da caixa de correio.  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |Faça uma solicitação de um representante que tenha uma versão de servidor diferente do servidor de caixa de correio da entidade.  <br/> |Usando um representante ou adicionando um representante cuja caixa de correio tem a mesma versão de servidor que o proprietário da caixa de correio.  <br/> |
|ErrorMissingEmailAddress  <br/> |Faça uma solicitação usando uma conta delegada que não tenha uma caixa de correio.  <br/> |Adicionando uma caixa de correio à conta do representante.  <br/> |
   
## <a name="see-also"></a>Confira também


- [Acesso de representante e EWS no Exchange](delegate-access-and-ews-in-exchange.md)
    
- [Ferramentas e recursos para solucionar problemas de aplicativos EWS para Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

