---
title: Função função cchksgfiles. New
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- New
api_type:
- dllExport
ms.assetid: 588d8c74-c9ce-4d5e-8a79-a2a68676e858
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: d18d3ef20890012a1d8c193ec87bdca10a1ed451
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455230"
---
# <a name="cchksgfilesnew-function"></a>Função função cchksgfiles. New

**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Cria uma nova instância da classe **função cchksgfiles** . Você deve chamar essa função antes de poder especificar o grupo de armazenamento e os bancos de dados a serem verificados. 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a>Parâmetros

Nenhum.
  
## <a name="return-value"></a>Valor retornado

Uma referência (ponteiro) para o objeto recém-criado.
  
## <a name="remarks"></a>Comentários

A **nova** função cria um objeto **CCheckSGFiles** e retorna ao chamador uma referência (ponteiro) para esse objeto. Você deve chamar essa função antes de chamar qualquer uma das outras funções na classe **CCheckSGFiles** . 
  
Se você estiver usando o CHKSGFILES em um aplicativo multi-threaded, deverá chamar a **nova** função na parte de thread único do aplicativo, e poderá chamá-la somente uma vez para cada objeto **CCheckSGFiles** . 
  
## <a name="requirements"></a>Requirements

O Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta sob a qual o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

