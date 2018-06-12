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
# <a name="use-the-exchange-management-shell-cmdlet-response"></a>Use a resposta de cmdlet do Shell de gerenciamento do Exchange

Saiba como usar a resposta de um cmdlet do Shell de gerenciamento do Exchange em um aplicativo gerenciado do Exchange.
  
**Aplica-se a:** Exchange Online | Exchange Server 2013 | Office 365
  
Cada cmdlet do Shell de gerenciamento do Exchange retorna uma ou mais instâncias [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) que fornecem uma visão consistente de qualquer objeto no ambiente do Shell de gerenciamento do Exchange. Este artigo fornece informações sobre como usar as propriedades de uma instância de **PSObject** para retornar os valores de propriedade do objeto subjacente API do Exchange Server 2013. 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a>Pré-requisitos para usar o cmdlet respostas
<a name="prerequisites_bk"> </a>

Para usar o cmdlet respostas, você precisa de uma referência ao namespace **System.Automation.Management** . 
  
> [!NOTE]
>  Quando você estiver usando o Visual Studio para criar um aplicativo, você deve adicionar uma referência para o assembly System.Mangagement.Automation.dll ao projeto. Você pode encontrar o assembly em um dos seguintes locais: 
> - Para Windows XP e Windows Vista sistemas operacionais, o diretório de instalação do Windows PowerShell ($PSHOME). 
> - Para os sistemas de operacionais Windows 7 e Windows 8, a seguinte pasta: Windows\assembly\GAC_MSIL\System.Management.Automation. 
  
## <a name="windows-powershell-remote-runspace"></a>Espaço de trabalho remoto do Windows PowerShell
<a name="usingremoterunspace_bk"> </a>

O Shell de gerenciamento do Exchange utiliza os recursos de Windows PowerShell remotos para todos os comandos, até os comandos que são executados no servidor local. Como resultado, todas as respostas do Shell de gerenciamento do Exchange cmdlets são serializados XML. Isso significa que, embora no objeto response indica o tipo de objeto do Exchange que foi usado para gerar a resposta, o objeto de resposta não pode ser convertido para o tipo de objeto do Exchange; em vez disso, você deve usar o recipiente de propriedades que é exposto por no objeto response para obter os valores de tipo de objeto do Exchange.
  
O recipiente de propriedades no objeto response contém um par de chave/valor para cada propriedade pública ou o método no tipo de objeto do Exchange. No objeto response contém o nome do tipo de objeto subjacente Exchange; Você pode usar esse nome para determinar o tipo de objeto do Exchange que é representado pelo objeto de resposta para que você pode extrair a propriedade apropriada. Cada valor no recipiente de propriedades também inclui informações sobre tipo de forma que você pode converter o valor da propriedade para o tipo apropriado de gerenciada.
  
## <a name="use-the-cmdlet-response"></a>Use a cmdlet de resposta
<a name="usingPSObject_bk"> </a>

A classe de [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) expõe as seguintes três propriedades públicas que contêm os valores do objeto subjacente API do Exchange 2013: [Propriedades](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [métodos](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.methods%28VS.85%29.aspx)e [membros](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.members%28VS.85%29.aspx). Cada propriedade que é exposta pelo objeto API do Exchange 2013 tem um par de chave/valor correspondente nas propriedades da **Propriedades** e **membros** . Seu aplicativo pode indexar a coleção **Properties** pelo nome de uma propriedade para recuperar o valor da propriedade. 
  
Você pode usar a propriedade **TypeNames** da instância **PSObject** para determinar o tipo do objeto subjacente Exchange encapsulado pela instância **PSObject** . A propriedade **TypeNames** é uma coleção de cadeias de caracteres que contém a hierarquia do objeto do tipo representado. Você pode usar esses nomes para determinar o objeto representado pela instância **PSObject** para que você pode extrair a propriedade apropriada. 
  
O exemplo de código a seguir usa a resposta de cmdlet para imprimir o conteúdo do conjunto de **Propriedades** de uma instância de **PSObject** no console. O exemplo de código requer uma referência ao namespace **System.Automation.Management** . 
  
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

## <a name="see-also"></a>Confira também

- [Criar ferramentas do Shell de gerenciamento do Exchange](create-exchange-management-shell-tools.md)   
- [Obter uma lista de usuários de email usando o Shell de gerenciamento do Exchange](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
    

