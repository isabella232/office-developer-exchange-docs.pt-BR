---
title: Representação e EWS no Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7e1ea63c-eb29-43d2-827f-2f2b1846483b
description: Saiba como e quando usar representação em seus aplicativos de serviço do Exchange.
ms.openlocfilehash: f8a215874475034f0d147b80a05cae414e6438f9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750841"
---
# <a name="impersonation-and-ews-in-exchange"></a>Representação e EWS no Exchange

Saiba como e quando usar representação em seus [aplicativos de serviço](ews-application-types.md)do Exchange.
  
Você pode permitir que os usuários acessem caixas de correio de outros usuários em uma destas três formas:
  
- Adicionando representantes e especificando permissões para cada delegado.
    
- Modificando permissões da pasta diretamente.
    
- Usando representação.
    
Quando você deve escolher representação sobre as permissões de pasta ou delegação? As diretrizes a seguir ajudarão você a decidir:
  
- Use as permissões da pasta quando você deseja fornecer um acesso de usuário para uma pasta, mas não quiser que o usuário a ter permissões "Enviar em nome de". 
    
- Use o acesso de representante quando você deseja conceder a um usuário permissão para executar o trabalho em nome de outro usuário. Geralmente, isso é uma permissão de um para um ou de um para alguns - por exemplo, um assistente administrativo único Gerenciando o calendário para um administrador ou um agendador de sala único Gerenciando os calendários para um grupo de salas de reunião.
    
- Use a representação quando você tem um aplicativo de serviço que precisam de acesso a várias caixas de correio e "agir como" o proprietário da caixa de correio.
    
Representação é a melhor escolha quando você está lidando com várias caixas de correio, pois você pode facilmente conceder um acesso de conta de serviço para cada caixa de correio em um banco de dados. Permissões de pasta e delegação são recomendadas quando somente você está concedendo acesso para alguns usuários, porque você precisou para adicionar permissões individualmente para cada caixa de correio. A Figura 1 mostra algumas das diferenças entre cada tipo de acesso.
  
**Figura 1. Maneiras de acessar caixas de correio de outros usuários**

![Diagrama que mostra tipos de acesso de caixa de correio, a relação entre proprietários de caixa de correio e o representante para cada tipo e o tipo de permissão. Permissões Enviar em nome de para permissões de delegação e/ou pastas. Permissões Enviar como para representação.](media/Ex15_Delegate_Overview.png)
  
Representação é ideal para aplicativos que se conectam ao Exchange Online, Exchange Online como parte do Office 365, e versões do Exchange no local e executar operações, como o arquivamento de email, configuração OOF automaticamente para usuários de férias ou qualquer outra tarefa que requer que o aplicativo agir como o proprietário de uma caixa de correio. Quando um aplicativo usa a representação para enviar uma mensagem, o email aparece sejam enviadas do proprietário da caixa de correio. Não há um meio para o destinatário saber que o email foi enviado pela conta de serviço. Delegação, por outro lado, oferece outra permissão de conta de caixa de correio ajam em nome de um proprietário de caixa de correio. Quando uma mensagem de email é enviada por um representante, o valor "de" identifica o proprietário da caixa de correio e o valor de "remetente" identifica o representante que enviou um email. 
  
## <a name="security-considerations-for-impersonation"></a>Considerações de segurança para representação

Representação permite que um chamador representar uma conta de usuário específico. Isso permite que o chamador executar operações usando as permissões que estão associadas a conta representada, em vez das permissões que estão associados a conta do chamador. Por esse motivo, você deve estar ciente das considerações de segurança a seguir:
  
- Somente as contas que tiverem sido concedidas a função **ApplicationImpersonation** por um administrador do Exchange server podem usar representação. 
    
- Você deve criar um escopo de gerenciamento que limita a representação para um grupo especificado de contas. Se você não criar um escopo de gerenciamento, a função **ApplicationImpersonation** é concedida a todas as contas em uma organização. 
    
- Geralmente, a função **ApplicationImpersonation** é concedida a uma conta de serviço dedicada a um determinado aplicativo ou grupo de aplicativos, em vez de uma conta de usuário. Você pode criar quantos ou poucas contas de serviço conforme necessário. 
    
Você pode ler mais sobre [Configurar representação](how-to-configure-impersonation.md), mas você devem trabalhar com o administrador do Exchange para garantir que as contas de serviço que você precisa são criadas com o [acesso e permissões](http://technet.microsoft.com/en-us/library/dd351175%28v=exchg.150%29.aspx) que atendem aos requisitos de segurança de sua organização. 
  
## <a name="in-this-section"></a>Nesta se��o

- [Configurar representação](how-to-configure-impersonation.md)
    
- [Identificar a conta para representar](how-to-identify-the-account-to-impersonate.md)
    
- [Adicione os compromissos, usando a representação do Exchange](how-to-add-appointments-by-using-exchange-impersonation.md)
    
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Acesso de representante e EWS no Exchange](delegate-access-and-ews-in-exchange.md)
    
- [Permissões do Exchange 2013](http://technet.microsoft.com/en-us/library/dd351175%28v=exchg.150%29.aspx)
    

