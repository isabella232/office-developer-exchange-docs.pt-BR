---
title: Função CChkSGFiles.New
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
description: 'Modificado pela última vez: 22 de fevereiro de 2013'
ms.openlocfilehash: b40f8b1a95477715b29defb4addabfb333e92d04
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750624"
---
# <a name="cchksgfilesnew-function"></a>Função CChkSGFiles.New

**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Cria uma nova instância da classe **CChkSGFiles** . Você deve chamar essa função antes de especificar o grupo de armazenamento e bancos de dados a ser verificado. 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a>Parâmetros

Nenhum.
  
## <a name="return-value"></a>Valor retornado

Uma referência (ponteiro) para o objeto recém-criado.
  
## <a name="remarks"></a>Coment�rios

A função **New** cria um objeto **CCheckSGFiles** e retorna ao chamador uma referência (ponteiro) para esse objeto. Antes de chamar qualquer uma das outras funções na classe **CCheckSGFiles** , você deve chamar essa função. 
  
Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você deve chamar a função **New** na parte com um único segmento do aplicativo e você poderá chamá-lo apenas uma vez para cada objeto **CCheckSGFiles** . 
  
## <a name="requirements"></a>Requisitos

Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.
  

