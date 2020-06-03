---
title: Representação e EWS no Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: 7e1ea63c-eb29-43d2-827f-2f2b1846483b
description: Saiba como e quando usar a representação em seus aplicativos de serviço do Exchange.
localization_priority: Priority
ms.openlocfilehash: 8151b3d83421786d99ee0c82eaf4f7a5c0721f25
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466609"
---
# <a name="impersonation-and-ews-in-exchange"></a>Representação e EWS no Exchange

Saiba como e quando usar a representação em seus [aplicativos de serviço](ews-application-types.md)do Exchange.
  
Você pode permitir que os usuários acessem caixas de correio de outros usuários de uma destas três maneiras:
  
- Adicionando delegados e especificando permissões para cada representante.
    
- Modificando as permissões de pasta diretamente.
    
- Usando a representação.
    
Quando você deve escolher a representação sobre as permissões de delegação ou de pasta? As diretrizes a seguir ajudarão você a decidir:
  
- Use permissões de pasta quando quiser fornecer acesso de usuário a uma pasta, mas não quiser que o usuário tenha permissões "enviar em nome de". 
    
- Use o acesso de representante quando quiser conceder a um usuário permissão para executar o trabalho em nome de outro usuário. Normalmente, essa é uma permissão de um-para-um ou um-para-alguns-por exemplo, um único assistente administrativo Gerenciando o calendário de um administrador ou um único Agendador de sala gerenciando os calendários para um grupo de salas de reunião.
    
- Use a representação quando você tem um aplicativo de serviço que precisa acessar várias caixas de correio e "atuar como" o proprietário da caixa de correio.
    
A representação é a melhor opção quando você está lidando com várias caixas de correio, pois pode facilmente conceder acesso a uma conta de serviço a cada caixa de correio em um banco de dados. As permissões de delegação e de pasta são melhores quando você só concede acesso a alguns usuários, pois você precisa adicionar permissões individualmente a cada caixa de correio. A Figura 1 mostra algumas das diferenças entre cada tipo de acesso.
  
**Figura 1. Maneiras de acessar caixas de correio de outros usuários**

![Diagrama que mostra tipos de acesso de caixa de correio, a relação entre proprietários de caixa de correio e o representante para cada tipo e o tipo de permissão. Permissões Enviar em nome de para permissões de delegação e/ou pastas. Permissões Enviar como para representação.](media/Ex15_Delegate_Overview.png)
  
A representação é ideal para aplicativos que se conectam ao Exchange Online, Exchange Online como parte do Office 365 e versões locais do Exchange e executam operações, como o arquivamento de email, a configuração automática de OOF para usuários de férias ou qualquer outra tarefa que exija que o aplicativo atue como o proprietário de uma caixa de correio. Quando um aplicativo usa representação para enviar uma mensagem, o email parece ser enviado do proprietário da caixa de correio. Não é possível que o destinatário saiba que o email foi enviado pela conta de serviço. A delegação, por outro lado, oferece a outra permissão de conta de caixa de correio para agir em nome de um proprietário de caixa de correio. Quando uma mensagem de email é enviada por um representante, o valor "de" identifica o proprietário da caixa de correio e o valor "Sender" identifica o representante que enviou o email. 
  
## <a name="security-considerations-for-impersonation"></a>Considerações de segurança para representação

A representação permite que o chamador represente uma determinada conta de usuário. Isso permite que o chamador realize operações usando as permissões que estão associadas à conta representada, em vez das permissões que estão associadas à conta do chamador. Por esse motivo, você deve estar ciente das seguintes considerações de segurança:
  
- Somente as contas que receberam a função **ApplicationImpersonation** por um administrador do Exchange Server podem usar representação. 
    
- Você deve criar um escopo de gerenciamento que limita a representação a um grupo de contas especificado. Se você não criar um escopo de gerenciamento, a função **ApplicationImpersonation** será concedida a todas as contas de uma organização. 
    
- Normalmente, a função **ApplicationImpersonation** é concedida a uma conta de serviço dedicada a um determinado aplicativo ou grupo de aplicativos, em vez de uma conta de usuário. Você pode criar quantas contas de serviço forem necessárias. 
    
Você pode ler mais sobre como [Configurar a representação](how-to-configure-impersonation.md), mas você deve trabalhar com seu administrador do Exchange para garantir que as contas de serviço que você precisa são criadas com as [permissões e o acesso](https://technet.microsoft.com/library/dd351175%28v=exchg.150%29.aspx) que atendem aos requisitos de segurança da sua organização. 
  
## <a name="in-this-section"></a>Nesta seção

- [Configurar representação](how-to-configure-impersonation.md)
    
- [Identificar a conta a ser representada](how-to-identify-the-account-to-impersonate.md)
    
- [Adicionar compromissos usando a representação do Exchange](how-to-add-appointments-by-using-exchange-impersonation.md)
    
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Acesso de representante e EWS no Exchange](delegate-access-and-ews-in-exchange.md)
    
- [Permissões do Exchange 2013](https://technet.microsoft.com/library/dd351175%28v=exchg.150%29.aspx)
    

