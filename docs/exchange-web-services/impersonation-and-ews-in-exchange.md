---
title: Representação e EWS no Exchange
manager: sethgros
ms.date: 08/24/2020
ms.audience: Developer
ms.assetid: 7e1ea63c-eb29-43d2-827f-2f2b1846483b
description: Saiba como e quando usar a representação em seus aplicativos de serviço do Exchange.
localization_priority: Priority
ms.openlocfilehash: da35fb04f316c21a1c85c71b789b7f1485653466
ms.sourcegitcommit: 636c05a929279812c6ef87d75b01c166a4a05584
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/26/2020
ms.locfileid: "47254969"
---
# <a name="impersonation-and-ews-in-exchange"></a>Representação e EWS no Exchange

Saiba como e quando usar a representação em seus [aplicativos de serviço](ews-application-types.md) do Exchange.
  
Você pode permitir que os usuários acessem as caixas de correio de outros usuários de três maneiras:
  
- Adicionando representantes e especificando permissões para cada representante.
    
- Modificando as permissões de pasta diretamente.
    
- Usando a representação.
    
Quando você deve escolher a representação em vez de delegação ou permissões da pasta? As orientações a seguir ajudarão você a decidir:
  
- Use as permissões de pasta quando desejar fornecer acesso a uma pasta para um usuário, mas não quiser que o usuário tenha permissões "enviar em nome de". 
    
- Use o acesso de representante quando desejar dar permissão a um usuário para realizar o trabalho em nome de outro usuário. Geralmente, essa é uma permissão individual ou de um indivíduo para poucos. Por exemplo, um único assistente administrativo gerenciando o calendário de um administrador, ou um único agendador de sala gerenciando os calendários para um grupo de salas de reunião.
    
- Use a representação quando você tiver um aplicativo de serviço que precisa acessar várias caixas de correio e "atua como" o proprietário da caixa de correio.
    
A representação é a melhor opção quando você lida com várias caixas de correio porque pode conceder acesso a uma conta de serviço para cada caixa de correio em um banco de dados. A delegação e as permissões da pasta são melhores quando você concede acesso a apenas alguns usuários, pois tem que adicionar permissões individualmente a cada caixa de correio. A Figura 1 mostra algumas das diferenças entre cada tipo de acesso.
  
**Figura 1. Maneiras de acessar as caixas de correio de outros usuários**

![Diagrama que mostra tipos de acesso de caixa de correio, a relação entre proprietários de caixa de correio e o representante para cada tipo e o tipo de permissão. Permissões Enviar em nome de para permissões de delegação e/ou pastas. Permissões Enviar como para representação.](media/Ex15_Delegate_Overview.png)
  
A representação é ideal para aplicativos que se conectam ao Exchange Online, o Exchange Online como parte do Office 365, e as versões locais do Exchange, e realizam operações como arquivar emails, configurar a OOF automaticamente para os usuários em férias, ou qualquer outra tarefa que exija que o aplicativo atue como o proprietário de uma caixa de correio. Quando um aplicativo usa a representação para enviar uma mensagem, o email parece ser enviado do proprietário da caixa de correio. Não é possível que o destinatário saiba que o email foi enviado pela conta de serviço. As delegações, por outro lado, oferecem permissão a outra conta de caixa de correio para agir em nome de um proprietário de caixa de correio. Quando uma mensagem de email é enviada por um representante, o valor "de" identifica o proprietário da caixa de correio e o valor de "remetente" identifica o representante que enviou o email. 
  
## <a name="security-considerations-for-impersonation"></a>Considerações de segurança para a representação

A representação permite que um chamador represente uma determinada conta de usuário. Isso permite que o chamador realize operações usando as permissões associadas à conta personificada, em vez das permissões associadas à conta do chamador. Por esse motivo, você deverá estar ciente das seguintes considerações de segurança:
  
- Somente as contas que receberam a função **ApplicationImpersonation** de um administrador do Exchange Server podem usar a representação. 
    
- Você deve criar um escopo de gerenciamento que limita a representação a um grupo especificado de contas. Se você não criar um escopo de gerenciamento, a função **ApplicationImpersonation** será concedida a todas as contas de uma organização. 
    
- Geralmente, a função **ApplicationImpersonation** é concedida a uma conta de serviço dedicada a um determinado aplicativo ou grupo de aplicativos, em vez de uma conta de usuário. Você pode criar quantas contas de serviços forem necessárias. 
    
Você pode ler mais sobre [configurando a representação](how-to-configure-impersonation.md), mas você deve trabalhar com o administrador do Exchange para garantir que as contas de serviço necessárias sejam criadas com as [permissões e acessos](https://technet.microsoft.com/library/dd351175%28v=exchg.150%29.aspx) que atendam aos requisitos de segurança da sua organização. 
  
## <a name="in-this-section"></a>Nesta seção

- [Configurar a representação](how-to-configure-impersonation.md)
    
- [Identificar a conta a ser representada](how-to-identify-the-account-to-impersonate.md)
    
- [Adicionar compromissos usando a representação do Exchange](how-to-add-appointments-by-using-exchange-impersonation.md)

## <a name="performance-considerations-for-ews-impersonation"></a>Considerações de desempenho para a representação do EWS

Quando a representação do EWS é usada, o X-AnchorMailbox sempre deve ser definido corretamente.  Caso contrário, você poderá receber mensagens de erro 500 ou 503. É fundamental para o desempenho e para obter notificações com o Exchange Online/Exchange 2013.  Não configurá-lo pode dobrar ou triplicar o tempo necessário para concluir a chamada. Em alguns casos, você também pode obter um esgotamento do tempo. 
    
## <a name="see-also"></a>Confira também


- [Desenvolver clientes do serviço Web para o Exchange](develop-web-service-clients-for-exchange.md)
    
- [Acesso de representante e EWS no Exchange](delegate-access-and-ews-in-exchange.md)
    
- [Permissões do Exchange 2013](https://technet.microsoft.com/library/dd351175%28v=exchg.150%29.aspx)
    

