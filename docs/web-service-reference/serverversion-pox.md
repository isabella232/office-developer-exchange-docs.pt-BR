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
ms.openlocfilehash: 3ef531a69d2dd00ee9784c9eb191684ce517e842
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461965"
---
# <a name="serverversion-pox"></a>ServerVersion (POX)

O elemento **ServerVersion** representa o número da versão do computador que está executando o Microsoft Exchange Server. 
  
- [Descoberta automática (POX)](autodiscover-pox.md) 
- [Resposta (POX)](response-pox.md)
- [Conta (POX)](account-pox.md)
- [Protocol (POX)](protocol-pox.md)
- [ServerVersion (POX)](serverversion-pox.md)
  
```xml
<ServerVersion/>
```

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange que tem a função de servidor de acesso para Cliente instalada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o número da versão do Exchange Server.
  
## <a name="remarks"></a>Comentários

O valor **ServerVersion** só será válido se o elemento [Type (POX)](type-pox.md) for igual a Exch ou expr. O valor **ServerVersion** é um número hexadecimal que contém o MajorVersion, o MinorVersion e o MajorBuildNumber do servidor. 
  
## <a name="example"></a>Exemplo

O exemplo a seguir retorna um valor **ServerVersion** que é retornado em uma resposta de descoberta automática para obter e exibir o MajorVersion, MinorVersion e MajorBuildNumber. Este exemplo permite que você insira um valor hexadecimal para o valor **ServerVersion** . Se nenhum valor **ServerVersion** for inserido, um valor padrão de **ServerVersion** de 738180DA será usado. 
  
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

## <a name="see-also"></a>Confira também

- [Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

