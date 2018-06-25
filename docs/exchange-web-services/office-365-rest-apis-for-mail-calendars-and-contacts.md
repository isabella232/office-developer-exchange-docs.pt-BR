---
title: APIs do Office 365 REST para emails, calendários e contatos
manager: sethgros
ms.date: 4/29/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3b2e71a6-5fa5-4008-b243-d3a6e9173b3d
description: Encontre informações sobre as APIs do Office 365 que você pode usar para acessar email, calendários e contatos no Office 365 ou Exchange Online.
ms.openlocfilehash: d42d3ff0b68dfbf23d5a4eebb826a6d39a4ac116
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750943"
---
# <a name="office-365-rest-apis-for-mail-calendars-and-contacts"></a>APIs do Office 365 REST para emails, calendários e contatos

Encontre informações sobre as APIs do Office 365 que você pode usar para acessar email, calendários e contatos no Office 365 ou Exchange Online.
  
O Office 365 e o Exchange Online fornecem uma nova maneira de trabalhar com email, calendários e contatos. O email, calendário e APIs REST de contato fornecem uma maneira poderosa e fácil de usar para acessar e manipular dados do Exchange. Essas APIs são baseadas em padrões abertos: OAuth versão 2.0 para autenticação e OData versão 4.0 e JSON abstração de dados. Isso oferece as seguintes vantagens:
  
- Como essas APIs exigem OAuth para autenticação, seu aplicativo não tem que manipular ou armazenar credenciais de usuário.
    
- OAuth torna possível solicitar permissões rigorosamente com escopo para dados do usuário. Por exemplo, você pode projetar seu aplicativo para solicitação de permissão e ler apenas o calendário do usuário.
    
## <a name="work-with-email-and-mail-folders"></a>Trabalhar com pastas de email e mala

Você pode usar a [API de E-mail](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx) para obter, criar, atualizar, excluir, mover, copiar e enviar email. Você também pode obter, criar, atualizar e excluir pastas de email. 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a>Trabalhar com grupos de calendário, calendários e eventos

Você pode usar a [API de calendário](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx) para obter, criar, atualizar e excluir eventos. Você também pode obter, criar, atualizar e excluir grupos de calendário e calendários. 
  
## <a name="work-with-contacts-and-contact-folders"></a>Trabalhe com contatos e pastas de contatos

Você pode usar a [API de contatos](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx) para obter, criar, atualizar e excluir contatos na caixa de correio do usuário. Você também pode obter pastas de contatos. 
  
## <a name="work-with-file-providers"></a>Trabalhar com provedores de arquivo

Você pode usar a [API REST do arquivo provedores](http://msdn.microsoft.com/library/8bab5403-de68-4b49-ab19-9a6470f2a2ce%28Office.15%29.aspx) para obter, criar, atualizar e excluir informações sobre provedores de arquivos suportados, como caixa de correio, pasta de recados e assim por diante. 
  
## <a name="next-steps"></a>Próximas etapas

Vá direto para a página de [desenvolvimento na plataforma do Office 365](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx) para obter mais informações sobre o email, calendário e APIs de contatos, incluindo diretrizes para configurar o seu ambiente e o guia de Introdução com as APIs. Certifique-se também fazer check-out de [projetos de início e códigos de exemplo](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx) para ver essas APIs em ação. 
  
## <a name="see-also"></a>Confira também


- [Como desenvolver na plataforma do Office 365](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx)
    
- [Como criar um aplicativo ASP.NET MVC no Office 365](http://msdn.microsoft.com/office/office365/howto/Build-your-first-ASPNET-MVC-app%28Office.15%29.aspx)
    
- [Operações REST de email](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx)
    
- [Operações REST do calendário](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx)
    
- [Operações REST de contatos](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx)
    
- [Exemplos de código e projetos iniciais de APIs do Office 365](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx)
    

