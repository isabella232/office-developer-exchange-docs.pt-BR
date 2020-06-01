---
title: Como lidar com erros relacionados à delegação no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 631d364f-e324-4838-a92c-820286f771f8
description: Descubra como lidar com erros relacionados à delegação em aplicativos que você desenvolve usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 145783c4e7f49ed6e2aa3a2dbe0d10909e06d7e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455349"
---
# <a name="handling-delegation-related-errors-in-ews-in-exchange"></a>Como lidar com erros relacionados à delegação no EWS no Exchange

Descubra como lidar com erros relacionados à delegação em aplicativos que você desenvolve usando a API gerenciada do EWS ou o EWS no Exchange.
  
Se o aplicativo usar delegação ou adicionar ou remover representantes, talvez seja necessário lidar com erros relacionados à delegação. Você pode manipular esses erros em tempo de execução ou enquanto desenvolve seu aplicativo do EWS. Esses erros são definidos pela enumeração de [erro](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) do EWS Managed API e pelo elemento EWS [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) . 
  
## <a name="delegation-related-errors"></a>Erros relacionados à delegação

|**Error**|**Ocorre quando você tenta...**|**Manipulá-lo pelo …**|
|:-----|:-----|:-----|
|ErrorItemNotFound  <br/> ErrorFolderNotFound  <br/> |Executar uma operação em uma caixa de correio, pasta ou item que você não tem acesso.  <br/> |Atualizando as permissões do representante para permitir que eles acessem a pasta ou o item chamando o método da API gerenciada do EWS [UpdateDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) ou a operação EWS do [UpdateDelegate](https://msdn.microsoft.com/library/03f618ac-ad1a-4772-9b81-c5bb0f12d6ab%28Office.15%29.aspx) e, em seguida, repetindo a solicitação.  <br/> |
|ErrorAccessDenied  <br/> |Modifique um item que você não tem privilégios suficientes para modificar.  <br/> |Atualização de suas permissões de representante chamando o método de API gerenciada do EWS **UpdateDelegate** ou a operação do EWS do **UpdateDelegate** e, em seguida, repetindo a solicitação.  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |Tente adicionar o proprietário da caixa de correio como um representante à sua própria caixa de correio.  <br/> |[Adicionar um usuário diferente como um representante](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md), não o proprietário da caixa de correio.  <br/> |
|ErrorDelegateAlreadyExists  <br/> |Adicionar o representante quando o representante já existir.  <br/> |Não faz nada, porque o representante já existe para o proprietário da caixa de correio. Ou, se você estiver tentando alterar as permissões de um representante existente, use o método **UpdateDelegates** ou a operação **UpdateDelegate** .  <br/> |
|ErrorNotDelegate  <br/> |Modificar permissões de representante para um usuário que não tem permissões de representante para a caixa de correio.  <br/> |[Adicionar o usuário como um representante](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) para a caixa de correio antes de tentar atualizar ou remover suas permissões.  <br/> |
|ErrorDelegateNoUser  <br/> |Modificar permissões de representante para um usuário que não está no AD DS (serviço de domínio Active Directory).  <br/> |Criar o usuário no AD DS ou corrigir as informações de representante na solicitação.  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |Use um representante para inscrever-se em notificações em nome do proprietário da caixa de correio.  <br/> |Assinatura de notificações como o proprietário da caixa de correio.  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |Faça uma solicitação de um representante que tenha uma versão de servidor diferente do servidor de caixa de correio da entidade de segurança.  <br/> |Usando um representante ou adicionando um delegado cuja caixa de correio tem a mesma versão do servidor do proprietário da caixa de correio.  <br/> |
|ErrorMissingEmailAddress  <br/> |Faça uma solicitação usando uma conta de representante que não tenha uma caixa de correio.  <br/> |Adição de uma caixa de correio à conta do representante.  <br/> |
   
## <a name="see-also"></a>Também consulte


- [Acesso de representante e EWS no Exchange](delegate-access-and-ews-in-exchange.md)
    
- [Ferramentas e recursos para a solução de problemas de aplicativos do EWS para Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

