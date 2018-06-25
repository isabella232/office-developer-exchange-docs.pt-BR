---
title: ServerVersion (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a
description: O elemento ServerVersion representa o número da versão do computador que está executando o Microsoft Exchange Server.
ms.openlocfilehash: ef0562e166094d75d0dd92f5f48bb558e11a2cad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825391"
---
# <a name="serverversion-pox"></a><span data-ttu-id="685c9-103">ServerVersion (POX)</span><span class="sxs-lookup"><span data-stu-id="685c9-103">ServerVersion (POX)</span></span>

<span data-ttu-id="685c9-104">O elemento **ServerVersion** representa o número da versão do computador que está executando o Microsoft Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="685c9-104">The **ServerVersion** element represents the version number of the computer that is running Microsoft Exchange Server.</span></span> 
  
- [<span data-ttu-id="685c9-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="685c9-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="685c9-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="685c9-106">Response (POX)</span></span>](response-pox.md)
- [<span data-ttu-id="685c9-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="685c9-107">Account (POX)</span></span>](account-pox.md)
- [<span data-ttu-id="685c9-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="685c9-108">Protocol (POX)</span></span>](protocol-pox.md)
- [<span data-ttu-id="685c9-109">ServerVersion (POX)</span><span class="sxs-lookup"><span data-stu-id="685c9-109">ServerVersion (POX)</span></span>](serverversion-pox.md)
  
```xml
<ServerVersion/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="685c9-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="685c9-110">Attributes and elements</span></span>

<span data-ttu-id="685c9-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="685c9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="685c9-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="685c9-112">Attributes</span></span>

<span data-ttu-id="685c9-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="685c9-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="685c9-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="685c9-114">Child elements</span></span>

<span data-ttu-id="685c9-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="685c9-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="685c9-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="685c9-116">Parent elements</span></span>

|<span data-ttu-id="685c9-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="685c9-117">**Element**</span></span>|<span data-ttu-id="685c9-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="685c9-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="685c9-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="685c9-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="685c9-120">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange que tenha a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="685c9-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="685c9-121">Text value</span><span class="sxs-lookup"><span data-stu-id="685c9-121">Text value</span></span>

<span data-ttu-id="685c9-122">O valor de texto representa o número de versão do Exchange server.</span><span class="sxs-lookup"><span data-stu-id="685c9-122">The text value represents the Exchange server version number.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="685c9-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="685c9-123">Remarks</span></span>

<span data-ttu-id="685c9-124">O valor de **ServerVersion** só será válido se o elemento de [Tipo POX ()](type-pox.md) é igual a EXCH ou EXPR.</span><span class="sxs-lookup"><span data-stu-id="685c9-124">The **ServerVersion** value is only valid if the [Type (POX)](type-pox.md) element is equal to EXCH or EXPR.</span></span> <span data-ttu-id="685c9-125">O valor de **ServerVersion** é um número hexadecimal que contém o MajorVersion, MinorVersion e MajorBuildNumber do servidor.</span><span class="sxs-lookup"><span data-stu-id="685c9-125">The **ServerVersion** value is a hexadecimal number that contains the MajorVersion, MinorVersion, and MajorBuildNumber of the server.</span></span> 
  
## <a name="example"></a><span data-ttu-id="685c9-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="685c9-126">Example</span></span>

<span data-ttu-id="685c9-127">As seguir coverts exemplo um **ServerVersion** valor que é retornado em uma resposta de descoberta automática para obter e exibir os MajorVersion, MinorVersion e MajorBuildNumber.</span><span class="sxs-lookup"><span data-stu-id="685c9-127">The following example coverts a **ServerVersion** value that is returned in an Autodiscover response to obtain and display the MajorVersion, MinorVersion, and MajorBuildNumber.</span></span> <span data-ttu-id="685c9-128">Este exemplo permite que você insira um valor hexadecimal para o valor de **ServerVersion** .</span><span class="sxs-lookup"><span data-stu-id="685c9-128">This example enables you to enter a hexadecimal value for the **ServerVersion** value.</span></span> <span data-ttu-id="685c9-129">Se nenhum valor **ServerVersion** for inserido, o valor padrão **ServerVersion** 738180DA é usado.</span><span class="sxs-lookup"><span data-stu-id="685c9-129">If no **ServerVersion** value is entered, a default **ServerVersion** value of 738180DA is used.</span></span> 
  
```csharp
static void Main(string[] args)
{
    // Convert a ServerVersion value that is returned from an Autodiscover request.
    // The value is a hex value and can be converted to the MajorVersion, MinorVersion,
    // and MajorBuildNumber.
    Console.WriteLine("Enter ServerVersion returned from the Autodiscover (eg. 738180DA) and Enter.");
    Console.WriteLine("To use the default ServerVersion of 738180DA, just hit Enter.");
    // Get the hexadecimal ServerVersion value.
    string serverversionhex = Console.ReadLine();
    // If nothing is entered, use the default server version of "738180DA"
    if (serverversionhex == "")
    {
        serverversionhex = "738180DA";
    }
    Console.WriteLine("ServerVersion (Hex) = " + serverversionhex);
    string serverversionbinary = Convert.ToString(Convert.ToInt32(serverversionhex, 16), 2);
    // The ServerVersion (binary) should be 32 bits in length. If the 
    // server version in binary is a length of 31 characters, the leading
    // zero has been removed in the conversion process. Put the missing zero back.
    if (serverversionbinary.Length == 31)
    {
        serverversionbinary = String.Concat("0", serverversionbinary);
    }
    Console.WriteLine("ServerVersion (bin) = " + serverversionbinary);
    // The first 4 bits represent a number used for comparison against  
    // older version number structures. You can ignore this.
    // The next 6 bits represent the major version number.
    int majorversion = Convert.ToInt32(serverversionbinary.Substring(4, 6), 2);
    Console.WriteLine("MajorVersion: " + majorversion);
    // The next 6 bits represent the minor version number.
    int minorversion = Convert.ToInt32(serverversionbinary.Substring(10, 6), 2);
    Console.WriteLine("MinorVersion: " + minorversion);
    
    // The next bit represent a flag - you can ignore this.
    // The next 15 bits represent the major build number.
    int majorbuild = Convert.ToInt32(serverversionbinary.Substring(17, 15), 2);
    Console.WriteLine("MajorBuildVersion: " + majorbuild);
    Console.WriteLine("\n\nPress any key to continue");
    Console.ReadKey();
}
```

## <a name="see-also"></a><span data-ttu-id="685c9-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="685c9-130">See also</span></span>

- [<span data-ttu-id="685c9-131">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="685c9-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

