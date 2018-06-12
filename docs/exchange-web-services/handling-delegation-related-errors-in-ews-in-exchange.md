---
title: Tratando erros relacionados a delegação no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 631d364f-e324-4838-a92c-820286f771f8
description: Descubra como lidar com erros relacionados a delegação em aplicativos que você desenvolva usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 3851709888e3a1087df02eea5d4d58888ad168e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750658"
---
# <a name="handling-delegation-related-errors-in-ews-in-exchange"></a>Tratando erros relacionados a delegação no EWS no Exchange

Descubra como lidar com erros relacionados a delegação em aplicativos que você desenvolva usando a API gerenciada de EWS ou EWS no Exchange.
  
Se seu aplicativo usa delegação ou adiciona ou remove representantes, você pode precisar manipular erros relacionados a delegação. Você pode manipular esses erros em tempo de execução ou enquanto desenvolve seu aplicativo do EWS. Esses erros são definidos pela enumeração EWS Managed API [ServiceError](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) e o elemento do EWS [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) . 
  
## <a name="delegation-related-errors"></a>Erros relacionados a delegação

|**Erro**|**Ocorre quando você tenta …**|**Manipulá-lo pelo …**|
|:-----|:-----|:-----|
|ErrorItemNotFound  <br/> ErrorFolderNotFound  <br/> |Realize uma operação em uma caixa de correio, pasta ou item que você não tem acesso ao.  <br/> |Atualizando as permissões do representante para habilitá-los acessar a pasta ou o item chamando o método de API gerenciada de EWS [UpdateDelegates](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) ou a operação [UpdateDelegate](http://msdn.microsoft.com/library/03f618ac-ad1a-4772-9b81-c5bb0f12d6ab%28Office.15%29.aspx) EWS e, em seguida, uma nova solicitação.  <br/> |
|ErrorAccessDenied  <br/> |Modifica um item que você não tem privilégios suficientes para modificar.  <br/> |Atualizar suas permissões de representante chamando o método de API gerenciada de EWS **UpdateDelegate** ou a operação **UpdateDelegate** EWS e, em seguida, uma nova solicitação.  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |Tentativa de adicionar o proprietário da caixa de correio como um representante para sua própria caixa de correio.  <br/> |[Adicionando um usuário diferente, como um representante](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md), não é o proprietário da caixa de correio.  <br/> |
|ErrorDelegateAlreadyExists  <br/> |Adicione o representante quando o delegado já existe.  <br/> |Fazer nada, porque o delegado já existe para o proprietário da caixa de correio. Ou, se você está tentando alterar as permissões de um representante existente e, em seguida, use o método de **UpdateDelegates** ou a operação **UpdateDelegate** .  <br/> |
|ErrorNotDelegate  <br/> |Modificar permissões de representante para um usuário que não tem nenhuma permissão de representante da caixa de correio.  <br/> |[Adicionar o usuário como um representante](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) para a caixa de correio antes de tentar atualizar ou remover suas permissões.  <br/> |
|ErrorDelegateNoUser  <br/> |Modificar permissões de representante para um usuário que não esteja no serviço de domínio Active Directory (AD DS).  <br/> |Criando o usuário no AD DS ou corrigir as informações de representante na solicitação.  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |Use um representante para assinar notificações em nome do proprietário da caixa de correio.  <br/> |Assinatura de notificações como o proprietário da caixa de correio.  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |Fazer uma solicitação de um delegado que tem uma versão de servidor diferente que o servidor de caixa de correio do principal.  <br/> |Usando um representante ou adicionando um representante cuja caixa de correio tem a mesma versão do servidor como o proprietário da caixa de correio.  <br/> |
|ErrorMissingEmailAddress  <br/> |Fazer uma solicitação usando uma conta de representante que não tem uma caixa de correio.  <br/> |Adicionando uma caixa de correio à conta do representante.  <br/> |
   
## <a name="see-also"></a>Confira também


- [Acesso de representante e EWS no Exchange](delegate-access-and-ews-in-exchange.md)
    
- [Ferramentas e recursos para solucionar problemas de aplicativos do EWS do Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

