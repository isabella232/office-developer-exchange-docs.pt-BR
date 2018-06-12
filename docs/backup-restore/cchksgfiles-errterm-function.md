---
title: Função CChkSGFiles.ErrTerm
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrTerm
api_type:
- dllExport
ms.assetid: eea20a55-4a2a-4209-ae79-dc1ee1cd631b
description: 'Última modificação: 25 de fevereiro de 2013'
ms.openlocfilehash: 099ec33663baa2414a0c28b90364523b6191c697
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750634"
---
# <a name="cchksgfileserrterm-function"></a>Função CChkSGFiles.ErrTerm
  
**Aplica-se a:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Fornece um status geral da verificação de banco de dados e log, que indica se todas as páginas de banco de dados e logs foram verificados com êxito.
  
> [!IMPORTANT]
> Grupos de armazenamento não estão disponíveis no Exchange 2013. Para manter a compatibilidade com bancos de dados e os grupos de armazenamento nas versões do Exchange anteriores ao Exchange Server 2010, a API CHKSGFILES permite especificar grupos de armazenamento. Quando você executa CHKSGFILES em bancos de dados do Exchange 2013, você deve definir parâmetros que especificam um identificador de grupo de armazenamento como uma sequência vazia. 
  
```cs
Vitual ERRErrTerm 
(
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Par�metros

### <a name="ulflags"></a>ulFlags
  
Parâmetro de entrada opcional. Esse valor é reservado para uso futuro. O valor passado por este parâmetro deve ser de 0 (zero).
    
## <a name="return-value"></a>Valor retornado

Um código de erro da enumeração [ERR](cchksgfiles-err-enumeration.md) . 
  
## <a name="remarks"></a>Coment�rios

O objeto **CChkSGFiles** determina se todos os bancos de dados registrados com a função **ErrInit** realmente marcados. Este objeto usa a função **ErrCheckDbPages** para verificar se o mesmo número de páginas identificadas pela função **ErrCheckDbHeaders** realmente foram verificadas de banco de dados. Se o número correto das páginas em cada banco de dados não forem verificado com êxito, a função de **ErrTerm** retornará um erro. 
  
Se o número de páginas de banco de dados verificado com **ErrCheckDbPages** for menor do que indicado pelo **ErrCheckDbHeaders**, essa função cria um erro no log de eventos do Windows e **ErrTerm** retornará um erro. 
  
Se o número de páginas de banco de dados verificado com **ErrCheckDbPages** for maior do que o indicado pelo **ErrCheckDbHeaders**, essa função cria um aviso no log de eventos do Windows para indicar que o aplicativo pode ser desnecessariamente verificando alguns páginas de banco de dados mais de uma vez. Nesse caso, entretanto, a função **ErrTerm** for bem-sucedido. 
  
O objeto **CChkSGFiles** também determina se os arquivos de log registrados com **ErrInit** realmente marcados. Se não todos os logs foram verificadas com êxito, a função **ErrTerm** retornará um erro. 
  
Quando **ErrTerm** retornará um erro, será o primeiro erro encontrar, mesmo que ele verifica o status de verificação para todos os bancos de dados registrados com **ErrInit**.
  
Se você estiver usando CHKSGFILES em um aplicativo multithreaded, você deve chamar a função **ErrTerm** na parte com um único segmento do aplicativo e você poderá chamá-lo sem com mais de uma vez para cada objeto **CCheckSGFiles** . 
  
## <a name="requirements"></a>Requisitos

Exchange 2013 inclui apenas uma versão de 64 bits do CHKSGFILES.
  
A conta que o aplicativo está sendo executado em deve ter permissões de acesso de leitura para os arquivos de log e de banco de dados que devem ser verificado.
  

