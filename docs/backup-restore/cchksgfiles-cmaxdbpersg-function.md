---
title: Função CChkSGFiles.CMaxDbPerSG
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CMaxDbPerSG
api_type:
- dllExport
ms.assetid: 5871988b-a5d7-42cc-9b83-8fededb5072f
description: 'Modificado pela última vez: 22 de fevereiro de 2013'
ms.openlocfilehash: bf09074bab6dee13e97e8a59a22ae1b19522a5e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751592"
---
# <a name="cchksgfilescmaxdbpersg-function"></a>Função CChkSGFiles.CMaxDbPerSG

**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Retorna o número máximo de bancos de dados permitidos em um único grupo de armazenamento do Exchange server.
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a>Parâmetros

Nenhum.
  
## <a name="return-value"></a>Valor retornado

O número máximo de bancos de dados que permite que o servidor Exchange especificado por grupo de armazenamento. Como os grupos de armazenamento não fazem parte do Exchange 2013, essa função retornará 1.
  
## <a name="remarks"></a>Comentários

Você pode usar o objeto **CCheckSGFiles** para validar os bancos de dados (e os arquivos de log de transação) em apenas um grupo de armazenamento e, portanto, o valor retornado pela função **CMaxDbPerSG** também representa o número máximo de bancos de dados que você pode verificar usando um instância da classe **CCheckSGFiles** . 
  
Observe que por padrão, o Exchange Server 2003 e Exchange Server 2007 permite que um máximo de cinco bancos de dados por grupo de armazenamento.
  
## <a name="requirements"></a>Requisitos

Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.
  

