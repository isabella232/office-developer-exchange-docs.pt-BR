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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466609"
---
# <a name="impersonation-and-ews-in-exchange"></a><span data-ttu-id="f3e77-103">Representação e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f3e77-103">Impersonation and EWS in Exchange</span></span>

<span data-ttu-id="f3e77-104">Saiba como e quando usar a representação em seus [aplicativos de serviço](ews-application-types.md)do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3e77-104">Learn how and when to use impersonation in your Exchange [service applications](ews-application-types.md).</span></span>
  
<span data-ttu-id="f3e77-105">Você pode permitir que os usuários acessem caixas de correio de outros usuários de uma destas três maneiras:</span><span class="sxs-lookup"><span data-stu-id="f3e77-105">You can enable users to access other users' mailboxes in one of three ways:</span></span>
  
- <span data-ttu-id="f3e77-106">Adicionando delegados e especificando permissões para cada representante.</span><span class="sxs-lookup"><span data-stu-id="f3e77-106">By adding delegates and specifying permissions for each delegate.</span></span>
    
- <span data-ttu-id="f3e77-107">Modificando as permissões de pasta diretamente.</span><span class="sxs-lookup"><span data-stu-id="f3e77-107">By modifying folder permissions directly.</span></span>
    
- <span data-ttu-id="f3e77-108">Usando a representação.</span><span class="sxs-lookup"><span data-stu-id="f3e77-108">By using impersonation.</span></span>
    
<span data-ttu-id="f3e77-109">Quando você deve escolher a representação sobre as permissões de delegação ou de pasta?</span><span class="sxs-lookup"><span data-stu-id="f3e77-109">When should you choose impersonation over delegation or folder permissions?</span></span> <span data-ttu-id="f3e77-110">As diretrizes a seguir ajudarão você a decidir:</span><span class="sxs-lookup"><span data-stu-id="f3e77-110">The following guidelines will help you decide:</span></span>
  
- <span data-ttu-id="f3e77-111">Use permissões de pasta quando quiser fornecer acesso de usuário a uma pasta, mas não quiser que o usuário tenha permissões "enviar em nome de".</span><span class="sxs-lookup"><span data-stu-id="f3e77-111">Use folder permissions when you want to provide a user access to a folder but do not want the user to have "send on behalf of" permissions.</span></span> 
    
- <span data-ttu-id="f3e77-112">Use o acesso de representante quando quiser conceder a um usuário permissão para executar o trabalho em nome de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="f3e77-112">Use delegate access when you want to give one user permission to perform work on behalf of another user.</span></span> <span data-ttu-id="f3e77-113">Normalmente, essa é uma permissão de um-para-um ou um-para-alguns-por exemplo, um único assistente administrativo Gerenciando o calendário de um administrador ou um único Agendador de sala gerenciando os calendários para um grupo de salas de reunião.</span><span class="sxs-lookup"><span data-stu-id="f3e77-113">Typically, this is a one-to-one or one-to-a-few permission - for example, a single administrative assistant managing the calendar for an administrator, or a single room scheduler managing the calendars for a group of meeting rooms.</span></span>
    
- <span data-ttu-id="f3e77-114">Use a representação quando você tem um aplicativo de serviço que precisa acessar várias caixas de correio e "atuar como" o proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f3e77-114">Use impersonation when you have a service application that needs to access multiple mailboxes and "act as" the mailbox owner.</span></span>
    
<span data-ttu-id="f3e77-115">A representação é a melhor opção quando você está lidando com várias caixas de correio, pois pode facilmente conceder acesso a uma conta de serviço a cada caixa de correio em um banco de dados.</span><span class="sxs-lookup"><span data-stu-id="f3e77-115">Impersonation is the best choice when you're dealing with multiple mailboxes because you can easily grant one service account access to every mailbox in a database.</span></span> <span data-ttu-id="f3e77-116">As permissões de delegação e de pasta são melhores quando você só concede acesso a alguns usuários, pois você precisa adicionar permissões individualmente a cada caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f3e77-116">Delegation and folder permissions are best when you're only granting access to a few users, because you have to add permissions individually to each mailbox.</span></span> <span data-ttu-id="f3e77-117">A Figura 1 mostra algumas das diferenças entre cada tipo de acesso.</span><span class="sxs-lookup"><span data-stu-id="f3e77-117">Figure 1 shows some of the differences between each type of access.</span></span>
  
<span data-ttu-id="f3e77-118">**Figura 1. Maneiras de acessar caixas de correio de outros usuários**</span><span class="sxs-lookup"><span data-stu-id="f3e77-118">**Figure 1. Ways to access other users' mailboxes**</span></span>

![Diagrama que mostra tipos de acesso de caixa de correio, a relação entre proprietários de caixa de correio e o representante para cada tipo e o tipo de permissão. Permissões Enviar em nome de para permissões de delegação e/ou pastas. Permissões Enviar como para representação.](media/Ex15_Delegate_Overview.png)
  
<span data-ttu-id="f3e77-122">A representação é ideal para aplicativos que se conectam ao Exchange Online, Exchange Online como parte do Office 365 e versões locais do Exchange e executam operações, como o arquivamento de email, a configuração automática de OOF para usuários de férias ou qualquer outra tarefa que exija que o aplicativo atue como o proprietário de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f3e77-122">Impersonation is ideal for applications that connect to Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange and perform operations, such as archiving email, setting OOF automatically for users on vacation, or any other task that requires that the application act as the owner of a mailbox.</span></span> <span data-ttu-id="f3e77-123">Quando um aplicativo usa representação para enviar uma mensagem, o email parece ser enviado do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f3e77-123">When an application uses impersonation to send a message, the email appears to be sent from the mailbox owner.</span></span> <span data-ttu-id="f3e77-124">Não é possível que o destinatário saiba que o email foi enviado pela conta de serviço.</span><span class="sxs-lookup"><span data-stu-id="f3e77-124">There is no way for the recipient to know the mail was sent by the service account.</span></span> <span data-ttu-id="f3e77-125">A delegação, por outro lado, oferece a outra permissão de conta de caixa de correio para agir em nome de um proprietário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f3e77-125">Delegation, on the other hand, gives another mailbox account permission to act on behalf of a mailbox owner.</span></span> <span data-ttu-id="f3e77-126">Quando uma mensagem de email é enviada por um representante, o valor "de" identifica o proprietário da caixa de correio e o valor "Sender" identifica o representante que enviou o email.</span><span class="sxs-lookup"><span data-stu-id="f3e77-126">When an email message is sent by a delegate, the "from" value identifies the mailbox owner, and the "sender" value identifies the delegate that sent the mail.</span></span> 
  
## <a name="security-considerations-for-impersonation"></a><span data-ttu-id="f3e77-127">Considerações de segurança para representação</span><span class="sxs-lookup"><span data-stu-id="f3e77-127">Security considerations for impersonation</span></span>

<span data-ttu-id="f3e77-128">A representação permite que o chamador represente uma determinada conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="f3e77-128">Impersonation enables a caller to impersonate a given user account.</span></span> <span data-ttu-id="f3e77-129">Isso permite que o chamador realize operações usando as permissões que estão associadas à conta representada, em vez das permissões que estão associadas à conta do chamador.</span><span class="sxs-lookup"><span data-stu-id="f3e77-129">This enables the caller to perform operations by using the permissions that are associated with the impersonated account, instead of the permissions that are associated with the caller's account.</span></span> <span data-ttu-id="f3e77-130">Por esse motivo, você deve estar ciente das seguintes considerações de segurança:</span><span class="sxs-lookup"><span data-stu-id="f3e77-130">For this reason, you should be aware of the following security considerations:</span></span>
  
- <span data-ttu-id="f3e77-131">Somente as contas que receberam a função **ApplicationImpersonation** por um administrador do Exchange Server podem usar representação.</span><span class="sxs-lookup"><span data-stu-id="f3e77-131">Only accounts that have been granted the **ApplicationImpersonation** role by an Exchange server administrator can use impersonation.</span></span> 
    
- <span data-ttu-id="f3e77-132">Você deve criar um escopo de gerenciamento que limita a representação a um grupo de contas especificado.</span><span class="sxs-lookup"><span data-stu-id="f3e77-132">You should create a management scope that limits impersonation to a specified group of accounts.</span></span> <span data-ttu-id="f3e77-133">Se você não criar um escopo de gerenciamento, a função **ApplicationImpersonation** será concedida a todas as contas de uma organização.</span><span class="sxs-lookup"><span data-stu-id="f3e77-133">If you do not create a management scope, the **ApplicationImpersonation** role is granted to all accounts in an organization.</span></span> 
    
- <span data-ttu-id="f3e77-134">Normalmente, a função **ApplicationImpersonation** é concedida a uma conta de serviço dedicada a um determinado aplicativo ou grupo de aplicativos, em vez de uma conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="f3e77-134">Typically, the **ApplicationImpersonation** role is granted to a service account dedicated to a particular application or group of applications, rather than a user account.</span></span> <span data-ttu-id="f3e77-135">Você pode criar quantas contas de serviço forem necessárias.</span><span class="sxs-lookup"><span data-stu-id="f3e77-135">You can create as many or as few service accounts as you need.</span></span> 
    
<span data-ttu-id="f3e77-136">Você pode ler mais sobre como [Configurar a representação](how-to-configure-impersonation.md), mas você deve trabalhar com seu administrador do Exchange para garantir que as contas de serviço que você precisa são criadas com as [permissões e o acesso](https://technet.microsoft.com/library/dd351175%28v=exchg.150%29.aspx) que atendem aos requisitos de segurança da sua organização.</span><span class="sxs-lookup"><span data-stu-id="f3e77-136">You can read more about [configuring impersonation](how-to-configure-impersonation.md), but you should work with your Exchange administrator to ensure that the service accounts that you need are created with the [permissions and access](https://technet.microsoft.com/library/dd351175%28v=exchg.150%29.aspx) that meet the security requirements of your organization.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="f3e77-137">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="f3e77-137">In this section</span></span>

- [<span data-ttu-id="f3e77-138">Configurar representação</span><span class="sxs-lookup"><span data-stu-id="f3e77-138">Configure impersonation</span></span>](how-to-configure-impersonation.md)
    
- [<span data-ttu-id="f3e77-139">Identificar a conta a ser representada</span><span class="sxs-lookup"><span data-stu-id="f3e77-139">Identify the account to impersonate</span></span>](how-to-identify-the-account-to-impersonate.md)
    
- [<span data-ttu-id="f3e77-140">Adicionar compromissos usando a representação do Exchange</span><span class="sxs-lookup"><span data-stu-id="f3e77-140">Add appointments by using Exchange impersonation</span></span>](how-to-add-appointments-by-using-exchange-impersonation.md)
    
## <a name="see-also"></a><span data-ttu-id="f3e77-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="f3e77-141">See also</span></span>


- [<span data-ttu-id="f3e77-142">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="f3e77-142">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="f3e77-143">Acesso de representante e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f3e77-143">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f3e77-144">Permissões do Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="f3e77-144">Exchange 2013 Permissions</span></span>](https://technet.microsoft.com/library/dd351175%28v=exchg.150%29.aspx)
    

