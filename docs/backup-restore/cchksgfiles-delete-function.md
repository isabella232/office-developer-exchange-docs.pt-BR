---
title: Função CChkSGFiles.Delete
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
description: 'Modificado pela última vez: 22 de fevereiro de 2013'
ms.openlocfilehash: 5c41007a797e5a256692b2c4bdcb3cfae82c12ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750630"
---
# <a name="cchksgfilesdelete-function"></a>Função CChkSGFiles.Delete

**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Destruir uma instância existente da classe **CChkSGFiles** . Você deve chamar essa função depois que o aplicativo tiver terminado de trabalhar com o objeto especificado. 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a>Par�metros

### <a name="pcchecksgfiles"></a>pcchecksgfiles 
  
Parâmetro de entrada. Um ponteiro para um objeto **CCheckSGFiles** existente. A memória associada ao objeto, em seguida, será liberada. 
    
## <a name="return-value"></a>Valor retornado

Nenhum.
  
## <a name="remarks"></a>Comentários

A função **Excluir** libera a memória associada ao objeto **CCheckSGFiles** . Depois de chamar **Excluir**, o ponteiro transmitido no parâmetro *pcchecksgfiles* será inválido e nenhuma outra operação pode ser executada em desse objeto. 
  
Se o aplicativo usa a função **ErrCheckDbPages** , o aplicativo deve liberar o buffer de memória manualmente; a função **Excluir** não serão liberá-la. 
  
Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você deve chamar a função **Excluir** na parte com um único segmento do aplicativo e você poderá chamá-lo apenas uma vez para cada objeto **CCheckSGFiles** . 
  
## <a name="requirements"></a>Requisitos

Exchange 2013 inclui apenas uma versão de 64 bits da API CHKSGFILES.
  
A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.
  

