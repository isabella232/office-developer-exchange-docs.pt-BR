---
title: Use a resposta de cmdlet do Shell de gerenciamento do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dac8e526-11c6-4c2e-b9a2-f016b1fc738a
description: Saiba como usar a resposta de um cmdlet do Shell de gerenciamento do Exchange em um aplicativo gerenciado do Exchange.
ms.openlocfilehash: 5edf75afd556f67e815bc519c87586f2f62f057b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750962"
---
# <a name="use-the-exchange-management-shell-cmdlet-response"></a><span data-ttu-id="9d830-103">Use a resposta de cmdlet do Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="9d830-103">Use the Exchange Management Shell cmdlet response</span></span>

<span data-ttu-id="9d830-104">Saiba como usar a resposta de um cmdlet do Shell de gerenciamento do Exchange em um aplicativo gerenciado do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d830-104">Learn how to use the response from an Exchange Management Shell cmdlet in your Exchange managed application.</span></span>
  
<span data-ttu-id="9d830-105">**Aplica-se a:** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="9d830-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="9d830-106">Cada cmdlet do Shell de gerenciamento do Exchange retorna uma ou mais instâncias [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) que fornecem uma visão consistente de qualquer objeto no ambiente do Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d830-106">Each Exchange Management Shell cmdlet returns one or more [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) instances that provide a consistent view of any object in the Exchange Management Shell environment.</span></span> <span data-ttu-id="9d830-107">Este artigo fornece informações sobre como usar as propriedades de uma instância de **PSObject** para retornar os valores de propriedade do objeto subjacente API do Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9d830-107">This article provides information about how to use the properties of a **PSObject** instance to return the property values of the underlying Exchange Server 2013 API object.</span></span> 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a><span data-ttu-id="9d830-108">Pré-requisitos para usar o cmdlet respostas</span><span class="sxs-lookup"><span data-stu-id="9d830-108">Prerequisites for using cmdlet responses</span></span>
<span data-ttu-id="9d830-109"><a name="prerequisites_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="9d830-109"></span></span>

<span data-ttu-id="9d830-110">Para usar o cmdlet respostas, você precisa de uma referência ao namespace **System.Automation.Management** .</span><span class="sxs-lookup"><span data-stu-id="9d830-110">To use cmdlet responses, you need a reference to the **System.Automation.Management** namespace.</span></span> 
  
> [!NOTE]
>  <span data-ttu-id="9d830-111">Quando você estiver usando o Visual Studio para criar um aplicativo, você deve adicionar uma referência para o assembly System.Mangagement.Automation.dll ao projeto.</span><span class="sxs-lookup"><span data-stu-id="9d830-111">When you are using Visual Studio to create an application, you must add a reference to the System.Mangagement.Automation.dll assembly to the project.</span></span> <span data-ttu-id="9d830-112">Você pode encontrar o assembly em um dos seguintes locais:</span><span class="sxs-lookup"><span data-stu-id="9d830-112">You can find the assembly in one of the following locations:</span></span> 
> - <span data-ttu-id="9d830-113">Para Windows XP e Windows Vista sistemas operacionais, o diretório de instalação do Windows PowerShell ($PSHOME).</span><span class="sxs-lookup"><span data-stu-id="9d830-113">For Windows XP and Windows Vista operating systems, the Windows PowerShell installation directory ($PSHOME).</span></span> 
> - <span data-ttu-id="9d830-114">Para os sistemas de operacionais Windows 7 e Windows 8, a seguinte pasta: Windows\assembly\GAC_MSIL\System.Management.Automation.</span><span class="sxs-lookup"><span data-stu-id="9d830-114">For the Windows 7 and Windows 8 operating systems, the following folder: Windows\assembly\GAC_MSIL\System.Management.Automation.</span></span> 
  
## <a name="windows-powershell-remote-runspace"></a><span data-ttu-id="9d830-115">Espaço de trabalho remoto do Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="9d830-115">Windows PowerShell remote runspace</span></span>
<span data-ttu-id="9d830-116"><a name="usingremoterunspace_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="9d830-116"></span></span>

<span data-ttu-id="9d830-117">O Shell de gerenciamento do Exchange utiliza os recursos de Windows PowerShell remotos para todos os comandos, até os comandos que são executados no servidor local.</span><span class="sxs-lookup"><span data-stu-id="9d830-117">The Exchange Management Shell uses remote Windows PowerShell features for all commands, even commands that are run on the local server.</span></span> <span data-ttu-id="9d830-118">Como resultado, todas as respostas do Shell de gerenciamento do Exchange cmdlets são serializados XML.</span><span class="sxs-lookup"><span data-stu-id="9d830-118">As a result, all responses from Exchange Management Shell cmdlets are serialized XML.</span></span> <span data-ttu-id="9d830-119">Isso significa que, embora no objeto response indica o tipo de objeto do Exchange que foi usado para gerar a resposta, o objeto de resposta não pode ser convertido para o tipo de objeto do Exchange; em vez disso, você deve usar o recipiente de propriedades que é exposto por no objeto response para obter os valores de tipo de objeto do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d830-119">This means that although the response object indicates the Exchange object type that was used to generate the response, the response object cannot be cast to the Exchange object type; instead, you must use the property bag that is exposed by the response object to obtain the values from the Exchange object type.</span></span>
  
<span data-ttu-id="9d830-120">O recipiente de propriedades no objeto response contém um par de chave/valor para cada propriedade pública ou o método no tipo de objeto do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d830-120">The property bag in the response object contains a key/value pair for each public property or method in the Exchange object type.</span></span> <span data-ttu-id="9d830-121">No objeto response contém o nome do tipo de objeto subjacente Exchange; Você pode usar esse nome para determinar o tipo de objeto do Exchange que é representado pelo objeto de resposta para que você pode extrair a propriedade apropriada.</span><span class="sxs-lookup"><span data-stu-id="9d830-121">The response object contains the name of the underlying Exchange object type; you can use this name to determine the Exchange object type that is represented by the response object so that you can extract the appropriate property.</span></span> <span data-ttu-id="9d830-122">Cada valor no recipiente de propriedades também inclui informações sobre tipo de forma que você pode converter o valor da propriedade para o tipo apropriado de gerenciada.</span><span class="sxs-lookup"><span data-stu-id="9d830-122">Each value in the property bag also includes type information so that you can cast the property value to the appropriate managed type.</span></span>
  
## <a name="use-the-cmdlet-response"></a><span data-ttu-id="9d830-123">Use a cmdlet de resposta</span><span class="sxs-lookup"><span data-stu-id="9d830-123">Use the cmdlet response</span></span>
<span data-ttu-id="9d830-124"><a name="usingPSObject_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="9d830-124"></span></span>

<span data-ttu-id="9d830-125">A classe de [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) expõe as seguintes três propriedades públicas que contêm os valores do objeto subjacente API do Exchange 2013: [Propriedades](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [métodos](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.methods%28VS.85%29.aspx)e [membros](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.members%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="9d830-125">The [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) class exposes the following three public properties that contain the values of the underlying Exchange 2013 API object: [Properties](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [Methods](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.methods%28VS.85%29.aspx), and [Members](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.members%28VS.85%29.aspx).</span></span> <span data-ttu-id="9d830-126">Cada propriedade que é exposta pelo objeto API do Exchange 2013 tem um par de chave/valor correspondente nas propriedades da **Propriedades** e **membros** .</span><span class="sxs-lookup"><span data-stu-id="9d830-126">Each property that is exposed by the Exchange 2013 API object has a corresponding key/value pair in the **Properties** and **Members** properties.</span></span> <span data-ttu-id="9d830-127">Seu aplicativo pode indexar a coleção **Properties** pelo nome de uma propriedade para recuperar o valor da propriedade.</span><span class="sxs-lookup"><span data-stu-id="9d830-127">Your application can index the **Properties** collection by the name of a property to retrieve the value of the property.</span></span> 
  
<span data-ttu-id="9d830-128">Você pode usar a propriedade **TypeNames** da instância **PSObject** para determinar o tipo do objeto subjacente Exchange encapsulado pela instância **PSObject** .</span><span class="sxs-lookup"><span data-stu-id="9d830-128">You can use the **TypeNames** property of the **PSObject** instance to determine the type of the underlying Exchange object that is encapsulated by the **PSObject** instance.</span></span> <span data-ttu-id="9d830-129">A propriedade **TypeNames** é uma coleção de cadeias de caracteres que contém a hierarquia do objeto do tipo representado.</span><span class="sxs-lookup"><span data-stu-id="9d830-129">The **TypeNames** property is a collection of strings that contains the object hierarchy of the represented type.</span></span> <span data-ttu-id="9d830-130">Você pode usar esses nomes para determinar o objeto representado pela instância **PSObject** para que você pode extrair a propriedade apropriada.</span><span class="sxs-lookup"><span data-stu-id="9d830-130">You can use these names to determine the object that is represented by the **PSObject** instance so that you can extract the appropriate property.</span></span> 
  
<span data-ttu-id="9d830-131">O exemplo de código a seguir usa a resposta de cmdlet para imprimir o conteúdo do conjunto de **Propriedades** de uma instância de **PSObject** no console.</span><span class="sxs-lookup"><span data-stu-id="9d830-131">The following code example uses the cmdlet response to print the contents of the **Properties** collection of a **PSObject** instance on the console.</span></span> <span data-ttu-id="9d830-132">O exemplo de código requer uma referência ao namespace **System.Automation.Management** .</span><span class="sxs-lookup"><span data-stu-id="9d830-132">The code example requires a reference to the **System.Automation.Management** namespace.</span></span> 
  
```cs
foreach (PSPropertyInfo propertyInfo in psObject.Properties)
{
    Console.WriteLine(string.Format("{0}: {1}",
        propertyInfo.Name, propertyInfo.Value);
}
```

<br/>

```vb
For Each PropertyInfo As PSProperty In ObjectInfo.Properties
    Console.WriteLine(String.Format("{0}: {1}", PropertyInfo.Name, PropertyInfo.Value))
Next

```

## <a name="see-also"></a><span data-ttu-id="9d830-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="9d830-133">See also</span></span>

- [<span data-ttu-id="9d830-134">Criar ferramentas do Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="9d830-134">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md)   
- [<span data-ttu-id="9d830-135">Obter uma lista de usuários de email usando o Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="9d830-135">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
    

