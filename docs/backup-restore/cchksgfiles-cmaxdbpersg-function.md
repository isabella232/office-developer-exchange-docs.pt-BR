---
title: Função CChkSGFiles.CMaxDbPerSG
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CMaxDbPerSG
api_type:
- dllExport
ms.assetid: 5871988b-a5d7-42cc-9b83-8fededb5072f
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: 1a82e71afde4766734d0875f68d7932a9fd9f26a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510521"
---
# <a name="cchksgfilescmaxdbpersg-function"></a>Função CChkSGFiles.CMaxDbPerSG

**Aplica-se a: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Retorna o número máximo de bancos de dados permitidos em um único Exchange de armazenamento de servidores.
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a>Parâmetros

Nenhum.
  
## <a name="return-value"></a>Valor retornado

O número máximo de bancos de dados que o servidor Exchange especificado permite por grupo de armazenamento. Como os grupos de armazenamento não fazem parte Exchange 2013, essa função retorna 1.
  
## <a name="remarks"></a>Comentários

Você pode usar o objeto **CCheckSGFiles** para validar bancos de dados (e arquivos de log de transações) em apenas um grupo de armazenamento, portanto, o valor retornado pela **função CMaxDbPerSG** também representa o número máximo de bancos de dados que você pode verificar usando uma instância da **classe CCheckSGFiles.** 
  
Observe que, por padrão, Exchange Server 2003 e Exchange Server 2007 permitem no máximo cinco bancos de dados por grupo de armazenamento.
  
## <a name="requirements"></a>Requisitos

Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta em que o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

