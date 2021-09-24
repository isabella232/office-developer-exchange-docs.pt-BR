---
title: Função CChkSGFiles.Delete
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Delete
api_type:
- dllExport
ms.assetid: 869e927f-7df2-4247-88ef-b8b05b29a700
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: cf1c23dd75442d73dfea49e0831d0859da321a40
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510537"
---
# <a name="cchksgfilesdelete-function"></a>Função CChkSGFiles.Delete

**Aplica-se a: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Destrói uma instância existente da **classe CChkSGFiles.** Você deve chamar essa função depois que o aplicativo terminar de trabalhar com o objeto especificado. 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a>Parâmetros

### <a name="pcchecksgfiles"></a>pcchecksgfiles 
  
Parâmetro de entrada. Um ponteiro para um objeto **CCheckSGFiles** existente. Em seguida, a memória associada ao objeto será liberada. 
    
## <a name="return-value"></a>Valor retornado

Nenhum.
  
## <a name="remarks"></a>Comentários

A **função Delete** libera a memória associada ao objeto **CCheckSGFiles.** Depois de chamar **Delete,** o ponteiro passado no parâmetro  *pcchecksgfiles*  será inválido e nenhuma outra operação poderá ser executada nesse objeto. 
  
Se o aplicativo usar a **função ErrCheckDbPages,** o aplicativo deverá liberar o buffer de memória manualmente; a **função Delete** não o liberará. 
  
Se você estiver usando CHKSGFILES em um aplicativo multithreaded, deverá chamar a função **Delete** na parte de thread único do aplicativo e poderá chamá-la apenas uma vez para cada **objeto CCheckSGFiles.** 
  
## <a name="requirements"></a>Requisitos

Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta em que o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

