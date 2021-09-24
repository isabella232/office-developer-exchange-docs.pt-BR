---
title: Backup e restauração para o Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 329902d9-0ecb-4cfb-86dd-5ce863deff3f
description: Encontre informações sobre como criar aplicativos de backup e restauração para Exchange 2013.
ms.openlocfilehash: 2be8295985651319860ab2d2a143d69f663bf932
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514897"
---
# <a name="backup-and-restore-for-exchange"></a>Backup e restauração para o Exchange
  
Exchange Server 2013 fornece DAGs (Grupos de Disponibilidade de Banco de Dados), que ajudam a manter os dados armazenados seguros e disponíveis e reduzir a necessidade de aplicativos personalizados de backup e restauração. Os DAGs habilitam a redundância de dados fora do site para ajudar a garantir que você não perca dados. No entanto, muitos planos de recuperação de desastres continuam a incluir métodos e sistemas de backup e restauração mais tradicionais, incluindo aplicativos personalizados, para redundância com o DAG. Para ajudar a garantir a disponibilidade e a redundância de dados em sua organização, você pode criar aplicativos personalizados que usam tecnologias de sistema operacional Exchange Server e Windows Server para fazer backup e restaurar seus dados Exchange de segurança.

<a name="bk_plugin"> </a>

## <a name="backup-technologies-in-exchange-2013"></a>Tecnologias de backup Exchange 2013

Exchange 2013 inclui um plug-in para o backup do Windows Server que os administradores podem usar para fazer backups baseados em VSS de dados Exchange. Os administradores também podem usar Windows Backup do Servidor para fazer backup e restaurar Exchange bancos de dados. Se você estiver criando um aplicativo de backup e restauração para o Exchange 2013, precisará criar um aplicativo com conhecimento de Exchange que suporte o escritor VSS para o Exchange 2013 e usar a API CHKSGFILES para validar a consistência desse backup. Para obter mais informações, consulte [Validate backup integrity by using the CHKSGFILES API in Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md).

<a name="bk_vsswriter"> </a>

## <a name="vss-writer-in-exchange-2013"></a>Escritor VSS no Exchange 2013

Exchange 2013 introduz uma mudança significativa na arquitetura de escritor VSS no Exchange Server 2010 e Exchange Server 2007. Exchange 2010 e Exchange 2007 incluem dois escritores VSS: um dentro do serviço de Armazenamento de Informações do Exchange (store.exe) e um dentro do serviço Exchange Replication (msexchangerepl.exe). No Exchange 2013, a funcionalidade de escritor VSS está localizada no serviço Exchange Replication. Seu aplicativo de backup e restauração usa o novo escritor VSS, chamado de Escritor do Microsoft Exchange, para fazer backup de cópias de banco de dados ativas e passivas e para restaurar cópias de banco de dados com backup. Embora o novo escritor VSS seja executado no serviço Exchange replicação, o serviço Exchange Armazenamento de Informações deve estar sendo executado para que o escritor seja disponibilizado. Com isso, ambos os serviços são necessários para o backup ou a restauração de bancos de dados do Exchange.
  
Embora a arquitetura de escritor VSS tenha sido atualizada Exchange 2013, a funcionalidade subjacente não foi alterada. Se você criou um aplicativo de backup e restauração para o Exchange 2010, não será necessário fazer alterações no aplicativo para o Exchange 2013. Certifique-se de recompilar seu aplicativo com os arquivos mais recentes para garantir a compatibilidade. Para aplicativos de backup e restauração criados para Exchange 2007 ou versões anteriores, você precisará reescrever seu código para usar a API CHKSGFILES mais recente.
  
## <a name="what-you-need-to-know-about-vss-backup-and-restore"></a>O que você precisa saber sobre backup e restauração do VSS

|Se você estiver se perguntando sobre...|Leia isto|
|:-----|:-----|
|Arquiteturas de aplicativos  <br/> |Aplicativos de backup e restauração que usam VSS para fazer backup de bancos de dados Exchange geralmente consistem em um serviço em segundo plano que executa o backup, um serviço de agendamento e um console de aplicativo gui Windows que controla e configura o sistema de backup e restauração.  <br/> |
|Uso remoto  <br/> |Os aplicativos que usam VSS para fazer o Exchange servidores devem ser executados no computador Windows Server 2008 no qual o processo de armazenamento Exchange está sendo executado. Devido à flexibilidade em sistemas de armazenamento grandes, o hardware que hospeda os volumes de armazenamento pode não fazer parte fisicamente do computador que executa o Windows Server 2008.  <br/> |
|Ferramentas e idiomas  <br/> |Você pode usar qualquer idioma compatível com COM para usar VSS. Ele é usado com mais frequência em aplicativos escritos em C++. Como você precisa levar o armazenamento Exchange offline para criar cópias de sombra, os aplicativos de backup geralmente são sensíveis ao tempo, o que, na maioria dos casos, torna o uso de idiomas como Visual Basic ou VBScript impraticável.  <br/> |
|Implementação gerenciada  <br/> |Você pode usar as APIs VSS em um ambiente de código gerenciado por meio de um Assembly de Interop COM.  <br/> |
|Programável  <br/> |Sim, mas não recomendado.  <br/> |
|Ferramentas de teste e depuração disponíveis  <br/> |Nenhuma ferramenta especial é necessária para depurar aplicativos que usam a Windows VSS.  <br/> |
   
## <a name="in-this-section"></a>Nesta seção

- [Conceitos de backup e restauração para Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Criar aplicativos de backup e restauração para Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Referência da classe CChkSGFiles](cchksgfiles-class-reference.md)
    
## <a name="see-also"></a>Confira também

- [Serviço de Cópia de Sombra de Volume (Windows)](https://msdn.microsoft.com/library/windows/desktop/bb968832%28v=vs.85%29.aspx)   
- [Explorar os recursos da API gerenciada por EWS, EWS e Serviços Web no Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [Exchange Management Shell](../management/exchange-management-shell.md)   
- [Agentes de transporte no Exchange](../transport-agents/transport-agents-in-exchange-2013.md) 
    

