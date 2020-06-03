---
title: Usar a resposta do cmdlet do Shell de gerenciamento do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dac8e526-11c6-4c2e-b9a2-f016b1fc738a
description: Saiba como usar a resposta de um cmdlet do Shell de gerenciamento do Exchange em seu aplicativo gerenciado do Exchange.
ms.openlocfilehash: c1b81356ab5dc288ab08287d47581871c36beb05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44435699"
---
# <a name="use-the-exchange-management-shell-cmdlet-response"></a>Usar a resposta do cmdlet do Shell de gerenciamento do Exchange

Saiba como usar a resposta de um cmdlet do Shell de gerenciamento do Exchange em seu aplicativo gerenciado do Exchange.
  
**Aplica-se a:** Exchange Online | Exchange Server 2013 | Office 365
  
Cada cmdlet do Shell de gerenciamento do Exchange retorna uma ou mais instâncias de [PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx) que fornecem um modo de exibição consistente de qualquer objeto no ambiente do Shell de gerenciamento do Exchange. Este artigo fornece informações sobre como usar as propriedades de uma instância de **PSObject** para retornar os valores de Propriedade do objeto de API subjacente do Exchange Server 2013. 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a>Pré-requisitos para usar respostas de cmdlet
<a name="prerequisites_bk"> </a>

Para usar respostas de cmdlet, você precisa de uma referência ao namespace **System. Automation. Management** . 
  
> [!NOTE]
>  Quando você estiver usando o Visual Studio para criar um aplicativo, você deve adicionar uma referência ao assembly System. mangagement. Automation. dll para o projeto. Você pode encontrar o assembly em um dos seguintes locais: 
> - Para os sistemas operacionais Windows XP e Windows Vista, o diretório de instalação do Windows PowerShell ($PSHOME). 
> - Para os sistemas operacionais Windows 7 e Windows 8, a seguinte pasta: Windows\assembly\ GAC_MSIL \System.Management.Automation. 
  
## <a name="windows-powershell-remote-runspace"></a>Runspace remoto do Windows PowerShell
<a name="usingremoterunspace_bk"> </a>

O Shell de gerenciamento do Exchange usa recursos remotos do Windows PowerShell para todos os comandos, até mesmo comandos que são executados no servidor local. Como resultado, todas as respostas dos cmdlets do Shell de gerenciamento do Exchange são XML serializados. Isso significa que, embora o objeto Response indique o tipo de objeto do Exchange usado para gerar a resposta, o objeto Response não pode ser convertido para o tipo de objeto do Exchange; em vez disso, você deve usar o conjunto de propriedades que é exposto pelo objeto Response para obter os valores do tipo de objeto do Exchange.
  
O recipiente de propriedades no objeto Response contém um par chave/valor para cada propriedade pública ou método no tipo de objeto do Exchange. O objeto Response contém o nome do tipo de objeto subjacente do Exchange; Você pode usar esse nome para determinar o tipo de objeto do Exchange que é representado pelo objeto Response para que você possa extrair a propriedade apropriada. Cada valor no recipiente de propriedades também inclui informações de tipo para que você possa converter o valor da propriedade para o tipo gerenciado apropriado.
  
## <a name="use-the-cmdlet-response"></a>Usar a resposta do cmdlet
<a name="usingPSObject_bk"> </a>

A classe [PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx) expõe as três propriedades públicas a seguir que contêm os valores do objeto de API do Exchange 2013 subjacente: [Propriedades](https://msdn.microsoft.com/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [métodos](https://msdn.microsoft.com/library/system.management.automation.psobject.methods%28VS.85%29.aspx)e [Membros](https://msdn.microsoft.com/library/system.management.automation.psobject.members%28VS.85%29.aspx). Cada propriedade exposta pelo objeto API do Exchange 2013 tem um par chave/valor correspondente nas propriedades **Properties** e **Members** . Seu aplicativo pode indexar a coleção **Properties** pelo nome de uma propriedade para recuperar o valor da propriedade. 
  
Você pode usar a propriedade **TypeNames** da instância de **PSObject** para determinar o tipo do objeto subjacente do Exchange que é encapsulado pela instância de **PSObject** . A propriedade **TypeNames** é uma coleção de cadeias de caracteres que contém a hierarquia de objeto do tipo representado. Você pode usar esses nomes para determinar o objeto que é representado pela instância de **PSObject** para que você possa extrair a propriedade apropriada. 
  
O exemplo de código a seguir usa a resposta do cmdlet para imprimir o conteúdo da coleção **Properties** de uma instância de **PSObject** no console. O exemplo de código requer uma referência ao namespace **System. Automation. Management** . 
  
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
    

