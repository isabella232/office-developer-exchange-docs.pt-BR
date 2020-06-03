---
title: Função função cchksgfiles. Delete
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- dllExport
ms.assetid: 869e927f-7df2-4247-88ef-b8b05b29a700
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: 38cb72b42727855f652de607bb2a02ecdeaae16e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44447047"
---
# <a name="cchksgfilesdelete-function"></a>Função função cchksgfiles. Delete

**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Destrói uma instância existente da classe **função cchksgfiles** . Você deve chamar essa função depois que o aplicativo tiver concluído o trabalho com o objeto especificado. 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a>Parâmetros

### <a name="pcchecksgfiles"></a>pcchecksgfiles 
  
Parâmetro de entrada. Um ponteiro para um objeto **CCheckSGFiles** existente. A memória associada ao objeto será liberada. 
    
## <a name="return-value"></a>Valor retornado

Nenhum.
  
## <a name="remarks"></a>Comentários

A função **delete** libera a memória associada ao objeto **CCheckSGFiles** . Depois de chamar **delete**, o ponteiro passado no parâmetro *pcchecksgfiles* será inválido e nenhuma outra operação poderá ser executada nesse objeto. 
  
Se o aplicativo usar a função **ErrCheckDbPages** , o aplicativo deverá liberar o buffer de memória manualmente; a função **excluir** não a liberará. 
  
Se você estiver usando o CHKSGFILES em um aplicativo multi-threaded, deverá chamar a função **excluir** na parte de thread único do aplicativo e poderá chamá-la somente uma vez para cada objeto **CCheckSGFiles** . 
  
## <a name="requirements"></a>Requirements

O Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

