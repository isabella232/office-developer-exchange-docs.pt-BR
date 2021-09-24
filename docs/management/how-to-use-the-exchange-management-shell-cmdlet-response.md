---
title: Usar a resposta de cmdlet Exchange Shell de Gerenciamento
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: dac8e526-11c6-4c2e-b9a2-f016b1fc738a
description: Saiba como usar a resposta de um cmdlet Exchange Shell de Gerenciamento em seu Exchange gerenciado.
ms.openlocfilehash: be66be31e435be1553eba16d8f367a79317618f2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520959"
---
# <a name="use-the-exchange-management-shell-cmdlet-response"></a>Usar a resposta de cmdlet Exchange Shell de Gerenciamento

Saiba como usar a resposta de um cmdlet Exchange Shell de Gerenciamento em seu Exchange gerenciado.
  
**Aplica-se a:** Exchange Online | Exchange Server 2013 | Office 365
  
Cada Exchange cmdlet do Shell de Gerenciamento retorna uma ou mais instâncias [PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx) que fornecem uma exibição consistente de qualquer objeto no ambiente Exchange Shell de Gerenciamento. Este artigo fornece informações sobre como usar as propriedades de uma instância **PSObject** para retornar os valores de propriedade do objeto Exchange Server API 2013 subjacente. 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a>Pré-requisitos para usar respostas de cmdlet
<a name="prerequisites_bk"> </a>

Para usar respostas de cmdlet, você precisa de uma referência ao namespace **System.Automation.Management.** 
  
> [!NOTE]
>  Ao usar o Visual Studio para criar um aplicativo, você deve adicionar uma referência ao assembly System.Mangagement.Automation.dll ao projeto. Você pode encontrar o assembly em um dos seguintes locais: 
> - Para Windows xp e Windows do Vista, o diretório de instalação Windows PowerShell ($PSHOME). 
> - Para os sistemas operacionais Windows 7 e Windows 8, a seguinte pasta: Windows\assembly\GAC_MSIL\System.Management.Automation. 
  
## <a name="windows-powershell-remote-runspace"></a>Windows PowerShell runspace remoto
<a name="usingremoterunspace_bk"> </a>

O Exchange Shell de Gerenciamento usa recursos de Windows PowerShell remotos para todos os comandos, até mesmo comandos executados no servidor local. Como resultado, todas as respostas Exchange cmdlets do Shell de Gerenciamento são XML serializados. Isso significa que, embora o objeto de resposta indique o tipo de objeto Exchange que foi usado para gerar a resposta, o objeto de resposta não pode ser lançado para o tipo de objeto Exchange do usuário; em vez disso, você deve usar o pacote de propriedades que é exposto pelo objeto de resposta para obter os valores do tipo Exchange objeto.
  
O pacote de propriedades no objeto de resposta contém um par de chave/valor para cada propriedade pública ou método no tipo Exchange objeto. O objeto response contém o nome do tipo de objeto Exchange subjacente; você pode usar esse nome para determinar o tipo de objeto Exchange representado pelo objeto de resposta para que você possa extrair a propriedade apropriada. Cada valor no pacote de propriedades também inclui informações de tipo para que você possa lançar o valor da propriedade para o tipo gerenciado apropriado.
  
## <a name="use-the-cmdlet-response"></a>Usar a resposta do cmdlet
<a name="usingPSObject_bk"> </a>

A [classe PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx) expõe as três propriedades públicas a seguir que contêm os valores do objeto da API Exchange 2013 subjacente: [Propriedades,](https://msdn.microsoft.com/library/system.management.automation.psobject.properties%28VS.85%29.aspx) [Métodos](https://msdn.microsoft.com/library/system.management.automation.psobject.methods%28VS.85%29.aspx)e [Membros](https://msdn.microsoft.com/library/system.management.automation.psobject.members%28VS.85%29.aspx). Cada propriedade exposta pelo objeto api Exchange 2013 tem um par de chave/valor correspondente nas **propriedades Properties** e **Members.** Seu aplicativo pode indexar a **coleção Properties** pelo nome de uma propriedade para recuperar o valor da propriedade. 
  
Você pode usar a propriedade **TypeNames** da instância **PSObject** para determinar o tipo do objeto Exchange subjacente encapsulado pela instância **PSObject.** A **propriedade TypeNames** é uma coleção de cadeias de caracteres que contém a hierarquia de objetos do tipo representado. Você pode usar esses nomes para determinar o objeto representado pela instância **PSObject** para que você possa extrair a propriedade apropriada. 
  
O exemplo de código a seguir usa a resposta do cmdlet para imprimir o conteúdo da coleção **Properties** de uma **instância PSObject** no console. O exemplo de código requer uma referência ao namespace **System.Automation.Management.** 
  
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

- [Criar ferramentas do Shell de Gerenciamento do Exchange](create-exchange-management-shell-tools.md)   
- [Obter uma lista de usuários de email usando o Shell Exchange Gerenciamento](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
    

