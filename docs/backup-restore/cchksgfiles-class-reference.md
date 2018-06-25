---
title: Referência de classe CChkSGFiles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9347d5f6-95bb-4045-9c86-0dc0ded24fe8
description: Encontre informações de referência para a API CHKSGFILES no Exchange 2013.
ms.openlocfilehash: 583ac5e16ab60d119c3028bf81123e9f60a58ff4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750631"
---
# <a name="cchksgfiles-class-reference"></a>Referência de classe CChkSGFiles

Encontre informações de referência para a API CHKSGFILES no Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013 
  
A API CHKSGFILES permite que os aplicativos de backup e restauração verificar a integridade dos arquivos de log de transações do Exchange Server 2013 e bancos de dados programaticamente. Você pode usar essa API no backup e restaurar aplicativos que usam o serviço de cópia de sombra de Volume (VSS).
  
> [!NOTE]
> Grupos de armazenamento não estão disponíveis no Exchange 2013. Suporte para grupos de armazenamento foi removido de versões do Exchange, começando com o Exchange Server 2010. Para manter a compatibilidade com bancos de dados e os grupos de armazenamento nas versões do Exchange anteriores ao Exchange 2010, a API CHKSGFILES permite especificar grupos de armazenamento. Quando você executa CHKSGFILES em bancos de dados do Exchange 2013, você deve definir parâmetros que especificam um identificador de grupo de armazenamento como uma sequência vazia. 
  
## <a name="file-location"></a>Local do arquivo
<a name="bk_fileslocation"> </a>

A API CHKSGFILES é fornecido como parte do Exchange 2013. Você pode usar essa API em um computador que possui a função de servidor de caixa de correio instalada. 
  
Por padrão, a DLL CHKSGFILES é instalada no diretório C:\Program Files\Microsoft\Exchange\V15\Bin.
  
Exchange 2013 inclui somente uma versão de 64 bits (amd64) da API CHKSGFILES. 
  
Você pode baixar um arquivo. zip que inclui a biblioteca CHKSGFILE.lib e arquivos de cabeçalho CHKSGFILES.hxx para uso em seu aplicativo personalizado a partir do [Centro de Download da Microsoft](http://www.microsoft.com/en-us/download/details.aspx?id=36802).
  
## <a name="development-languages"></a>Idiomas de desenvolvimento
<a name="bk_developmentlanguages"> </a>

A API CHKSGFILES destina-se a uso com versões do Visual Studio, começando com o Visual Studio 2005 em C/C++ nativo. A API CHKSGFILES não é destinada para uso em código gerenciado. Embora você possa criar um assembly de interoperabilidade COM CHKSGFILES, podemos não são fornecidos um assembly de interoperabilidade COM compatíveis com o Exchange 2013.
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Função CChkSGFiles.CMaxDbPerSG](cchksgfiles-cmaxdbpersg-function.md)
    
- [Função CChkSGFiles.Delete](cchksgfiles-delete-function.md)
    
- [Enumeração CChkSGFiles.ERR](cchksgfiles-err-enumeration.md)
    
- [Função CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md)
    
- [Função CChkSGFiles.ErrCheckDbPages](cchksgfiles-errcheckdbpages-function.md)
    
- [Função CChkSGFiles.ErrCheckLogs](cchksgfiles-errchecklogs-function.md)
    
- [Função de CChkSGFiles.ErrGetHeader (reservada)](cchksgfiles-errgetheader-function-reserved.md)
    
- [Função CChkSGFiles.ErrInit](cchksgfiles-errinit-function.md)
    
- [Função CChkSGFiles.ErrTerm](cchksgfiles-errterm-function.md)
    
- [Enumeração CChkSGFiles.iDbInvalid](cchksgfiles-idbinvalid-enumeration.md)
    
- [Função CChkSGFiles.New](cchksgfiles-new-function.md)
    
- [Enumeração CChkSGFiles.NO_FLAGS](cchksgfiles-no_flags-enumeration.md)
    
- [CChkSGFiles.PAGE_INFO struct](cchksgfiles-page_info-struct.md)
    
- [Função CChkSGFiles.PgnoFromFileOffset](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a>Confira também

- [Exchange Online e o desenvolvimento do Exchange](../exchange-server-development.md)
- [Backup, restauração e recuperação de desastres](http://technet.microsoft.com/en-us/library/dd876874)
    

