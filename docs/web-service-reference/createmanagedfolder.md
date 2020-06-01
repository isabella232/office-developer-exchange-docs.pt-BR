---
title: CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: cfdf01a9-0191-47c7-a7ad-5254d8bdee4a
description: O elemento CreateManagedFolder define uma solicitação para adicionar pastas personalizadas gerenciadas a uma caixa de correio.
ms.openlocfilehash: 01fe8b7341c38ad33089c56271434ad3f9a4e5f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458359"
---
# <a name="createmanagedfolder"></a><span data-ttu-id="77a19-103">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="77a19-103">CreateManagedFolder</span></span>

<span data-ttu-id="77a19-104">O elemento **CreateManagedFolder** define uma solicitação para adicionar pastas personalizadas gerenciadas a uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="77a19-104">The **CreateManagedFolder** element defines a request to add managed custom folders to a mailbox.</span></span> 
  
```xml
<CreateManagedFolder>
   <FolderNames/>
   <Mailbox/>
</CreateManagedFolder>
```

 <span data-ttu-id="77a19-105">**CreateManagedFolderRequestType**</span><span class="sxs-lookup"><span data-stu-id="77a19-105">**CreateManagedFolderRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="77a19-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="77a19-106">Attributes and elements</span></span>

<span data-ttu-id="77a19-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="77a19-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77a19-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="77a19-108">Attributes</span></span>

<span data-ttu-id="77a19-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="77a19-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="77a19-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="77a19-110">Child elements</span></span>

|<span data-ttu-id="77a19-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="77a19-111">**Element**</span></span>|<span data-ttu-id="77a19-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="77a19-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77a19-113">FolderNames</span><span class="sxs-lookup"><span data-stu-id="77a19-113">FolderNames</span></span>](foldernames.md) <br/> |<span data-ttu-id="77a19-114">Contém uma matriz de pastas gerenciadas nomeadas para adicionar a uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="77a19-114">Contains an array of named managed folders to add to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="77a19-115">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="77a19-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="77a19-116">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="77a19-116">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="77a19-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="77a19-117">Parent elements</span></span>

<span data-ttu-id="77a19-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="77a19-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="77a19-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="77a19-119">Remarks</span></span>

<span data-ttu-id="77a19-120">A conta da pessoa que está fazendo a solicitação deve ter permissões FullAccess na caixa de correio onde as pastas gerenciadas são criadas.</span><span class="sxs-lookup"><span data-stu-id="77a19-120">The account of the person who is making the request must have FullAccess permissions on the mailbox where the managed folders are created.</span></span> <span data-ttu-id="77a19-121">Você pode usar o parâmetro _-AccessRights _ com o cmdlet **Add-MailboxPermission** do Shell de gerenciamento do Exchange para atribuir a permissão FullAccess.</span><span class="sxs-lookup"><span data-stu-id="77a19-121">You can use the _ -AccessRights _ parameter with the Exchange Management Shell **Add-MailboxPermission** cmdlet to assign the FullAccess permission.</span></span> 
  
<span data-ttu-id="77a19-122">Embora você possa usar os serviços Web do Exchange para adicionar pastas gerenciadas a uma caixa de correio, não é possível usar os serviços Web do Exchange para acessar a lista de pastas gerenciadas que estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="77a19-122">Although you can use Exchange Web Services to add managed folders to a mailbox, you cannot use Exchange Web Services to access the list of managed folders that are available.</span></span> <span data-ttu-id="77a19-123">Para obter uma lista de pastas gerenciadas disponíveis, use o cmdlet **Get-ManagedFolder** do Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="77a19-123">To obtain a list of available managed folders, use the **get-managedfolder** Exchange Management Shell cmdlet.</span></span> <span data-ttu-id="77a19-124">A lista retornada pelo **cmdlet Get-ManagedFolder** conterá pastas personalizadas gerenciadas e pastas padrão gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="77a19-124">The list that is returned by the **get-managedfolder cmdlet** will contain both managed custom folders and managed default folders.</span></span> <span data-ttu-id="77a19-125">Você só pode adicionar pastas do tipo **ManagedCustomFolder** à caixa de correio usando a operação CreateManagedFolder.</span><span class="sxs-lookup"><span data-stu-id="77a19-125">You can only add folders of type **managedcustomfolder** to the mailbox by using the CreateManagedFolder operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="77a19-126">Você também pode obter uma lista de pastas gerenciadas usando a API DirectoryServices do Microsoft .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="77a19-126">You can also get a list of managed folders by using the DirectoryServices API of the Microsoft .NET Framework.</span></span> 
  
<span data-ttu-id="77a19-127">Você pode usar a [operação FindFolder](findfolder-operation.md) para localizar pastas gerenciadas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="77a19-127">You can use the [FindFolder operation](findfolder-operation.md) to find managed folders in a mailbox.</span></span> <span data-ttu-id="77a19-128">Pastas gerenciadas podem ser distinguidas Configurando o elemento [BaseShape](baseshape.md) para myproperties na solicitação.</span><span class="sxs-lookup"><span data-stu-id="77a19-128">Managed folders can be distinguished by setting the [BaseShape](baseshape.md) element to AllProperties in the request.</span></span> <span data-ttu-id="77a19-129">A resposta conterá um elemento [ManagedFolderInformation](managedfolderinformation.md) para distinguir as pastas gerenciadas das pastas do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="77a19-129">The response will contain a [ManagedFolderInformation](managedfolderinformation.md) element to distinguish the managed folders from the Exchange store folders.</span></span> <span data-ttu-id="77a19-130">Você pode excluir pastas gerenciadas da mesma maneira que exclui outros tipos de pasta.</span><span class="sxs-lookup"><span data-stu-id="77a19-130">You can delete managed folders in the same manner that you delete other folder types.</span></span> 
  
<span data-ttu-id="77a19-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="77a19-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77a19-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="77a19-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77a19-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="77a19-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="77a19-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="77a19-134">Schema Name</span></span>  <br/> |<span data-ttu-id="77a19-135">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="77a19-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="77a19-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="77a19-136">Validation File</span></span>  <br/> |<span data-ttu-id="77a19-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="77a19-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="77a19-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="77a19-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="77a19-139">False</span><span class="sxs-lookup"><span data-stu-id="77a19-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77a19-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="77a19-140">See also</span></span>



[<span data-ttu-id="77a19-141">Operação CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="77a19-141">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)
  
[<span data-ttu-id="77a19-142">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="77a19-142">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="77a19-143">Localizando pastas</span><span class="sxs-lookup"><span data-stu-id="77a19-143">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="77a19-144">Adicionando pastas gerenciadas</span><span class="sxs-lookup"><span data-stu-id="77a19-144">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

