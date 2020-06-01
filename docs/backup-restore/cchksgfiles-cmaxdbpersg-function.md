---
title: Função função cchksgfiles. CMaxDbPerSG
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
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: b7c3517779eb07ef053c1dd4fa25544310fb3343
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455258"
---
# <a name="cchksgfilescmaxdbpersg-function"></a>Função função cchksgfiles. CMaxDbPerSG

**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Retorna o número máximo de bancos de dados permitidos em um único grupo de armazenamento do Exchange Server.
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a>Parâmetros

Nenhum.
  
## <a name="return-value"></a>Valor retornado

O número máximo de bancos de dados que o servidor do Exchange especificado permite por grupo de armazenamento. Como os grupos de armazenamento não fazem parte do Exchange 2013, essa função retorna 1.
  
## <a name="remarks"></a>Comentários

Você pode usar o objeto **CCheckSGFiles** para validar bancos de dados (e arquivos de log de transações) em apenas um grupo de armazenamento, portanto, o valor retornado pela função **CMaxDbPerSG** também representa o número máximo de bancos de dados que você pode verificar usando uma instância da classe **CCheckSGFiles** . 
  
Observe que, por padrão, o Exchange Server 2003 e o Exchange Server 2007 permitem um máximo de cinco bancos de dados por grupo de armazenamento.
  
## <a name="requirements"></a>Requirements

O Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

