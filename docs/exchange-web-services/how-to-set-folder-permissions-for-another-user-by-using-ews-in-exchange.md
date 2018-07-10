---
title: Definir permissões de pasta para outro usuário usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7eb81676-a780-4c56-b4f2-c4ed2697107d
description: Saiba como definir níveis de permissão em uma pasta usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 5bf570612d6349628e7f3abf858daa33daa13745
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750830"
---
# <a name="set-folder-permissions-for-another-user-by-using-ews-in-exchange"></a><span data-ttu-id="348a3-103">Definir permissões de pasta para outro usuário usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="348a3-103">Set folder permissions for another user by using EWS in Exchange</span></span>

<span data-ttu-id="348a3-104">Saiba como definir níveis de permissão em uma pasta usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="348a3-104">Learn how to set permission levels on a folder by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="348a3-105">Permissões de nível de pasta permitem que os usuários acessem uma ou mais pastas na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="348a3-105">Folder-level permissions enable users to access one or more folders in another user's mailbox.</span></span> <span data-ttu-id="348a3-106">Permissões da pasta são semelhantes às Delegar acesso, mas diferem das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="348a3-106">Folder permissions are similar to delegate access, but they differ in the following ways:</span></span> 
  
- <span data-ttu-id="348a3-107">Permissões da pasta não permitir que um usuário "Enviar em nome de" ou "Enviar como" outro usuário.</span><span class="sxs-lookup"><span data-stu-id="348a3-107">Folder permissions do not enable a user to "send on behalf of" or "send as" another user.</span></span> <span data-ttu-id="348a3-108">Eles só pode ativar o acesso às pastas.</span><span class="sxs-lookup"><span data-stu-id="348a3-108">They only enable access to folders.</span></span> <span data-ttu-id="348a3-109">Os usuários podem criar itens nessas pastas, mas eles não podem enviá-los.</span><span class="sxs-lookup"><span data-stu-id="348a3-109">Users can create items in those folders, but they can't send them.</span></span>
    
- <span data-ttu-id="348a3-110">Você pode definir permissões de pasta em qualquer pasta na caixa de correio, mas você só pode adicionar um representante para as pastas de calendário, contatos, caixa de entrada, diário, anotações e tarefas.</span><span class="sxs-lookup"><span data-stu-id="348a3-110">You can set folder permissions on any folder in the mailbox, but you can only add a delegate to the Calendar, Contacts, Inbox, Journal, Notes, and Tasks folders.</span></span>
    
- <span data-ttu-id="348a3-111">Você pode definir um número de [permissões em uma pasta específica](#bk_folderperms).</span><span class="sxs-lookup"><span data-stu-id="348a3-111">You can set a number of [permissions on a specific folder](#bk_folderperms).</span></span> <span data-ttu-id="348a3-112">Quando você adiciona um representante, você pode atribuir um dos [cinco níveis de permissão](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span><span class="sxs-lookup"><span data-stu-id="348a3-112">When you add a delegate, you can assign one of only [five permission levels](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span></span>
    
- <span data-ttu-id="348a3-113">Você pode definir permissões da pasta para anônimos e usuários de padrão.</span><span class="sxs-lookup"><span data-stu-id="348a3-113">You can set folder permissions for anonymous and default users.</span></span> <span data-ttu-id="348a3-114">Você só pode conceder acesso de representante para uma conta habilitada para email.</span><span class="sxs-lookup"><span data-stu-id="348a3-114">You can only grant delegate access to a mail-enabled account.</span></span>
    
<span data-ttu-id="348a3-115">Se você estiver familiarizado com as entradas de controle de acesso (ACEs) e controle de acesso discricionário listas (DACLs), você sabe que um usuário pode ter apenas um conjunto de permissões para cada pasta.</span><span class="sxs-lookup"><span data-stu-id="348a3-115">If you're familiar with Access Control Entries (ACEs) and Discretionary Access Control Lists (DACLs), you know that a user can only have one set of permissions for each folder.</span></span> <span data-ttu-id="348a3-116">Se você tentar adicionar um conjunto de permissões para um usuário e já tenham um conjunto de permissões, você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="348a3-116">If you try to add a set of permissions for a user and they already have a set of permissions, you'll get an error.</span></span> <span data-ttu-id="348a3-117">Quando você adicionar, remove ou atualizar permissões em uma pasta, você fazer a DACL atual, adicionar ou remove qualquer ACEs e envie a DACL atualizada.</span><span class="sxs-lookup"><span data-stu-id="348a3-117">When you add, remove, or update permissions on a folder, you get the current DACL, add or remove any ACEs, and then send the updated DACL.</span></span> <span data-ttu-id="348a3-118">Não é possível adicionar vários ACEs para o mesmo usuário.</span><span class="sxs-lookup"><span data-stu-id="348a3-118">You cannot add multiple ACEs for the same user.</span></span> <span data-ttu-id="348a3-119">Quando você atualizar permissões usando a API gerenciada de EWS, você precisa remover ACE do usuário atual e, em seguida, adicionar seu ACE nova à coleção.</span><span class="sxs-lookup"><span data-stu-id="348a3-119">When you update permissions by using the EWS Managed API, you need to remove the user's current ACE and then add their new ACE to the collection.</span></span> <span data-ttu-id="348a3-120">Se você estiver usando o EWS, apenas substitua o conjunto de ACEs anterior com as novas.</span><span class="sxs-lookup"><span data-stu-id="348a3-120">If you're using EWS, you just replace the previous set of ACEs with the new ones.</span></span>
  
<span data-ttu-id="348a3-121">Se você estiver fazendo várias alterações de permissão para uma única pasta, você pode lote adições, remoções ou atualizações — apenas Observe que você não pode atualizações do usuário em várias pastas de lote.</span><span class="sxs-lookup"><span data-stu-id="348a3-121">If you're making multiple permission changes to a single folder, you can batch additions, removals, or updates —just note that you cannot batch user updates on multiple folders.</span></span> <span data-ttu-id="348a3-122">Uma chamada é necessário para obter as permissões em uma única pasta e uma segunda chamada é necessária para atualizar as permissões dessa pasta.</span><span class="sxs-lookup"><span data-stu-id="348a3-122">One call is required to get the permissions on a single folder, and a second call is required to update the permissions on that folder.</span></span> <span data-ttu-id="348a3-123">Quando você adicionar, remove ou atualizar as permissões de usuário, você deve usar o mesmo método de duas chamadas ou operações para cada tarefa.</span><span class="sxs-lookup"><span data-stu-id="348a3-123">When you add, remove, or update user permissions, you use the same two method calls or operations for each task.</span></span>
  
<span data-ttu-id="348a3-124">**Tabela 1. Métodos de API gerenciada de EWS e operações de EWS para configurar permissões de pasta**</span><span class="sxs-lookup"><span data-stu-id="348a3-124">**Table 1. EWS Managed API methods and EWS operations for setting folder permissions**</span></span>

|<span data-ttu-id="348a3-125">Se você quiser …</span><span class="sxs-lookup"><span data-stu-id="348a3-125">If you want to…</span></span>|<span data-ttu-id="348a3-126">Use este método de API gerenciada de EWS …</span><span class="sxs-lookup"><span data-stu-id="348a3-126">Use this EWS Managed API method…</span></span>|<span data-ttu-id="348a3-127">Use essa operação EWS …</span><span class="sxs-lookup"><span data-stu-id="348a3-127">Use this EWS operation…</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="348a3-128">Habilitar, remover ou atualizar as permissões de pasta</span><span class="sxs-lookup"><span data-stu-id="348a3-128">Enable, remove, or update folder permissions</span></span>  <br/> |<span data-ttu-id="348a3-129">[Folder.Bind](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) seguido [Folder.Update](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="348a3-129">[Folder.Bind](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) followed by [Folder.Update](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="348a3-130">[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) seguido [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="348a3-130">[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) followed by [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="348a3-131">Crie uma pasta e definir permissões de pasta</span><span class="sxs-lookup"><span data-stu-id="348a3-131">Create a folder and define folder permissions</span></span>  <br/> |[<span data-ttu-id="348a3-132">Folder.Save</span><span class="sxs-lookup"><span data-stu-id="348a3-132">Folder.Save</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="348a3-133">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="348a3-133">CreateFolder</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
   
## <a name="folder-permissions"></a><span data-ttu-id="348a3-134">Permissões de pasta</span><span class="sxs-lookup"><span data-stu-id="348a3-134">Folder permissions</span></span>
<span data-ttu-id="348a3-135"><a name="bk_folderperms"> </a></span><span class="sxs-lookup"><span data-stu-id="348a3-135"></span></span>

<span data-ttu-id="348a3-136">Há algumas opções que diz respeito à definição de permissões de pasta em uma pasta específica.</span><span class="sxs-lookup"><span data-stu-id="348a3-136">You have quite a few options when it comes to setting folder permissions on a specific folder.</span></span> <span data-ttu-id="348a3-137">Você pode definir um nível de permissão em uma pasta para cada usuário, que adiciona um conjunto de permissões individuais predefinidos à DACL, ou você pode definir permissões individuais em uma pasta — mas não é possível misturar e corresponder.</span><span class="sxs-lookup"><span data-stu-id="348a3-137">You can set a permission level on a folder for each user, which adds a set of predefined individual permissions to the DACL, or you can set individual permissions on a folder — but you can't mix and match.</span></span>
  
<span data-ttu-id="348a3-138">As seguintes permissões individuais estão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="348a3-138">The following individual permissions are available:</span></span>
  
- <span data-ttu-id="348a3-139">Pode criar</span><span class="sxs-lookup"><span data-stu-id="348a3-139">Can create</span></span>
- <span data-ttu-id="348a3-140">Pode criar subpastas</span><span class="sxs-lookup"><span data-stu-id="348a3-140">Can create subfolders</span></span>    
- <span data-ttu-id="348a3-141">É o proprietário da pasta</span><span class="sxs-lookup"><span data-stu-id="348a3-141">Is folder owner</span></span>    
- <span data-ttu-id="348a3-142">Pasta está visível</span><span class="sxs-lookup"><span data-stu-id="348a3-142">Is folder visible</span></span>    
- <span data-ttu-id="348a3-143">É o contato da pasta</span><span class="sxs-lookup"><span data-stu-id="348a3-143">Is folder contact</span></span>    
- <span data-ttu-id="348a3-144">Editar itens</span><span class="sxs-lookup"><span data-stu-id="348a3-144">Edit items</span></span>    
- <span data-ttu-id="348a3-145">Excluir itens</span><span class="sxs-lookup"><span data-stu-id="348a3-145">Delete items</span></span>    
- <span data-ttu-id="348a3-146">Ler itens</span><span class="sxs-lookup"><span data-stu-id="348a3-146">Read items</span></span>
    
<span data-ttu-id="348a3-147">Além disso, os seguintes níveis de permissão estão disponíveis, que definem um subconjunto de permissões individuais e valores, conforme mostrado na tabela 2:</span><span class="sxs-lookup"><span data-stu-id="348a3-147">In addition, the following permission levels are available, which define a subset of individual permissions and values, as shown in Table 2:</span></span>
  
- <span data-ttu-id="348a3-148">None</span><span class="sxs-lookup"><span data-stu-id="348a3-148">None</span></span>    
- <span data-ttu-id="348a3-149">Proprietário</span><span class="sxs-lookup"><span data-stu-id="348a3-149">Owner</span></span>    
- <span data-ttu-id="348a3-150">PublishingEditor</span><span class="sxs-lookup"><span data-stu-id="348a3-150">PublishingEditor</span></span>    
- <span data-ttu-id="348a3-151">Editor</span><span class="sxs-lookup"><span data-stu-id="348a3-151">Editor</span></span>    
- <span data-ttu-id="348a3-152">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="348a3-152">PublishingAuthor</span></span>    
- <span data-ttu-id="348a3-153">Autor</span><span class="sxs-lookup"><span data-stu-id="348a3-153">Author</span></span>    
- <span data-ttu-id="348a3-154">NoneditingAuthor</span><span class="sxs-lookup"><span data-stu-id="348a3-154">NoneditingAuthor</span></span>    
- <span data-ttu-id="348a3-155">Reviewer</span><span class="sxs-lookup"><span data-stu-id="348a3-155">Reviewer</span></span>    
- <span data-ttu-id="348a3-156">Colaborador</span><span class="sxs-lookup"><span data-stu-id="348a3-156">Contributor</span></span>   
- <span data-ttu-id="348a3-157">Personalizado - este valor não pode ser definido pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="348a3-157">Custom - This value cannot be set by the application.</span></span> <span data-ttu-id="348a3-158">O servidor define esse valor se o aplicativo inclui uma coleção personalizada de permissões individuais.</span><span class="sxs-lookup"><span data-stu-id="348a3-158">The server sets this value if the application includes a custom collection of individual permissions.</span></span>    
- <span data-ttu-id="348a3-159">FreeBusyTimeOnly - isso pode apenas ser definida em pastas de calendário.</span><span class="sxs-lookup"><span data-stu-id="348a3-159">FreeBusyTimeOnly - This can only be set on Calendar folders.</span></span>   
- <span data-ttu-id="348a3-160">FreeBusyTimeAndSubjectAndLocation - isso pode apenas ser definida em pastas de calendário.</span><span class="sxs-lookup"><span data-stu-id="348a3-160">FreeBusyTimeAndSubjectAndLocation - This can only be set on Calendar folders.</span></span>
    
<span data-ttu-id="348a3-161">A tabela a seguir mostra quais permissões individuais são aplicadas por padrão, com base no nível de permissão.</span><span class="sxs-lookup"><span data-stu-id="348a3-161">The following table shows which individual permissions are applied by default based on permission level.</span></span>
  
<span data-ttu-id="348a3-162">**Tabela 2. Permissões individuais por nível de permissão**</span><span class="sxs-lookup"><span data-stu-id="348a3-162">**Table 2. Individual permissions by permission level**</span></span>

|<span data-ttu-id="348a3-163">Nível da permissão</span><span class="sxs-lookup"><span data-stu-id="348a3-163">Permission level</span></span>|<span data-ttu-id="348a3-164">Pode criar itens</span><span class="sxs-lookup"><span data-stu-id="348a3-164">Can create items</span></span>|<span data-ttu-id="348a3-165">Pode criar subpastas</span><span class="sxs-lookup"><span data-stu-id="348a3-165">Can create sub folders</span></span>|<span data-ttu-id="348a3-166">É o proprietário da pasta</span><span class="sxs-lookup"><span data-stu-id="348a3-166">Is folder owner</span></span>|<span data-ttu-id="348a3-167">Pasta está visível</span><span class="sxs-lookup"><span data-stu-id="348a3-167">Is folder visible</span></span>|<span data-ttu-id="348a3-168">É o contato da pasta</span><span class="sxs-lookup"><span data-stu-id="348a3-168">Is folder contact</span></span>|<span data-ttu-id="348a3-169">Editar itens</span><span class="sxs-lookup"><span data-stu-id="348a3-169">Edit items</span></span>|<span data-ttu-id="348a3-170">Excluir itens</span><span class="sxs-lookup"><span data-stu-id="348a3-170">Delete items</span></span>|<span data-ttu-id="348a3-171">Pode ler itens</span><span class="sxs-lookup"><span data-stu-id="348a3-171">Can read items</span></span>|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|<span data-ttu-id="348a3-172">None</span><span class="sxs-lookup"><span data-stu-id="348a3-172">None</span></span>  <br/> |<span data-ttu-id="348a3-173">False</span><span class="sxs-lookup"><span data-stu-id="348a3-173">False</span></span>  <br/> |<span data-ttu-id="348a3-174">False</span><span class="sxs-lookup"><span data-stu-id="348a3-174">False</span></span>  <br/> |<span data-ttu-id="348a3-175">False</span><span class="sxs-lookup"><span data-stu-id="348a3-175">False</span></span>  <br/> |<span data-ttu-id="348a3-176">False</span><span class="sxs-lookup"><span data-stu-id="348a3-176">False</span></span>  <br/> |<span data-ttu-id="348a3-177">False</span><span class="sxs-lookup"><span data-stu-id="348a3-177">False</span></span>  <br/> |<span data-ttu-id="348a3-178">Nenhum</span><span class="sxs-lookup"><span data-stu-id="348a3-178">None</span></span>  <br/> |<span data-ttu-id="348a3-179">Nenhum</span><span class="sxs-lookup"><span data-stu-id="348a3-179">None</span></span>  <br/> |<span data-ttu-id="348a3-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="348a3-180">None</span></span>  <br/> |
|<span data-ttu-id="348a3-181">Proprietário</span><span class="sxs-lookup"><span data-stu-id="348a3-181">Owner</span></span>  <br/> |<span data-ttu-id="348a3-182">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="348a3-182">True</span></span>  <br/> |<span data-ttu-id="348a3-183">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="348a3-183">True</span></span>  <br/> |<span data-ttu-id="348a3-184">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="348a3-184">True</span></span>  <br/> |<span data-ttu-id="348a3-185">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="348a3-185">True</span></span>  <br/> |<span data-ttu-id="348a3-186">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="348a3-186">True</span></span>  <br/> |<span data-ttu-id="348a3-187">Todos</span><span class="sxs-lookup"><span data-stu-id="348a3-187">All</span></span>  <br/> |<span data-ttu-id="348a3-188">Todos</span><span class="sxs-lookup"><span data-stu-id="348a3-188">All</span></span>  <br/> |<span data-ttu-id="348a3-189">FullDetails</span><span class="sxs-lookup"><span data-stu-id="348a3-189">FullDetails</span></span>  <br/> |
|<span data-ttu-id="348a3-190">PublishingEditor</span><span class="sxs-lookup"><span data-stu-id="348a3-190">PublishingEditor</span></span>  <br/> |<span data-ttu-id="348a3-191">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="348a3-191">True</span></span>  <br/> |<span data-ttu-id="348a3-192">True</span><span class="sxs-lookup"><span data-stu-id="348a3-192">True</span></span>  <br/> |<span data-ttu-id="348a3-193">False</span><span class="sxs-lookup"><span data-stu-id="348a3-193">False</span></span>  <br/> |<span data-ttu-id="348a3-194">True</span><span class="sxs-lookup"><span data-stu-id="348a3-194">True</span></span>  <br/> |<span data-ttu-id="348a3-195">False</span><span class="sxs-lookup"><span data-stu-id="348a3-195">False</span></span>  <br/> |<span data-ttu-id="348a3-196">Todos</span><span class="sxs-lookup"><span data-stu-id="348a3-196">All</span></span>  <br/> |<span data-ttu-id="348a3-197">Todos</span><span class="sxs-lookup"><span data-stu-id="348a3-197">All</span></span>  <br/> |<span data-ttu-id="348a3-198">FullDetails</span><span class="sxs-lookup"><span data-stu-id="348a3-198">FullDetails</span></span>  <br/> |
|<span data-ttu-id="348a3-199">Editor</span><span class="sxs-lookup"><span data-stu-id="348a3-199">Editor</span></span>  <br/> |<span data-ttu-id="348a3-200">True</span><span class="sxs-lookup"><span data-stu-id="348a3-200">True</span></span>  <br/> |<span data-ttu-id="348a3-201">False</span><span class="sxs-lookup"><span data-stu-id="348a3-201">False</span></span>  <br/> |<span data-ttu-id="348a3-202">False</span><span class="sxs-lookup"><span data-stu-id="348a3-202">False</span></span>  <br/> |<span data-ttu-id="348a3-203">True</span><span class="sxs-lookup"><span data-stu-id="348a3-203">True</span></span>  <br/> |<span data-ttu-id="348a3-204">False</span><span class="sxs-lookup"><span data-stu-id="348a3-204">False</span></span>  <br/> |<span data-ttu-id="348a3-205">Todos</span><span class="sxs-lookup"><span data-stu-id="348a3-205">All</span></span>  <br/> |<span data-ttu-id="348a3-206">Todos</span><span class="sxs-lookup"><span data-stu-id="348a3-206">All</span></span>  <br/> |<span data-ttu-id="348a3-207">FullDetails</span><span class="sxs-lookup"><span data-stu-id="348a3-207">FullDetails</span></span>  <br/> |
|<span data-ttu-id="348a3-208">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="348a3-208">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="348a3-209">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="348a3-209">True</span></span>  <br/> |<span data-ttu-id="348a3-210">True</span><span class="sxs-lookup"><span data-stu-id="348a3-210">True</span></span>  <br/> |<span data-ttu-id="348a3-211">False</span><span class="sxs-lookup"><span data-stu-id="348a3-211">False</span></span>  <br/> |<span data-ttu-id="348a3-212">True</span><span class="sxs-lookup"><span data-stu-id="348a3-212">True</span></span>  <br/> |<span data-ttu-id="348a3-213">False</span><span class="sxs-lookup"><span data-stu-id="348a3-213">False</span></span>  <br/> |<span data-ttu-id="348a3-214">Pertencentes</span><span class="sxs-lookup"><span data-stu-id="348a3-214">Owned</span></span>  <br/> |<span data-ttu-id="348a3-215">Pertencentes</span><span class="sxs-lookup"><span data-stu-id="348a3-215">Owned</span></span>  <br/> |<span data-ttu-id="348a3-216">FullDetails</span><span class="sxs-lookup"><span data-stu-id="348a3-216">FullDetails</span></span>  <br/> |
|<span data-ttu-id="348a3-217">Autor</span><span class="sxs-lookup"><span data-stu-id="348a3-217">Author</span></span>  <br/> |<span data-ttu-id="348a3-218">True</span><span class="sxs-lookup"><span data-stu-id="348a3-218">True</span></span>  <br/> |<span data-ttu-id="348a3-219">False</span><span class="sxs-lookup"><span data-stu-id="348a3-219">False</span></span>  <br/> |<span data-ttu-id="348a3-220">False</span><span class="sxs-lookup"><span data-stu-id="348a3-220">False</span></span>  <br/> |<span data-ttu-id="348a3-221">True</span><span class="sxs-lookup"><span data-stu-id="348a3-221">True</span></span>  <br/> |<span data-ttu-id="348a3-222">False</span><span class="sxs-lookup"><span data-stu-id="348a3-222">False</span></span>  <br/> |<span data-ttu-id="348a3-223">Pertencentes</span><span class="sxs-lookup"><span data-stu-id="348a3-223">Owned</span></span>  <br/> |<span data-ttu-id="348a3-224">Pertencentes</span><span class="sxs-lookup"><span data-stu-id="348a3-224">Owned</span></span>  <br/> |<span data-ttu-id="348a3-225">FullDetails</span><span class="sxs-lookup"><span data-stu-id="348a3-225">FullDetails</span></span>  <br/> |
|<span data-ttu-id="348a3-226">NoneditingAuthor</span><span class="sxs-lookup"><span data-stu-id="348a3-226">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="348a3-227">True</span><span class="sxs-lookup"><span data-stu-id="348a3-227">True</span></span>  <br/> |<span data-ttu-id="348a3-228">False</span><span class="sxs-lookup"><span data-stu-id="348a3-228">False</span></span>  <br/> |<span data-ttu-id="348a3-229">False</span><span class="sxs-lookup"><span data-stu-id="348a3-229">False</span></span>  <br/> |<span data-ttu-id="348a3-230">True</span><span class="sxs-lookup"><span data-stu-id="348a3-230">True</span></span>  <br/> |<span data-ttu-id="348a3-231">False</span><span class="sxs-lookup"><span data-stu-id="348a3-231">False</span></span>  <br/> |<span data-ttu-id="348a3-232">None</span><span class="sxs-lookup"><span data-stu-id="348a3-232">None</span></span>  <br/> |<span data-ttu-id="348a3-233">Pertencentes</span><span class="sxs-lookup"><span data-stu-id="348a3-233">Owned</span></span>  <br/> |<span data-ttu-id="348a3-234">FullDetails</span><span class="sxs-lookup"><span data-stu-id="348a3-234">FullDetails</span></span>  <br/> |
|<span data-ttu-id="348a3-235">Reviewer</span><span class="sxs-lookup"><span data-stu-id="348a3-235">Reviewer</span></span>  <br/> |<span data-ttu-id="348a3-236">False</span><span class="sxs-lookup"><span data-stu-id="348a3-236">False</span></span>  <br/> |<span data-ttu-id="348a3-237">False</span><span class="sxs-lookup"><span data-stu-id="348a3-237">False</span></span>  <br/> |<span data-ttu-id="348a3-238">False</span><span class="sxs-lookup"><span data-stu-id="348a3-238">False</span></span>  <br/> |<span data-ttu-id="348a3-239">True</span><span class="sxs-lookup"><span data-stu-id="348a3-239">True</span></span>  <br/> |<span data-ttu-id="348a3-240">False</span><span class="sxs-lookup"><span data-stu-id="348a3-240">False</span></span>  <br/> |<span data-ttu-id="348a3-241">Nenhum</span><span class="sxs-lookup"><span data-stu-id="348a3-241">None</span></span>  <br/> |<span data-ttu-id="348a3-242">Nenhum</span><span class="sxs-lookup"><span data-stu-id="348a3-242">None</span></span>  <br/> |<span data-ttu-id="348a3-243">FullDetails</span><span class="sxs-lookup"><span data-stu-id="348a3-243">FullDetails</span></span>  <br/> |
|<span data-ttu-id="348a3-244">Colaborador</span><span class="sxs-lookup"><span data-stu-id="348a3-244">Contributor</span></span>  <br/> |<span data-ttu-id="348a3-245">True</span><span class="sxs-lookup"><span data-stu-id="348a3-245">True</span></span>  <br/> |<span data-ttu-id="348a3-246">False</span><span class="sxs-lookup"><span data-stu-id="348a3-246">False</span></span>  <br/> |<span data-ttu-id="348a3-247">False</span><span class="sxs-lookup"><span data-stu-id="348a3-247">False</span></span>  <br/> |<span data-ttu-id="348a3-248">True</span><span class="sxs-lookup"><span data-stu-id="348a3-248">True</span></span>  <br/> |<span data-ttu-id="348a3-249">False</span><span class="sxs-lookup"><span data-stu-id="348a3-249">False</span></span>  <br/> |<span data-ttu-id="348a3-250">Nenhum</span><span class="sxs-lookup"><span data-stu-id="348a3-250">None</span></span>  <br/> |<span data-ttu-id="348a3-251">Nenhum</span><span class="sxs-lookup"><span data-stu-id="348a3-251">None</span></span>  <br/> |<span data-ttu-id="348a3-252">Nenhum</span><span class="sxs-lookup"><span data-stu-id="348a3-252">None</span></span>  <br/> |
   
<span data-ttu-id="348a3-253">Se você especificar um nível de permissão não personalizadas na solicitação de permissões de nível de pasta, você não precisará especificar as configurações de permissão individual.</span><span class="sxs-lookup"><span data-stu-id="348a3-253">If you specify a non-custom permission level in the folder-level permissions request, you don't need to specify the individual permission settings.</span></span> <span data-ttu-id="348a3-254">Se você especificar uma permissão individual ao definir um nível de permissão, será retornado um erro **ErrorInvalidPermissionSettings** na resposta.</span><span class="sxs-lookup"><span data-stu-id="348a3-254">If you do specify an individual permission when you set a permission level, an **ErrorInvalidPermissionSettings** error will be returned in the response.</span></span> 
  
## <a name="adding-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="348a3-255">Adicionar permissões de pasta usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="348a3-255">Adding folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="348a3-256"><a name="bk_enableewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="348a3-256"></span></span>

<span data-ttu-id="348a3-257">O exemplo de código a seguir mostra como usar a API gerenciada de EWS para:</span><span class="sxs-lookup"><span data-stu-id="348a3-257">The following code example shows how to use the EWS Managed API to:</span></span> 
  
- <span data-ttu-id="348a3-258">Crie um novo objeto de [FolderPermission](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) para o novo usuário.</span><span class="sxs-lookup"><span data-stu-id="348a3-258">Create a new [FolderPermission](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) object for the new user.</span></span> 
    
- <span data-ttu-id="348a3-259">Obtenha as permissões atuais de uma pasta usando o método [vincular](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="348a3-259">Get the current permissions for a folder by using the [Bind](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method.</span></span> 
    
- <span data-ttu-id="348a3-260">Adicione o novo **FolderPermissions** à propriedade [Folder.Permissions](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="348a3-260">Add the new **FolderPermissions** to the [Folder.Permissions](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) property.</span></span> 
    
- <span data-ttu-id="348a3-261">Chame o método [Update](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) para salvar as novas permissões no servidor.</span><span class="sxs-lookup"><span data-stu-id="348a3-261">Call the [Update](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the new permissions to the server.</span></span> 
    
<span data-ttu-id="348a3-262">Este exemplo supõe que esse **serviço** é um objeto [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o proprietário da caixa de correio e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="348a3-262">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void EnableFolderPermissions(ExchangeService service)
{
    // Create a property set to use for folder binding.
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.Permissions);
    // Specify the SMTP address of the new user and the folder permissions level.
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
    
    // Bind to the folder and get the current permissions. 
    // This call results in a GetFolder call to EWS.
    Folder sentItemsFolder = Folder.Bind(service, WellKnownFolderName.SentItems, propSet);
 
    // Add the permissions for the new user to the Sent Items DACL.
    sentItemsFolder.Permissions.Add(fldperm);
    // This call results in a UpdateFolder call to EWS.
    sentItemsFolder.Update();
}
```

<span data-ttu-id="348a3-263">A linha de código a seguir especifica o nível de permissão.</span><span class="sxs-lookup"><span data-stu-id="348a3-263">The following line of code specifies the permission level.</span></span>
  
```cs
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
```

<span data-ttu-id="348a3-264">Se você quiser usar o nível de permissão personalizado, use este código.</span><span class="sxs-lookup"><span data-stu-id="348a3-264">If you want to use the custom permission level, use this code instead.</span></span>
  
```cs
FolderPermission fldperm = new FolderPermission();
fldperm.UserId = "sadie@Contoso1000.onmicrosoft.com";
fldperm.CanCreateItems = true;
fldperm.CanCreateSubFolders = true;
…
```

<span data-ttu-id="348a3-265">Você pode definir qualquer uma ou todas as [Propriedades de FolderPermission](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) de gravável quando você cria um objeto **FolderPermission** com um nível de permissão personalizados.</span><span class="sxs-lookup"><span data-stu-id="348a3-265">You can set any or all of the writable [FolderPermission properties](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) when you create a **FolderPermission** object with a custom permission level.</span></span> <span data-ttu-id="348a3-266">No entanto, observe que o [FolderPermissionLevel](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) nunca explicitamente estiver definido como **personalizada** pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="348a3-266">Note, however, that the [FolderPermissionLevel](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) is never explicitly set to **Custom** by the application.</span></span> <span data-ttu-id="348a3-267">O **FolderPermissionLevel** é definido como o sinalizador somente quando você cria um objeto **FolderPermission** e definir permissões individuais.</span><span class="sxs-lookup"><span data-stu-id="348a3-267">The **FolderPermissionLevel** is set to Custom only when you create a **FolderPermission** object and set individual permissions.</span></span> 
  
## <a name="adding-folder-permissions-by-using-ews"></a><span data-ttu-id="348a3-268">Adicionando permissões da pasta usando o EWS</span><span class="sxs-lookup"><span data-stu-id="348a3-268">Adding folder permissions by using EWS</span></span>
<span data-ttu-id="348a3-269"><a name="bk_enableews"> </a></span><span class="sxs-lookup"><span data-stu-id="348a3-269"></span></span>

<span data-ttu-id="348a3-270">Os seguintes exemplos de código do EWS mostram como adicionar permissões a uma pasta específica por recuperar as permissões atuais e, em seguida, enviar uma lista das novas permissões.</span><span class="sxs-lookup"><span data-stu-id="348a3-270">The following EWS code examples show how to add permissions to a specific folder by retrieving the current permissions and then submitting a list of new permissions.</span></span>
  
<span data-ttu-id="348a3-271">A primeira etapa é enviar uma solicitação de [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , onde o valor de [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) Especifica a pasta na qual deseja adicionar permissões (a pasta Itens enviados neste exemplo) e o valor de [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) inclui a pasta: PermissionSet.</span><span class="sxs-lookup"><span data-stu-id="348a3-271">The first step is to send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request, where the [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) value specifies the folder in which to add permissions (the Sent Items folder in this example) and the [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) value includes folder:PermissionSet.</span></span> <span data-ttu-id="348a3-272">Essa solicitação irá recuperar as configurações de permissão para a pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="348a3-272">This request will retrieve the permission settings for the folder specified.</span></span> 
  
<span data-ttu-id="348a3-273">Isso também é a solicitação XML que o EWS Managed API envia quando você chama o método **ligar** para [Adicionar permissões da pasta](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="348a3-273">This is also the XML request that the EWS Managed API sends when you call the **Bind** method to [add folder permissions](#bk_enableewsma).</span></span>
  
```XML
  <?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:GetFolder>
        <m:FolderShape>
          <t:BaseShape>IdOnly</t:BaseShape>
          <t:AdditionalProperties>
            <t:FieldURI FieldURI="folder:PermissionSet" />
          </t:AdditionalProperties>
        </m:FolderShape>
        <m:FolderIds>
          <t:DistinguishedFolderId Id="sentitems" />
        </m:FolderIds>
      </m:GetFolder>
    </soap:Body>
  </soap:Envelope>
```

<span data-ttu-id="348a3-274">O servidor responde à solicitação **GetFolder** com uma mensagem de [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a pasta foi recuperada com êxito.</span><span class="sxs-lookup"><span data-stu-id="348a3-274">The server responds to the **GetFolder** request with a [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was retrieved successfully.</span></span> <span data-ttu-id="348a3-275">Os valores [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) e [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="348a3-275">The [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) and [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) values have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="CgAAAA=="
                          ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd1" />
              <t:PermissionSet>
                <t:Permissions>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Default</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                </t:Permissions>
              </t:PermissionSet>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="348a3-276">Em seguida, use a operação de **UpdateFolder** para enviar o atualizados [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx), que inclui a [permissão](http://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) para o novo usuário.</span><span class="sxs-lookup"><span data-stu-id="348a3-276">Next, use the **UpdateFolder** operation to send the updated [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx), which includes the [Permission](http://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) for the new user.</span></span> <span data-ttu-id="348a3-277">Observe que incluindo o elemento [SetFolderField](http://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) para a pasta respectivo na operação [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) substituirá todas as definições de permissão na pasta.</span><span class="sxs-lookup"><span data-stu-id="348a3-277">Note that including the [SetFolderField](http://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) element for the respective folder in the [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation will overwrite all the permission settings on the folder.</span></span> <span data-ttu-id="348a3-278">Da mesma forma, incluindo a opção [DeleteFolderField](http://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) da operação **UpdateFolder** excluirá também todas as definições de permissão na pasta.</span><span class="sxs-lookup"><span data-stu-id="348a3-278">Likewise, including the [DeleteFolderField](http://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) option of the **UpdateFolder** operation will also delete all the permission settings on the folder.</span></span> 
  
<span data-ttu-id="348a3-279">Isso também é a solicitação XML que o EWS Managed API envia ao chamar o método **Update** para [Adicionar permissões da pasta](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="348a3-279">This is also the XML request that the EWS Managed API sends when you call the **Update** method to [add folder permissions](#bk_enableewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="CgAAAA=="
                      ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd1" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:PermissionSet" />
              <t:Folder>
                <t:PermissionSet>
                  <t:Permissions>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Default</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
                      </t:UserId>
                      <t:PermissionLevel>Editor</t:PermissionLevel>
                    </t:Permission>
                  </t:Permissions>
                </t:PermissionSet>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="348a3-280">A linha de código a seguir especifica o nível de permissão.</span><span class="sxs-lookup"><span data-stu-id="348a3-280">The following line of code specifies the permission level.</span></span>
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
    </t:UserId>
    <t:PermissionLevel>Editor</t:PermissionLevel>
</t:Permission>
```

<span data-ttu-id="348a3-281">Se você quiser usar o nível de permissão personalizado, use este código.</span><span class="sxs-lookup"><span data-stu-id="348a3-281">If you want to use the custom permission level, use this code instead.</span></span>
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress> sadie@contoso.com </t:PrimarySmtpAddress>
    </t:UserId>
    <t:CanCreateItems>true</t:CanCreateItems>
    <t:CanCreateSubFolders>true</t:CanCreateSubFolders>
    <t:IsFolderOwner>false</t:IsFolderOwner>
    <t:IsFolderVisible>false</t:IsFolderVisible>
    <t:IsFolderContact>false</t:IsFolderContact>
    <t:EditItems>None</t:EditItems>
    <t:DeleteItems>None</t:DeleteItems>
    <t:ReadItems>None</t:ReadItems>
    <t:PermissionLevel>Custom</t:PermissionLevel>
</t:Permission>
```

<span data-ttu-id="348a3-282">O servidor responde à solicitação **UpdateFolder** com uma mensagem de [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a pasta foi atualizada com êxito.</span><span class="sxs-lookup"><span data-stu-id="348a3-282">The server responds to the **UpdateFolder** request with an [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was updated successfully.</span></span>
  
## <a name="removing-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="348a3-283">Remover permissões de pasta usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="348a3-283">Removing folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="348a3-284"><a name="bk_removeewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="348a3-284"></span></span>

<span data-ttu-id="348a3-285">O exemplo de código a seguir mostra como usar a API gerenciada de EWS para remover todas as permissões de usuário em uma pasta específica, exceto para o padrão e permissões anônimas, por:</span><span class="sxs-lookup"><span data-stu-id="348a3-285">The following code example shows how to use the EWS Managed API to remove all user permissions on a specific folder, except for the default and anonymous permissions, by:</span></span>
  
1. <span data-ttu-id="348a3-286">Obtendo as permissões atuais de uma pasta usando o método **vincular** .</span><span class="sxs-lookup"><span data-stu-id="348a3-286">Getting the current permissions for a folder by using the **Bind** method.</span></span> 
    
2. <span data-ttu-id="348a3-287">Iterar através da coleção de **permissões** e remover permissões para usuários individuais.</span><span class="sxs-lookup"><span data-stu-id="348a3-287">Iterating through the **Permissions** collection and removing permissions for individual users.</span></span> 
    
3. <span data-ttu-id="348a3-288">Chamar o método **Update** para salvar as alterações.</span><span class="sxs-lookup"><span data-stu-id="348a3-288">Calling the **Update** method to save the changes.</span></span> 
    
<span data-ttu-id="348a3-289">Este exemplo remove todas as permissões de usuário em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="348a3-289">This example removes all user permissions on a folder.</span></span> <span data-ttu-id="348a3-290">Se desejar modificar este exemplo para remover permissões somente para um usuário específico, altere a seguinte linha de código para identificar o nome de exibição ou o endereço SMTP do usuário.</span><span class="sxs-lookup"><span data-stu-id="348a3-290">If you want to modify this example to remove permissions only for a specific user, change the following line of code to identify either the display name or SMTP address of the user.</span></span>
  
```cs
if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
```

<span data-ttu-id="348a3-291">Este exemplo supõe que esse **serviço** é um objeto [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o proprietário da caixa de correio e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="348a3-291">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void RemoveFolderPermissions(ExchangeService service)
{
    // Create a property set to use for folder binding.
    PropertySet propSet = new PropertySet(BasePropertySet.FirstClassProperties, FolderSchema.Permissions);
    // Bind to the folder and get the current permissions. 
    // This call results in a GetFolder call to EWS.
    Folder sentItemsFolder = Folder.Bind(service, new FolderId(WellKnownFolderName.SentItems, "primary@contoso.com"), propSet);
    // Iterate through the collection of permissions and remove permissions for any 
    // user with a display name or SMTP address. This leaves the anonymous and 
    // default user permissions unchanged. 
    if (sentItemsFolder.Permissions.Count != 0)
    {
        for (int t = 0; t < sentItemsFolder.Permissions.Count; t++)
        {
            // Find any permissions associated with the specified user and remove them from the DACL
            if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
            {
                sentItemsFolder.Permissions.Remove(sentItemsFolder.Permissions[t]);
            }
        }
    }
    // This call results in an UpdateFolder call to EWS.
    sentItemsFolder.Update();
}
```

## <a name="removing-folder-permissions-by-using-ews"></a><span data-ttu-id="348a3-292">Removendo permissões da pasta usando o EWS</span><span class="sxs-lookup"><span data-stu-id="348a3-292">Removing folder permissions by using EWS</span></span>
<span data-ttu-id="348a3-293"><a name="bk_removeews"> </a></span><span class="sxs-lookup"><span data-stu-id="348a3-293"></span></span>

<span data-ttu-id="348a3-294">Os seguintes exemplos de código do EWS mostram como remover todas as permissões de usuário em uma pasta específica, exceto para o padrão e permissões anônimas.</span><span class="sxs-lookup"><span data-stu-id="348a3-294">The following EWS code examples show how to remove all user permissions on a specific folder, except for the default and anonymous permissions.</span></span>
  
<span data-ttu-id="348a3-295">Primeiro, envie uma solicitação de [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) onde o valor de [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) Especifica a pasta na qual deseja remover permissões (a pasta Itens enviados neste exemplo) e o valor de [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) inclui a pasta: PermissionSet.</span><span class="sxs-lookup"><span data-stu-id="348a3-295">First, send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request where the [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) value specifies the folder in which to remove permissions (the Sent Items folder in this example) and the [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) value includes folder:PermissionSet.</span></span> <span data-ttu-id="348a3-296">Essa solicitação irá recuperar o [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) para a pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="348a3-296">This request will retrieve the [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) for the folder specified.</span></span> 
  
<span data-ttu-id="348a3-297">Isso também é a solicitação XML que o EWS Managed API envia quando você chama o método **ligar** para [Remover permissões de pasta](#bk_removeewsma).</span><span class="sxs-lookup"><span data-stu-id="348a3-297">This is also the XML request that the EWS Managed API sends when you call the **Bind** method to [remove folder permissions](#bk_removeewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:PermissionSet" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="drafts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="348a3-298">O servidor responde à solicitação **GetFolder** com uma mensagem de [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a pasta foi recuperada com êxito.</span><span class="sxs-lookup"><span data-stu-id="348a3-298">The server responds to the **GetFolder** request with a [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was retrieved successfully.</span></span> <span data-ttu-id="348a3-299">Os valores dos elementos **FolderId** e **ParentFolderId** foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="348a3-299">The values of the **FolderId** and **ParentFolderId** elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="EAAAAA=="
                          ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd5" />
              <t:ParentFolderId Id="CQAAAA=="
                                ChangeKey="AQAAAA==" />
              <t:FolderClass>IPF.Note</t:FolderClass>
              <t:DisplayName>Drafts</t:DisplayName>
              <t:TotalCount>0</t:TotalCount>
              <t:ChildFolderCount>0</t:ChildFolderCount>
              <t:EffectiveRights>
                <t:CreateAssociated>true</t:CreateAssociated>
                <t:CreateContents>true</t:CreateContents>
                <t:CreateHierarchy>true</t:CreateHierarchy>
                <t:Delete>true</t:Delete>
                <t:Modify>true</t:Modify>
                <t:Read>true</t:Read>
                <t:ViewPrivateItems>true</t:ViewPrivateItems>
              </t:EffectiveRights>
              <t:PermissionSet>
                <t:Permissions>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Default</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:SID>S-1-5-21-1337771579-694202782-848329751-1535223</t:SID>
                      <t:PrimarySmtpAddress>sadie@Contoso.com</t:PrimarySmtpAddress>
                      <t:DisplayName>Sadie Daniels</t:DisplayName>
                    </t:UserId>
                    <t:CanCreateItems>true</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>true</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>All</t:EditItems>
                    <t:DeleteItems>All</t:DeleteItems>
                    <t:ReadItems>FullDetails</t:ReadItems>
                    <t:PermissionLevel>Editor</t:PermissionLevel>
                  </t:Permission>
                </t:Permissions>
              </t:PermissionSet>
              <t:UnreadCount>0</t:UnreadCount>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="348a3-300">Em seguida, use a operação de **UpdateFolder** para enviar o atualizados **PermissionSet**, que não inclui a **permissão** para o usuário removido.</span><span class="sxs-lookup"><span data-stu-id="348a3-300">Next, use the **UpdateFolder** operation to send the updated **PermissionSet**, which does not include the **Permission** for the removed user.</span></span> 
  
<span data-ttu-id="348a3-301">Isso também é a solicitação XML que o EWS Managed API envia ao chamar o método **Update** para [Remover permissões de pasta](#bk_removeewsma).</span><span class="sxs-lookup"><span data-stu-id="348a3-301">This is also the XML request that the EWS Managed API sends when you call the **Update** method to [remove folder permissions](#bk_removeewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="EAAAAA=="
                      ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd5" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:PermissionSet" />
              <t:Folder>
                <t:PermissionSet>
                  <t:Permissions>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Default</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                  </t:Permissions>
                </t:PermissionSet>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="348a3-302">O servidor responde à solicitação **UpdateFolder** com uma mensagem de **UpdateFolderResponse** que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica se a atualização foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="348a3-302">The server responds to the **UpdateFolder** request with an **UpdateFolderResponse** message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the update was successful.</span></span>
  
## <a name="updating-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="348a3-303">Atualizando permissões de pasta usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="348a3-303">Updating folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="348a3-304"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="348a3-304"></span></span>

<span data-ttu-id="348a3-305">Você também pode atualizar as permissões da pasta para uma pasta específica usando a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="348a3-305">You can also update folder permissions for a specific folder by using the EWS Managed API.</span></span> <span data-ttu-id="348a3-306">Para atualizar as permissões:</span><span class="sxs-lookup"><span data-stu-id="348a3-306">To update the permissions:</span></span> 
  
1. <span data-ttu-id="348a3-307">[Remover as permissões de pasta](#bk_removeewsma) para as permissões desatualizadas, mas não chamar o método **Update** (ainda).</span><span class="sxs-lookup"><span data-stu-id="348a3-307">[Remove the folder permissions](#bk_removeewsma) for the outdated permissions, but do not call the **Update** method (yet).</span></span> 
    
2. <span data-ttu-id="348a3-308">[Adicionar permissões de pasta para os usuários novos ou alterados](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="348a3-308">[Add folder permissions for the new or changed users](#bk_enableewsma).</span></span>
    
3. <span data-ttu-id="348a3-309">Chame o método **Update** para salvar as alterações.</span><span class="sxs-lookup"><span data-stu-id="348a3-309">Call the **Update** method to save the changes.</span></span> 
    
<span data-ttu-id="348a3-310">Se você tentar adicionar dois conjuntos de permissões para o mesmo usuário, você receberá um erro de **ServiceResponseException** com a seguinte descrição: "o conjunto de permissões especificado contém UserIds duplicados".</span><span class="sxs-lookup"><span data-stu-id="348a3-310">If you try to add two sets of permissions for the same user, you will receive a **ServiceResponseException** error with the following description: "The specified permission set contains duplicate UserIds".</span></span> <span data-ttu-id="348a3-311">Nesse caso, remova as permissões atuais da coleção **Permission** e adicione novas permissões ao conjunto de **permissão** .</span><span class="sxs-lookup"><span data-stu-id="348a3-311">In that case, remove the current permissions from the **Permission** collection, then add the new permissions to the **Permission** collection.</span></span> 
  
## <a name="updating-folder-permissions-by-using-ews"></a><span data-ttu-id="348a3-312">Atualizando permissões de pasta usando o EWS</span><span class="sxs-lookup"><span data-stu-id="348a3-312">Updating folder permissions by using EWS</span></span>
<span data-ttu-id="348a3-313"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="348a3-313"></span></span>

<span data-ttu-id="348a3-314">Você também pode atualizar as permissões da pasta para pastas específicas usando o EWS combinando o processo de adição e a remoção.</span><span class="sxs-lookup"><span data-stu-id="348a3-314">You can also update folder permissions for specific folders by using EWS by combining the removal and addition process.</span></span> <span data-ttu-id="348a3-315">Para atualizar as permissões:</span><span class="sxs-lookup"><span data-stu-id="348a3-315">To update the permissions:</span></span> 
  
1. <span data-ttu-id="348a3-316">Recupere as permissões da pasta atual usando a operação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="348a3-316">Retrieve the folder's current permissions by using the **GetFolder** operation.</span></span> 
    
2. <span data-ttu-id="348a3-317">Envie uma lista atualizada de permissões usando a operação **UpdateFolder** .</span><span class="sxs-lookup"><span data-stu-id="348a3-317">Send an updated list of permissions by using the **UpdateFolder** operation.</span></span> 
    
<span data-ttu-id="348a3-318">Essas são as mesmas operações de dois, que você pode usar para [Habilitar](#bk_enableews) ou [Remover o acesso](#bk_removeews) usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="348a3-318">These are the same two operations you use to [enable](#bk_enableews) or [remove access](#bk_removeews) by using EWS.</span></span> <span data-ttu-id="348a3-319">A única diferença é que quando você recebe a resposta **GetFolder** , ele conterá uma **permissão** definido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="348a3-319">The only difference is that when you receive the **GetFolder** response, it will contain a **Permission** set for user.</span></span> <span data-ttu-id="348a3-320">Simplesmente substituir esse elemento de **permissão** existente com o novo elemento de **permissão** e envie a operação **UpdateFolder** com o novo valor de **permissão** ou valores.</span><span class="sxs-lookup"><span data-stu-id="348a3-320">Simply replace that existing **Permission** element with the new **Permission** element, and then send the **UpdateFolder** operation with the new **Permission** value or values.</span></span> 
  
<span data-ttu-id="348a3-321">Se você tentar adicionar dois conjuntos de permissões para o mesmo usuário, você receberá um valor de **ResponseCode** de **ErrorDuplicateUserIdsSpecified**.</span><span class="sxs-lookup"><span data-stu-id="348a3-321">If you try to add two sets of permissions for the same user, you will receive a **ResponseCode** value of **ErrorDuplicateUserIdsSpecified**.</span></span> <span data-ttu-id="348a3-322">Nesse caso, remova o valor de permissão desatualizado para o usuário da solicitação e tente novamente a solicitação.</span><span class="sxs-lookup"><span data-stu-id="348a3-322">In that case, remove the outdated Permission value for the user from the request and then retry the request.</span></span>

## <a name="next-steps"></a><span data-ttu-id="348a3-323">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="348a3-323">Next steps</span></span>

<span data-ttu-id="348a3-324">Depois de conceder uma permissão de usuário para uma pasta específica, o usuário pode acessar a pasta como um representante.</span><span class="sxs-lookup"><span data-stu-id="348a3-324">After you give a user permission to a specific folder, the user can access the folder as a delegate.</span></span> <span data-ttu-id="348a3-325">For more information, see:</span><span class="sxs-lookup"><span data-stu-id="348a3-325">For more information, see:</span></span>
  
- [<span data-ttu-id="348a3-326">Email de acesso como um representante, usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="348a3-326">Access email as a delegate by using EWS in Exchange</span></span>](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="348a3-327">Acessar um calendário como um representante, usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="348a3-327">Access a calendar as a delegate by using EWS in Exchange</span></span>](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="348a3-328">Contatos de acesso como um representante, usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="348a3-328">Access contacts as a delegate by using EWS in Exchange</span></span>](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="348a3-329">Confira também</span><span class="sxs-lookup"><span data-stu-id="348a3-329">See also</span></span>

- [<span data-ttu-id="348a3-330">Acesso de representante e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="348a3-330">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)   
- [<span data-ttu-id="348a3-331">Adicionar e remover representantes usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="348a3-331">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="348a3-332">Pastas e itens no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="348a3-332">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    

