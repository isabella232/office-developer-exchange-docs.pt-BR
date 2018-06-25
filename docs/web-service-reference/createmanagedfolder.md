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
description: O elemento de CreateManagedFolder define uma solicitação para adicionar pastas personalizadas gerenciadas para uma caixa de correio.
ms.openlocfilehash: 4acc931de2a8665db092c3b309d914f0a3c67558
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751618"
---
# <a name="createmanagedfolder"></a><span data-ttu-id="d8200-103">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="d8200-103">CreateManagedFolder</span></span>

<span data-ttu-id="d8200-104">O elemento de **CreateManagedFolder** define uma solicitação para adicionar pastas personalizadas gerenciadas para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d8200-104">The **CreateManagedFolder** element defines a request to add managed custom folders to a mailbox.</span></span> 
  
```xml
<CreateManagedFolder>
   <FolderNames/>
   <Mailbox/>
</CreateManagedFolder>
```

 <span data-ttu-id="d8200-105">**CreateManagedFolderRequestType**</span><span class="sxs-lookup"><span data-stu-id="d8200-105">**CreateManagedFolderRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8200-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d8200-106">Attributes and elements</span></span>

<span data-ttu-id="d8200-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d8200-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8200-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d8200-108">Attributes</span></span>

<span data-ttu-id="d8200-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d8200-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8200-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d8200-110">Child elements</span></span>

|<span data-ttu-id="d8200-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d8200-111">**Element**</span></span>|<span data-ttu-id="d8200-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d8200-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8200-113">Nomes de pastas</span><span class="sxs-lookup"><span data-stu-id="d8200-113">FolderNames</span></span>](foldernames.md) <br/> |<span data-ttu-id="d8200-114">Contém uma matriz de nomeada pastas gerenciadas para adicionar uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d8200-114">Contains an array of named managed folders to add to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d8200-115">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="d8200-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="d8200-116">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="d8200-116">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d8200-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d8200-117">Parent elements</span></span>

<span data-ttu-id="d8200-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d8200-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d8200-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="d8200-119">Remarks</span></span>

<span data-ttu-id="d8200-120">A conta da pessoa que está fazendo a solicitação deve ter permissões de FullAccess na caixa de correio onde as pastas gerenciadas são criadas.</span><span class="sxs-lookup"><span data-stu-id="d8200-120">The account of the person who is making the request must have FullAccess permissions on the mailbox where the managed folders are created.</span></span> <span data-ttu-id="d8200-121">Você pode usar o parâmetro de _ _ - AccessRights com o cmdlet do Shell de gerenciamento do Exchange **Add-MailboxPermission** para atribuir a permissão FullAccess.</span><span class="sxs-lookup"><span data-stu-id="d8200-121">You can use the _ -AccessRights _ parameter with the Exchange Management Shell **Add-MailboxPermission** cmdlet to assign the FullAccess permission.</span></span> 
  
<span data-ttu-id="d8200-122">Embora você possa usar os serviços Web do Exchange para adicionar pastas gerenciadas para uma caixa de correio, você não pode usar os serviços Web do Exchange para acessar a lista de pastas gerenciadas que estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="d8200-122">Although you can use Exchange Web Services to add managed folders to a mailbox, you cannot use Exchange Web Services to access the list of managed folders that are available.</span></span> <span data-ttu-id="d8200-123">Para obter uma lista de pastas gerenciadas disponíveis, use o cmdlet do Shell de gerenciamento do Exchange de **get-managedfolder** .</span><span class="sxs-lookup"><span data-stu-id="d8200-123">To obtain a list of available managed folders, use the **get-managedfolder** Exchange Management Shell cmdlet.</span></span> <span data-ttu-id="d8200-124">A lista retornada pelo **cmdlet get-managedfolder** conterá pastas personalizadas gerenciadas e a pastas padrão gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="d8200-124">The list that is returned by the **get-managedfolder cmdlet** will contain both managed custom folders and managed default folders.</span></span> <span data-ttu-id="d8200-125">Você somente pode adicionar pastas do tipo **managedcustomfolder** à caixa de correio usando a operação CreateManagedFolder.</span><span class="sxs-lookup"><span data-stu-id="d8200-125">You can only add folders of type **managedcustomfolder** to the mailbox by using the CreateManagedFolder operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d8200-126">Você também pode obter uma lista de pastas gerenciadas usando a API DirectoryServices do Microsoft .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="d8200-126">You can also get a list of managed folders by using the DirectoryServices API of the Microsoft .NET Framework.</span></span> 
  
<span data-ttu-id="d8200-127">Você pode usar a [operação FindFolder](findfolder-operation.md) para localizar pastas gerenciadas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d8200-127">You can use the [FindFolder operation](findfolder-operation.md) to find managed folders in a mailbox.</span></span> <span data-ttu-id="d8200-128">Pastas gerenciadas podem ser diferenciadas, definindo o elemento [BaseShape](baseshape.md) para AllProperties na solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8200-128">Managed folders can be distinguished by setting the [BaseShape](baseshape.md) element to AllProperties in the request.</span></span> <span data-ttu-id="d8200-129">A resposta conterá um elemento [ManagedFolderInformation](managedfolderinformation.md) para distinguir as pastas gerenciadas a partir das pastas de repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d8200-129">The response will contain a [ManagedFolderInformation](managedfolderinformation.md) element to distinguish the managed folders from the Exchange store folders.</span></span> <span data-ttu-id="d8200-130">Você pode excluir pastas gerenciadas da mesma maneira que você exclua outros tipos de pasta.</span><span class="sxs-lookup"><span data-stu-id="d8200-130">You can delete managed folders in the same manner that you delete other folder types.</span></span> 
  
<span data-ttu-id="d8200-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d8200-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8200-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d8200-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8200-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="d8200-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d8200-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d8200-134">Schema Name</span></span>  <br/> |<span data-ttu-id="d8200-135">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d8200-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d8200-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d8200-136">Validation File</span></span>  <br/> |<span data-ttu-id="d8200-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d8200-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d8200-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d8200-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="d8200-139">False</span><span class="sxs-lookup"><span data-stu-id="d8200-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8200-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="d8200-140">See also</span></span>



[<span data-ttu-id="d8200-141">Operação CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="d8200-141">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)
  
[<span data-ttu-id="d8200-142">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="d8200-142">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="d8200-143">Localizando pastas</span><span class="sxs-lookup"><span data-stu-id="d8200-143">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="d8200-144">Adicionando pastas gerenciadas</span><span class="sxs-lookup"><span data-stu-id="d8200-144">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

