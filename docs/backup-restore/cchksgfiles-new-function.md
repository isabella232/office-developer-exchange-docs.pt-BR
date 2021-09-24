---
title: Função CChkSGFiles.New
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- New
api_type:
- dllExport
ms.assetid: 588d8c74-c9ce-4d5e-8a79-a2a68676e858
description: 'Última modificação: 22 de fevereiro de 2013'
ms.openlocfilehash: e50b41e761b8e46d778011b6bac3db4dbb624809
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516269"
---
# <a name="cchksgfilesnew-function"></a>Função CChkSGFiles.New

**Aplica-se a: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Cria uma nova instância da **classe CChkSGFiles.** Você deve chamar essa função antes de especificar o grupo de armazenamento e os bancos de dados a serem verificados. 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a>Parâmetros

Nenhum.
  
## <a name="return-value"></a>Valor retornado

Uma referência (ponteiro) ao objeto recém-criado.
  
## <a name="remarks"></a>Comentários

A **função New** cria um objeto **CCheckSGFiles** e retorna ao chamador uma referência (ponteiro) para esse objeto. Você deve chamar essa função antes que ela chame qualquer uma das outras funções na **classe CCheckSGFiles.** 
  
Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você deve chamar a função **New** na parte de thread único do aplicativo e pode chamá-la apenas uma vez para cada **objeto CCheckSGFiles.** 
  
## <a name="requirements"></a>Requisitos

Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta em que o aplicativo está sendo executado deve ter permissões de acesso de leitura para o banco de dados e arquivos de log que devem ser verificados.
  

