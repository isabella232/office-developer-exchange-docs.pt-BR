---
title: Definir permissões de pasta para outro usuário usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7eb81676-a780-4c56-b4f2-c4ed2697107d
description: Saiba como definir níveis de permissão em uma pasta usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: e25f1a49a430e8c95829d404fa53451b76cab167
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455867"
---
# <a name="set-folder-permissions-for-another-user-by-using-ews-in-exchange"></a><span data-ttu-id="b2871-103">Definir permissões de pasta para outro usuário usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b2871-103">Set folder permissions for another user by using EWS in Exchange</span></span>

<span data-ttu-id="b2871-104">Saiba como definir níveis de permissão em uma pasta usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2871-104">Learn how to set permission levels on a folder by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="b2871-105">As permissões no nível de pasta permitem que os usuários acessem uma ou mais pastas na caixa de correio de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="b2871-105">Folder-level permissions enable users to access one or more folders in another user's mailbox.</span></span> <span data-ttu-id="b2871-106">As permissões de pasta são semelhantes ao acesso de delegação, mas diferem das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="b2871-106">Folder permissions are similar to delegate access, but they differ in the following ways:</span></span> 
  
- <span data-ttu-id="b2871-107">As permissões de pasta não permitem que o usuário "enviar em nome de" ou "enviar como" outro usuário.</span><span class="sxs-lookup"><span data-stu-id="b2871-107">Folder permissions do not enable a user to "send on behalf of" or "send as" another user.</span></span> <span data-ttu-id="b2871-108">Eles só habilitam o acesso a pastas.</span><span class="sxs-lookup"><span data-stu-id="b2871-108">They only enable access to folders.</span></span> <span data-ttu-id="b2871-109">Os usuários podem criar itens nessas pastas, mas não podem enviá-los.</span><span class="sxs-lookup"><span data-stu-id="b2871-109">Users can create items in those folders, but they can't send them.</span></span>
    
- <span data-ttu-id="b2871-110">Você pode definir permissões de pasta em qualquer pasta da caixa de correio, mas só pode adicionar um representante às pastas calendário, contatos, caixa de entrada, diário, anotações e tarefas.</span><span class="sxs-lookup"><span data-stu-id="b2871-110">You can set folder permissions on any folder in the mailbox, but you can only add a delegate to the Calendar, Contacts, Inbox, Journal, Notes, and Tasks folders.</span></span>
    
- <span data-ttu-id="b2871-111">Você pode definir várias [permissões em uma pasta específica](#bk_folderperms).</span><span class="sxs-lookup"><span data-stu-id="b2871-111">You can set a number of [permissions on a specific folder](#bk_folderperms).</span></span> <span data-ttu-id="b2871-112">Ao adicionar um representante, você pode atribuir um apenas [cinco níveis de permissão](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span><span class="sxs-lookup"><span data-stu-id="b2871-112">When you add a delegate, you can assign one of only [five permission levels](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span></span>
    
- <span data-ttu-id="b2871-113">Você pode definir permissões de pasta para usuários anônimos e padrão.</span><span class="sxs-lookup"><span data-stu-id="b2871-113">You can set folder permissions for anonymous and default users.</span></span> <span data-ttu-id="b2871-114">Você só pode conceder acesso de representante a uma conta habilitada para email.</span><span class="sxs-lookup"><span data-stu-id="b2871-114">You can only grant delegate access to a mail-enabled account.</span></span>
    
<span data-ttu-id="b2871-115">Se você estiver familiarizado com as entradas de controle de acesso (ACEs) e listas de controle de acesso discricional (DACLs), saberá que um usuário só pode ter um conjunto de permissões para cada pasta.</span><span class="sxs-lookup"><span data-stu-id="b2871-115">If you're familiar with Access Control Entries (ACEs) and Discretionary Access Control Lists (DACLs), you know that a user can only have one set of permissions for each folder.</span></span> <span data-ttu-id="b2871-116">Se você tentar adicionar um conjunto de permissões para um usuário e ele já tiver um conjunto de permissões, você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="b2871-116">If you try to add a set of permissions for a user and they already have a set of permissions, you'll get an error.</span></span> <span data-ttu-id="b2871-117">Ao adicionar, remover ou atualizar permissões em uma pasta, você obtém a DACL atual, adiciona ou remove quaisquer ACEs e, em seguida, envia a DACL atualizada.</span><span class="sxs-lookup"><span data-stu-id="b2871-117">When you add, remove, or update permissions on a folder, you get the current DACL, add or remove any ACEs, and then send the updated DACL.</span></span> <span data-ttu-id="b2871-118">Você não pode adicionar várias ACEs para o mesmo usuário.</span><span class="sxs-lookup"><span data-stu-id="b2871-118">You cannot add multiple ACEs for the same user.</span></span> <span data-ttu-id="b2871-119">Ao atualizar permissões usando a API gerenciada do EWS, você precisa remover a ACE atual do usuário e, em seguida, adicionar sua nova ACE à coleção.</span><span class="sxs-lookup"><span data-stu-id="b2871-119">When you update permissions by using the EWS Managed API, you need to remove the user's current ACE and then add their new ACE to the collection.</span></span> <span data-ttu-id="b2871-120">Se você estiver usando o EWS, basta substituir o conjunto anterior de ACEs com as novas.</span><span class="sxs-lookup"><span data-stu-id="b2871-120">If you're using EWS, you just replace the previous set of ACEs with the new ones.</span></span>
  
<span data-ttu-id="b2871-121">Se você estiver fazendo várias alterações de permissão em uma única pasta, poderá realizar adições, remoções ou atualizações em lote, apenas Observe que não é possível colocar em lote as atualizações do usuário em várias pastas.</span><span class="sxs-lookup"><span data-stu-id="b2871-121">If you're making multiple permission changes to a single folder, you can batch additions, removals, or updates —just note that you cannot batch user updates on multiple folders.</span></span> <span data-ttu-id="b2871-122">Uma chamada é necessária para obter as permissões em uma única pasta e uma segunda chamada é necessária para atualizar as permissões nessa pasta.</span><span class="sxs-lookup"><span data-stu-id="b2871-122">One call is required to get the permissions on a single folder, and a second call is required to update the permissions on that folder.</span></span> <span data-ttu-id="b2871-123">Ao adicionar, remover ou atualizar permissões de usuário, você usa as mesmas duas chamadas de método ou operações para cada tarefa.</span><span class="sxs-lookup"><span data-stu-id="b2871-123">When you add, remove, or update user permissions, you use the same two method calls or operations for each task.</span></span>
  
<span data-ttu-id="b2871-124">**Tabela 1. Métodos da API gerenciada do EWS e operações do EWS para definir permissões de pasta**</span><span class="sxs-lookup"><span data-stu-id="b2871-124">**Table 1. EWS Managed API methods and EWS operations for setting folder permissions**</span></span>

|<span data-ttu-id="b2871-125">Se você quiser...</span><span class="sxs-lookup"><span data-stu-id="b2871-125">If you want to…</span></span>|<span data-ttu-id="b2871-126">Use este método de API gerenciada do EWS...</span><span class="sxs-lookup"><span data-stu-id="b2871-126">Use this EWS Managed API method…</span></span>|<span data-ttu-id="b2871-127">Use esta operação do EWS...</span><span class="sxs-lookup"><span data-stu-id="b2871-127">Use this EWS operation…</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b2871-128">Habilitar, remover ou atualizar permissões de pasta</span><span class="sxs-lookup"><span data-stu-id="b2871-128">Enable, remove, or update folder permissions</span></span>  <br/> |<span data-ttu-id="b2871-129">[Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) seguido por [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b2871-129">[Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) followed by [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="b2871-130">[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) seguido por [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b2871-130">[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) followed by [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="b2871-131">Criar uma pasta e definir permissões de pasta</span><span class="sxs-lookup"><span data-stu-id="b2871-131">Create a folder and define folder permissions</span></span>  <br/> |[<span data-ttu-id="b2871-132">Folder. Save</span><span class="sxs-lookup"><span data-stu-id="b2871-132">Folder.Save</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="b2871-133">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="b2871-133">CreateFolder</span></span>](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
   
## <a name="folder-permissions"></a><span data-ttu-id="b2871-134">Permissões de pastas</span><span class="sxs-lookup"><span data-stu-id="b2871-134">Folder permissions</span></span>
<span data-ttu-id="b2871-135"><a name="bk_folderperms"> </a></span><span class="sxs-lookup"><span data-stu-id="b2871-135"><a name="bk_folderperms"> </a></span></span>

<span data-ttu-id="b2871-136">Há algumas opções em relação à definição de permissões de pasta em uma pasta específica.</span><span class="sxs-lookup"><span data-stu-id="b2871-136">You have quite a few options when it comes to setting folder permissions on a specific folder.</span></span> <span data-ttu-id="b2871-137">Você pode definir um nível de permissão em uma pasta para cada usuário, que adiciona um conjunto de permissões individuais predefinidas à DACL ou pode definir permissões individuais em uma pasta, mas não é possível misturar e corresponder.</span><span class="sxs-lookup"><span data-stu-id="b2871-137">You can set a permission level on a folder for each user, which adds a set of predefined individual permissions to the DACL, or you can set individual permissions on a folder — but you can't mix and match.</span></span>
  
<span data-ttu-id="b2871-138">As seguintes permissões individuais estão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="b2871-138">The following individual permissions are available:</span></span>
  
- <span data-ttu-id="b2871-139">Pode criar</span><span class="sxs-lookup"><span data-stu-id="b2871-139">Can create</span></span>
- <span data-ttu-id="b2871-140">Pode criar subpastas</span><span class="sxs-lookup"><span data-stu-id="b2871-140">Can create subfolders</span></span>    
- <span data-ttu-id="b2871-141">É proprietário da pasta</span><span class="sxs-lookup"><span data-stu-id="b2871-141">Is folder owner</span></span>    
- <span data-ttu-id="b2871-142">A pasta é visível</span><span class="sxs-lookup"><span data-stu-id="b2871-142">Is folder visible</span></span>    
- <span data-ttu-id="b2871-143">É o contato da pasta</span><span class="sxs-lookup"><span data-stu-id="b2871-143">Is folder contact</span></span>    
- <span data-ttu-id="b2871-144">Editar itens</span><span class="sxs-lookup"><span data-stu-id="b2871-144">Edit items</span></span>    
- <span data-ttu-id="b2871-145">Excluir itens</span><span class="sxs-lookup"><span data-stu-id="b2871-145">Delete items</span></span>    
- <span data-ttu-id="b2871-146">Ler itens</span><span class="sxs-lookup"><span data-stu-id="b2871-146">Read items</span></span>
    
<span data-ttu-id="b2871-147">Além disso, os seguintes níveis de permissão estão disponíveis, que definem um subconjunto de permissões e valores individuais, conforme mostrado na tabela 2:</span><span class="sxs-lookup"><span data-stu-id="b2871-147">In addition, the following permission levels are available, which define a subset of individual permissions and values, as shown in Table 2:</span></span>
  
- <span data-ttu-id="b2871-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2871-148">None</span></span>    
- <span data-ttu-id="b2871-149">Proprietário</span><span class="sxs-lookup"><span data-stu-id="b2871-149">Owner</span></span>    
- <span data-ttu-id="b2871-150">Publishingeditorcreateitems</span><span class="sxs-lookup"><span data-stu-id="b2871-150">PublishingEditor</span></span>    
- <span data-ttu-id="b2871-151">Editor</span><span class="sxs-lookup"><span data-stu-id="b2871-151">Editor</span></span>    
- <span data-ttu-id="b2871-152">Publishingauthorcreateitems</span><span class="sxs-lookup"><span data-stu-id="b2871-152">PublishingAuthor</span></span>    
- <span data-ttu-id="b2871-153">Autor</span><span class="sxs-lookup"><span data-stu-id="b2871-153">Author</span></span>    
- <span data-ttu-id="b2871-154">Noneditingauthorcreateitems</span><span class="sxs-lookup"><span data-stu-id="b2871-154">NoneditingAuthor</span></span>    
- <span data-ttu-id="b2871-155">Revisor</span><span class="sxs-lookup"><span data-stu-id="b2871-155">Reviewer</span></span>    
- <span data-ttu-id="b2871-156">Colaborador</span><span class="sxs-lookup"><span data-stu-id="b2871-156">Contributor</span></span>   
- <span data-ttu-id="b2871-157">Custom-este valor não pode ser definido pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b2871-157">Custom - This value cannot be set by the application.</span></span> <span data-ttu-id="b2871-158">O servidor define esse valor se o aplicativo incluir uma coleção personalizada de permissões individuais.</span><span class="sxs-lookup"><span data-stu-id="b2871-158">The server sets this value if the application includes a custom collection of individual permissions.</span></span>    
- <span data-ttu-id="b2871-159">FreeBusyTimeOnly-isso só pode ser definido em pastas de calendário.</span><span class="sxs-lookup"><span data-stu-id="b2871-159">FreeBusyTimeOnly - This can only be set on Calendar folders.</span></span>   
- <span data-ttu-id="b2871-160">FreeBusyTimeAndSubjectAndLocation-isso só pode ser definido em pastas de calendário.</span><span class="sxs-lookup"><span data-stu-id="b2871-160">FreeBusyTimeAndSubjectAndLocation - This can only be set on Calendar folders.</span></span>
    
<span data-ttu-id="b2871-161">A tabela a seguir mostra quais permissões individuais são aplicadas por padrão com base no nível de permissão.</span><span class="sxs-lookup"><span data-stu-id="b2871-161">The following table shows which individual permissions are applied by default based on permission level.</span></span>
  
<span data-ttu-id="b2871-162">**Tabela 2. Permissões individuais por nível de permissão**</span><span class="sxs-lookup"><span data-stu-id="b2871-162">**Table 2. Individual permissions by permission level**</span></span>

|<span data-ttu-id="b2871-163">Nível da permissão</span><span class="sxs-lookup"><span data-stu-id="b2871-163">Permission level</span></span>|<span data-ttu-id="b2871-164">Pode criar itens</span><span class="sxs-lookup"><span data-stu-id="b2871-164">Can create items</span></span>|<span data-ttu-id="b2871-165">Pode criar subpastas</span><span class="sxs-lookup"><span data-stu-id="b2871-165">Can create sub folders</span></span>|<span data-ttu-id="b2871-166">É proprietário da pasta</span><span class="sxs-lookup"><span data-stu-id="b2871-166">Is folder owner</span></span>|<span data-ttu-id="b2871-167">A pasta é visível</span><span class="sxs-lookup"><span data-stu-id="b2871-167">Is folder visible</span></span>|<span data-ttu-id="b2871-168">É o contato da pasta</span><span class="sxs-lookup"><span data-stu-id="b2871-168">Is folder contact</span></span>|<span data-ttu-id="b2871-169">Editar itens</span><span class="sxs-lookup"><span data-stu-id="b2871-169">Edit items</span></span>|<span data-ttu-id="b2871-170">Excluir itens</span><span class="sxs-lookup"><span data-stu-id="b2871-170">Delete items</span></span>|<span data-ttu-id="b2871-171">Pode ler itens</span><span class="sxs-lookup"><span data-stu-id="b2871-171">Can read items</span></span>|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|<span data-ttu-id="b2871-172">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2871-172">None</span></span>  <br/> |<span data-ttu-id="b2871-173">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-173">False</span></span>  <br/> |<span data-ttu-id="b2871-174">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-174">False</span></span>  <br/> |<span data-ttu-id="b2871-175">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-175">False</span></span>  <br/> |<span data-ttu-id="b2871-176">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-176">False</span></span>  <br/> |<span data-ttu-id="b2871-177">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-177">False</span></span>  <br/> |<span data-ttu-id="b2871-178">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2871-178">None</span></span>  <br/> |<span data-ttu-id="b2871-179">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2871-179">None</span></span>  <br/> |<span data-ttu-id="b2871-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2871-180">None</span></span>  <br/> |
|<span data-ttu-id="b2871-181">Proprietário</span><span class="sxs-lookup"><span data-stu-id="b2871-181">Owner</span></span>  <br/> |<span data-ttu-id="b2871-182">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-182">True</span></span>  <br/> |<span data-ttu-id="b2871-183">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-183">True</span></span>  <br/> |<span data-ttu-id="b2871-184">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-184">True</span></span>  <br/> |<span data-ttu-id="b2871-185">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-185">True</span></span>  <br/> |<span data-ttu-id="b2871-186">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-186">True</span></span>  <br/> |<span data-ttu-id="b2871-187">Todos</span><span class="sxs-lookup"><span data-stu-id="b2871-187">All</span></span>  <br/> |<span data-ttu-id="b2871-188">Todos</span><span class="sxs-lookup"><span data-stu-id="b2871-188">All</span></span>  <br/> |<span data-ttu-id="b2871-189">FullDetails</span><span class="sxs-lookup"><span data-stu-id="b2871-189">FullDetails</span></span>  <br/> |
|<span data-ttu-id="b2871-190">Publishingeditorcreateitems</span><span class="sxs-lookup"><span data-stu-id="b2871-190">PublishingEditor</span></span>  <br/> |<span data-ttu-id="b2871-191">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-191">True</span></span>  <br/> |<span data-ttu-id="b2871-192">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-192">True</span></span>  <br/> |<span data-ttu-id="b2871-193">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-193">False</span></span>  <br/> |<span data-ttu-id="b2871-194">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-194">True</span></span>  <br/> |<span data-ttu-id="b2871-195">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-195">False</span></span>  <br/> |<span data-ttu-id="b2871-196">Todos</span><span class="sxs-lookup"><span data-stu-id="b2871-196">All</span></span>  <br/> |<span data-ttu-id="b2871-197">Todos</span><span class="sxs-lookup"><span data-stu-id="b2871-197">All</span></span>  <br/> |<span data-ttu-id="b2871-198">FullDetails</span><span class="sxs-lookup"><span data-stu-id="b2871-198">FullDetails</span></span>  <br/> |
|<span data-ttu-id="b2871-199">Editor</span><span class="sxs-lookup"><span data-stu-id="b2871-199">Editor</span></span>  <br/> |<span data-ttu-id="b2871-200">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-200">True</span></span>  <br/> |<span data-ttu-id="b2871-201">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-201">False</span></span>  <br/> |<span data-ttu-id="b2871-202">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-202">False</span></span>  <br/> |<span data-ttu-id="b2871-203">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-203">True</span></span>  <br/> |<span data-ttu-id="b2871-204">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-204">False</span></span>  <br/> |<span data-ttu-id="b2871-205">Todos</span><span class="sxs-lookup"><span data-stu-id="b2871-205">All</span></span>  <br/> |<span data-ttu-id="b2871-206">Todos</span><span class="sxs-lookup"><span data-stu-id="b2871-206">All</span></span>  <br/> |<span data-ttu-id="b2871-207">FullDetails</span><span class="sxs-lookup"><span data-stu-id="b2871-207">FullDetails</span></span>  <br/> |
|<span data-ttu-id="b2871-208">Publishingauthorcreateitems</span><span class="sxs-lookup"><span data-stu-id="b2871-208">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="b2871-209">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-209">True</span></span>  <br/> |<span data-ttu-id="b2871-210">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-210">True</span></span>  <br/> |<span data-ttu-id="b2871-211">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-211">False</span></span>  <br/> |<span data-ttu-id="b2871-212">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-212">True</span></span>  <br/> |<span data-ttu-id="b2871-213">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-213">False</span></span>  <br/> |<span data-ttu-id="b2871-214">Possuir</span><span class="sxs-lookup"><span data-stu-id="b2871-214">Owned</span></span>  <br/> |<span data-ttu-id="b2871-215">Possuir</span><span class="sxs-lookup"><span data-stu-id="b2871-215">Owned</span></span>  <br/> |<span data-ttu-id="b2871-216">FullDetails</span><span class="sxs-lookup"><span data-stu-id="b2871-216">FullDetails</span></span>  <br/> |
|<span data-ttu-id="b2871-217">Autor</span><span class="sxs-lookup"><span data-stu-id="b2871-217">Author</span></span>  <br/> |<span data-ttu-id="b2871-218">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-218">True</span></span>  <br/> |<span data-ttu-id="b2871-219">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-219">False</span></span>  <br/> |<span data-ttu-id="b2871-220">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-220">False</span></span>  <br/> |<span data-ttu-id="b2871-221">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-221">True</span></span>  <br/> |<span data-ttu-id="b2871-222">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-222">False</span></span>  <br/> |<span data-ttu-id="b2871-223">Possuir</span><span class="sxs-lookup"><span data-stu-id="b2871-223">Owned</span></span>  <br/> |<span data-ttu-id="b2871-224">Possuir</span><span class="sxs-lookup"><span data-stu-id="b2871-224">Owned</span></span>  <br/> |<span data-ttu-id="b2871-225">FullDetails</span><span class="sxs-lookup"><span data-stu-id="b2871-225">FullDetails</span></span>  <br/> |
|<span data-ttu-id="b2871-226">Noneditingauthorcreateitems</span><span class="sxs-lookup"><span data-stu-id="b2871-226">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="b2871-227">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-227">True</span></span>  <br/> |<span data-ttu-id="b2871-228">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-228">False</span></span>  <br/> |<span data-ttu-id="b2871-229">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-229">False</span></span>  <br/> |<span data-ttu-id="b2871-230">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-230">True</span></span>  <br/> |<span data-ttu-id="b2871-231">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-231">False</span></span>  <br/> |<span data-ttu-id="b2871-232">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2871-232">None</span></span>  <br/> |<span data-ttu-id="b2871-233">Possuir</span><span class="sxs-lookup"><span data-stu-id="b2871-233">Owned</span></span>  <br/> |<span data-ttu-id="b2871-234">FullDetails</span><span class="sxs-lookup"><span data-stu-id="b2871-234">FullDetails</span></span>  <br/> |
|<span data-ttu-id="b2871-235">Revisor</span><span class="sxs-lookup"><span data-stu-id="b2871-235">Reviewer</span></span>  <br/> |<span data-ttu-id="b2871-236">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-236">False</span></span>  <br/> |<span data-ttu-id="b2871-237">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-237">False</span></span>  <br/> |<span data-ttu-id="b2871-238">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-238">False</span></span>  <br/> |<span data-ttu-id="b2871-239">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-239">True</span></span>  <br/> |<span data-ttu-id="b2871-240">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-240">False</span></span>  <br/> |<span data-ttu-id="b2871-241">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2871-241">None</span></span>  <br/> |<span data-ttu-id="b2871-242">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2871-242">None</span></span>  <br/> |<span data-ttu-id="b2871-243">FullDetails</span><span class="sxs-lookup"><span data-stu-id="b2871-243">FullDetails</span></span>  <br/> |
|<span data-ttu-id="b2871-244">Colaborador</span><span class="sxs-lookup"><span data-stu-id="b2871-244">Contributor</span></span>  <br/> |<span data-ttu-id="b2871-245">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-245">True</span></span>  <br/> |<span data-ttu-id="b2871-246">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-246">False</span></span>  <br/> |<span data-ttu-id="b2871-247">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-247">False</span></span>  <br/> |<span data-ttu-id="b2871-248">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b2871-248">True</span></span>  <br/> |<span data-ttu-id="b2871-249">Falso</span><span class="sxs-lookup"><span data-stu-id="b2871-249">False</span></span>  <br/> |<span data-ttu-id="b2871-250">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2871-250">None</span></span>  <br/> |<span data-ttu-id="b2871-251">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2871-251">None</span></span>  <br/> |<span data-ttu-id="b2871-252">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2871-252">None</span></span>  <br/> |
   
<span data-ttu-id="b2871-253">Se você especificar um nível de permissão não personalizado na solicitação de permissões de nível de pasta, não será necessário especificar as configurações de permissão individuais.</span><span class="sxs-lookup"><span data-stu-id="b2871-253">If you specify a non-custom permission level in the folder-level permissions request, you don't need to specify the individual permission settings.</span></span> <span data-ttu-id="b2871-254">Se você especificar uma permissão individual ao definir um nível de permissão, um erro **ErrorInvalidPermissionSettings** será retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="b2871-254">If you do specify an individual permission when you set a permission level, an **ErrorInvalidPermissionSettings** error will be returned in the response.</span></span> 
  
## <a name="adding-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="b2871-255">Adicionando permissões de pasta usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="b2871-255">Adding folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="b2871-256"><a name="bk_enableewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b2871-256"><a name="bk_enableewsma"> </a></span></span>

<span data-ttu-id="b2871-257">O exemplo de código a seguir mostra como usar a API gerenciada do EWS para:</span><span class="sxs-lookup"><span data-stu-id="b2871-257">The following code example shows how to use the EWS Managed API to:</span></span> 
  
- <span data-ttu-id="b2871-258">Criar um novo objeto [FolderPermission](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) para o novo usuário.</span><span class="sxs-lookup"><span data-stu-id="b2871-258">Create a new [FolderPermission](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) object for the new user.</span></span> 
    
- <span data-ttu-id="b2871-259">Obtenha as permissões atuais para uma pasta usando o método [BIND](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b2871-259">Get the current permissions for a folder by using the [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method.</span></span> 
    
- <span data-ttu-id="b2871-260">Adicione o novo **FolderPermissions** à propriedade [Folder. Permissions](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b2871-260">Add the new **FolderPermissions** to the [Folder.Permissions](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) property.</span></span> 
    
- <span data-ttu-id="b2871-261">Chame o método [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) para salvar as novas permissões no servidor.</span><span class="sxs-lookup"><span data-stu-id="b2871-261">Call the [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the new permissions to the server.</span></span> 
    
<span data-ttu-id="b2871-262">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o proprietário da caixa de correio e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2871-262">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="b2871-263">A linha de código a seguir especifica o nível de permissão.</span><span class="sxs-lookup"><span data-stu-id="b2871-263">The following line of code specifies the permission level.</span></span>
  
```cs
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
```

<span data-ttu-id="b2871-264">Se você quiser usar o nível de permissão personalizado, use este código em vez disso.</span><span class="sxs-lookup"><span data-stu-id="b2871-264">If you want to use the custom permission level, use this code instead.</span></span>
  
```cs
FolderPermission fldperm = new FolderPermission();
fldperm.UserId = "sadie@Contoso1000.onmicrosoft.com";
fldperm.CanCreateItems = true;
fldperm.CanCreateSubFolders = true;
…
```

<span data-ttu-id="b2871-265">Você pode definir qualquer uma ou todas as [Propriedades FolderPermission](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) graváveis ao criar um objeto **FolderPermission** com um nível de permissão personalizado.</span><span class="sxs-lookup"><span data-stu-id="b2871-265">You can set any or all of the writable [FolderPermission properties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) when you create a **FolderPermission** object with a custom permission level.</span></span> <span data-ttu-id="b2871-266">Observe, no entanto, que o [FolderPermissionLevel](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) nunca é explicitamente definido como **personalizado** pelo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b2871-266">Note, however, that the [FolderPermissionLevel](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) is never explicitly set to **Custom** by the application.</span></span> <span data-ttu-id="b2871-267">**FolderPermissionLevel** é definido como Custom somente quando você cria um objeto **FolderPermission** e define permissões individuais.</span><span class="sxs-lookup"><span data-stu-id="b2871-267">The **FolderPermissionLevel** is set to Custom only when you create a **FolderPermission** object and set individual permissions.</span></span> 
  
## <a name="adding-folder-permissions-by-using-ews"></a><span data-ttu-id="b2871-268">Adicionando permissões de pasta usando EWS</span><span class="sxs-lookup"><span data-stu-id="b2871-268">Adding folder permissions by using EWS</span></span>
<span data-ttu-id="b2871-269"><a name="bk_enableews"> </a></span><span class="sxs-lookup"><span data-stu-id="b2871-269"><a name="bk_enableews"> </a></span></span>

<span data-ttu-id="b2871-270">Os exemplos de código do EWS a seguir mostram como adicionar permissões a uma pasta específica, recuperando as permissões atuais e, em seguida, enviando uma lista de novas permissões.</span><span class="sxs-lookup"><span data-stu-id="b2871-270">The following EWS code examples show how to add permissions to a specific folder by retrieving the current permissions and then submitting a list of new permissions.</span></span>
  
<span data-ttu-id="b2871-271">A primeira etapa é enviar uma solicitação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , em que o valor [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) especifica a pasta na qual adicionar permissões (a pasta Itens enviados neste exemplo) e o valor de [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) inclui a pasta: PermissionSet.</span><span class="sxs-lookup"><span data-stu-id="b2871-271">The first step is to send a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request, where the [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) value specifies the folder in which to add permissions (the Sent Items folder in this example) and the [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) value includes folder:PermissionSet.</span></span> <span data-ttu-id="b2871-272">Essa solicitação irá recuperar as configurações de permissão para a pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="b2871-272">This request will retrieve the permission settings for the folder specified.</span></span> 
  
<span data-ttu-id="b2871-273">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você chama o método **BIND** para [adicionar permissões de pasta](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="b2871-273">This is also the XML request that the EWS Managed API sends when you call the **Bind** method to [add folder permissions](#bk_enableewsma).</span></span>
  
```XML
  <?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                 xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="b2871-274">O servidor responde à solicitação **GetFolder** com uma mensagem [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a pasta foi recuperada com êxito.</span><span class="sxs-lookup"><span data-stu-id="b2871-274">The server responds to the **GetFolder** request with a [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was retrieved successfully.</span></span> <span data-ttu-id="b2871-275">Os valores [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) e [ParentFolderId](https://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) foram reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="b2871-275">The [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) and [ParentFolderId](https://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) values have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="b2871-276">Em seguida, use a operação **UpdateFolder** para enviar o [PermissionSet](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx)atualizado, que inclui a [permissão](https://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) para o novo usuário.</span><span class="sxs-lookup"><span data-stu-id="b2871-276">Next, use the **UpdateFolder** operation to send the updated [PermissionSet](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx), which includes the [Permission](https://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) for the new user.</span></span> <span data-ttu-id="b2871-277">Observe que, incluindo o elemento [Setfolderfield](https://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) da respectiva pasta na operação [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) substituirá todas as configurações de permissão na pasta.</span><span class="sxs-lookup"><span data-stu-id="b2871-277">Note that including the [SetFolderField](https://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) element for the respective folder in the [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation will overwrite all the permission settings on the folder.</span></span> <span data-ttu-id="b2871-278">Da mesma forma, incluindo a opção [DeleteFolderField](https://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) da operação **UpdateFolder** também excluirá todas as configurações de permissão na pasta.</span><span class="sxs-lookup"><span data-stu-id="b2871-278">Likewise, including the [DeleteFolderField](https://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) option of the **UpdateFolder** operation will also delete all the permission settings on the folder.</span></span> 
  
<span data-ttu-id="b2871-279">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você chama o método **Update** para [adicionar permissões de pasta](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="b2871-279">This is also the XML request that the EWS Managed API sends when you call the **Update** method to [add folder permissions](#bk_enableewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="b2871-280">A linha de código a seguir especifica o nível de permissão.</span><span class="sxs-lookup"><span data-stu-id="b2871-280">The following line of code specifies the permission level.</span></span>
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
    </t:UserId>
    <t:PermissionLevel>Editor</t:PermissionLevel>
</t:Permission>
```

<span data-ttu-id="b2871-281">Se você quiser usar o nível de permissão personalizado, use este código em vez disso.</span><span class="sxs-lookup"><span data-stu-id="b2871-281">If you want to use the custom permission level, use this code instead.</span></span>
  
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

<span data-ttu-id="b2871-282">O servidor responde à solicitação **UpdateFolder** com uma mensagem [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a pasta foi atualizada com êxito.</span><span class="sxs-lookup"><span data-stu-id="b2871-282">The server responds to the **UpdateFolder** request with an [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was updated successfully.</span></span>
  
## <a name="removing-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="b2871-283">Removendo permissões de pasta usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="b2871-283">Removing folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="b2871-284"><a name="bk_removeewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b2871-284"><a name="bk_removeewsma"> </a></span></span>

<span data-ttu-id="b2871-285">O exemplo de código a seguir mostra como usar a API gerenciada do EWS para remover todas as permissões de usuário em uma pasta específica, exceto as permissões padrão e anônimas, por:</span><span class="sxs-lookup"><span data-stu-id="b2871-285">The following code example shows how to use the EWS Managed API to remove all user permissions on a specific folder, except for the default and anonymous permissions, by:</span></span>
  
1. <span data-ttu-id="b2871-286">Obtendo as permissões atuais para uma pasta usando o método **BIND** .</span><span class="sxs-lookup"><span data-stu-id="b2871-286">Getting the current permissions for a folder by using the **Bind** method.</span></span> 
    
2. <span data-ttu-id="b2871-287">Iterar pela coleção **Permissions** e remover permissões para usuários individuais.</span><span class="sxs-lookup"><span data-stu-id="b2871-287">Iterating through the **Permissions** collection and removing permissions for individual users.</span></span> 
    
3. <span data-ttu-id="b2871-288">Chamar o método **Update** para salvar as alterações.</span><span class="sxs-lookup"><span data-stu-id="b2871-288">Calling the **Update** method to save the changes.</span></span> 
    
<span data-ttu-id="b2871-289">Este exemplo remove todas as permissões de usuário em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="b2871-289">This example removes all user permissions on a folder.</span></span> <span data-ttu-id="b2871-290">Se você deseja modificar este exemplo para remover permissões somente para um usuário específico, altere a linha de código a seguir para identificar o nome de exibição ou o endereço SMTP do usuário.</span><span class="sxs-lookup"><span data-stu-id="b2871-290">If you want to modify this example to remove permissions only for a specific user, change the following line of code to identify either the display name or SMTP address of the user.</span></span>
  
```cs
if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
```

<span data-ttu-id="b2871-291">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o proprietário da caixa de correio e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2871-291">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="removing-folder-permissions-by-using-ews"></a><span data-ttu-id="b2871-292">Removendo permissões de pasta usando EWS</span><span class="sxs-lookup"><span data-stu-id="b2871-292">Removing folder permissions by using EWS</span></span>
<span data-ttu-id="b2871-293"><a name="bk_removeews"> </a></span><span class="sxs-lookup"><span data-stu-id="b2871-293"><a name="bk_removeews"> </a></span></span>

<span data-ttu-id="b2871-294">Os exemplos de código do EWS a seguir mostram como remover todas as permissões de usuário em uma pasta específica, exceto as permissões padrão e anônimas.</span><span class="sxs-lookup"><span data-stu-id="b2871-294">The following EWS code examples show how to remove all user permissions on a specific folder, except for the default and anonymous permissions.</span></span>
  
<span data-ttu-id="b2871-295">Primeiro, envie uma solicitação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) onde o valor [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) especifica a pasta na qual as permissões serão removidas (a pasta Itens enviados neste exemplo) e o valor [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) inclui Folder: PermissionSet.</span><span class="sxs-lookup"><span data-stu-id="b2871-295">First, send a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request where the [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) value specifies the folder in which to remove permissions (the Sent Items folder in this example) and the [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) value includes folder:PermissionSet.</span></span> <span data-ttu-id="b2871-296">Essa solicitação recuperará o [PermissionSet](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) para a pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="b2871-296">This request will retrieve the [PermissionSet](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) for the folder specified.</span></span> 
  
<span data-ttu-id="b2871-297">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você chama o método **BIND** para [remover permissões de pasta](#bk_removeewsma).</span><span class="sxs-lookup"><span data-stu-id="b2871-297">This is also the XML request that the EWS Managed API sends when you call the **Bind** method to [remove folder permissions](#bk_removeewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="b2871-298">O servidor responde à solicitação **GetFolder** com uma mensagem [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a pasta foi recuperada com êxito.</span><span class="sxs-lookup"><span data-stu-id="b2871-298">The server responds to the **GetFolder** request with a [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was retrieved successfully.</span></span> <span data-ttu-id="b2871-299">Os valores dos elementos **FolderId** e **ParentFolderId** foram reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="b2871-299">The values of the **FolderId** and **ParentFolderId** elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="b2871-300">Em seguida, use a operação **UpdateFolder** para enviar o **PermissionSet**atualizado, que não inclui a **permissão** para o usuário removido.</span><span class="sxs-lookup"><span data-stu-id="b2871-300">Next, use the **UpdateFolder** operation to send the updated **PermissionSet**, which does not include the **Permission** for the removed user.</span></span> 
  
<span data-ttu-id="b2871-301">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você chama o método **Update** para [remover as permissões de pasta](#bk_removeewsma).</span><span class="sxs-lookup"><span data-stu-id="b2871-301">This is also the XML request that the EWS Managed API sends when you call the **Update** method to [remove folder permissions](#bk_removeewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="b2871-302">O servidor responde à solicitação **UpdateFolder** com uma mensagem **UpdateFolderResponse** que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a atualização foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="b2871-302">The server responds to the **UpdateFolder** request with an **UpdateFolderResponse** message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the update was successful.</span></span>
  
## <a name="updating-folder-permissions-by-using-the-ews-managed-api"></a><span data-ttu-id="b2871-303">Atualizando permissões de pasta usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="b2871-303">Updating folder permissions by using the EWS Managed API</span></span>
<span data-ttu-id="b2871-304"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b2871-304"><a name="bk_updateewsma"> </a></span></span>

<span data-ttu-id="b2871-305">Você também pode atualizar as permissões de pasta de uma pasta específica usando a API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="b2871-305">You can also update folder permissions for a specific folder by using the EWS Managed API.</span></span> <span data-ttu-id="b2871-306">Para atualizar as permissões:</span><span class="sxs-lookup"><span data-stu-id="b2871-306">To update the permissions:</span></span> 
  
1. <span data-ttu-id="b2871-307">[Remova as permissões de pasta](#bk_removeewsma) para as permissões desatualizadas, mas não chame o método **Update** (ainda).</span><span class="sxs-lookup"><span data-stu-id="b2871-307">[Remove the folder permissions](#bk_removeewsma) for the outdated permissions, but do not call the **Update** method (yet).</span></span> 
    
2. <span data-ttu-id="b2871-308">[Adicione permissões de pasta para os usuários novos ou alterados](#bk_enableewsma).</span><span class="sxs-lookup"><span data-stu-id="b2871-308">[Add folder permissions for the new or changed users](#bk_enableewsma).</span></span>
    
3. <span data-ttu-id="b2871-309">Chame o método **Update** para salvar as alterações.</span><span class="sxs-lookup"><span data-stu-id="b2871-309">Call the **Update** method to save the changes.</span></span> 
    
<span data-ttu-id="b2871-310">Se você tentar adicionar dois conjuntos de permissões para o mesmo usuário, receberá **um erro de** ServiceDescription com a seguinte descrição: "o conjunto de permissões especificado contém userids duplicados".</span><span class="sxs-lookup"><span data-stu-id="b2871-310">If you try to add two sets of permissions for the same user, you will receive a **ServiceResponseException** error with the following description: "The specified permission set contains duplicate UserIds".</span></span> <span data-ttu-id="b2871-311">Nesse caso, remova as permissões atuais da coleção **Permission** e, em seguida, adicione as novas permissões à coleção **Permission** .</span><span class="sxs-lookup"><span data-stu-id="b2871-311">In that case, remove the current permissions from the **Permission** collection, then add the new permissions to the **Permission** collection.</span></span> 
  
## <a name="updating-folder-permissions-by-using-ews"></a><span data-ttu-id="b2871-312">Atualizando permissões de pasta usando EWS</span><span class="sxs-lookup"><span data-stu-id="b2871-312">Updating folder permissions by using EWS</span></span>
<span data-ttu-id="b2871-313"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="b2871-313"><a name="bk_updateews"> </a></span></span>

<span data-ttu-id="b2871-314">Você também pode atualizar as permissões de pasta para pastas específicas usando o EWS, combinando o processo de remoção e adição.</span><span class="sxs-lookup"><span data-stu-id="b2871-314">You can also update folder permissions for specific folders by using EWS by combining the removal and addition process.</span></span> <span data-ttu-id="b2871-315">Para atualizar as permissões:</span><span class="sxs-lookup"><span data-stu-id="b2871-315">To update the permissions:</span></span> 
  
1. <span data-ttu-id="b2871-316">Recupere as permissões atuais da pasta usando a operação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="b2871-316">Retrieve the folder's current permissions by using the **GetFolder** operation.</span></span> 
    
2. <span data-ttu-id="b2871-317">Envie uma lista atualizada de permissões usando a operação **UpdateFolder** .</span><span class="sxs-lookup"><span data-stu-id="b2871-317">Send an updated list of permissions by using the **UpdateFolder** operation.</span></span> 
    
<span data-ttu-id="b2871-318">Essas são as mesmas duas operações que você usa para [habilitar](#bk_enableews) ou [remover o acesso](#bk_removeews) usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="b2871-318">These are the same two operations you use to [enable](#bk_enableews) or [remove access](#bk_removeews) by using EWS.</span></span> <span data-ttu-id="b2871-319">A única diferença é que, quando você recebe a resposta **GetFolder** , ele conterá um conjunto de **permissões** para User.</span><span class="sxs-lookup"><span data-stu-id="b2871-319">The only difference is that when you receive the **GetFolder** response, it will contain a **Permission** set for user.</span></span> <span data-ttu-id="b2871-320">Basta substituir esse elemento de **permissão** existente pelo novo elemento **Permission** e, em seguida, enviar a operação **UpdateFolder** com o novo valor de **permissão** ou valores.</span><span class="sxs-lookup"><span data-stu-id="b2871-320">Simply replace that existing **Permission** element with the new **Permission** element, and then send the **UpdateFolder** operation with the new **Permission** value or values.</span></span> 
  
<span data-ttu-id="b2871-321">Se você tentar adicionar dois conjuntos de permissões para o mesmo usuário, receberá um valor de **ResponseCode** de **ErrorDuplicateUserIdsSpecified**.</span><span class="sxs-lookup"><span data-stu-id="b2871-321">If you try to add two sets of permissions for the same user, you will receive a **ResponseCode** value of **ErrorDuplicateUserIdsSpecified**.</span></span> <span data-ttu-id="b2871-322">Nesse caso, remova o valor de permissão desatualizado para o usuário da solicitação e repita a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2871-322">In that case, remove the outdated Permission value for the user from the request and then retry the request.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b2871-323">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="b2871-323">Next steps</span></span>

<span data-ttu-id="b2871-324">Depois de conceder a um usuário permissão para uma pasta específica, o usuário pode acessar a pasta como um representante.</span><span class="sxs-lookup"><span data-stu-id="b2871-324">After you give a user permission to a specific folder, the user can access the folder as a delegate.</span></span> <span data-ttu-id="b2871-325">Para saber mais, confira:</span><span class="sxs-lookup"><span data-stu-id="b2871-325">For more information, see:</span></span>
  
- [<span data-ttu-id="b2871-326">Acessar email como um representante usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b2871-326">Access email as a delegate by using EWS in Exchange</span></span>](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="b2871-327">Acessar um calendário como um representante usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b2871-327">Access a calendar as a delegate by using EWS in Exchange</span></span>](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="b2871-328">Acessar contatos como um representante usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b2871-328">Access contacts as a delegate by using EWS in Exchange</span></span>](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="b2871-329">Também consulte</span><span class="sxs-lookup"><span data-stu-id="b2871-329">See also</span></span>

- [<span data-ttu-id="b2871-330">Acesso de representante e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b2871-330">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)   
- [<span data-ttu-id="b2871-331">Adicionar e remover representantes usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b2871-331">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="b2871-332">Pastas e itens no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b2871-332">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    

