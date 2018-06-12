---
title: Visão geral de design de cliente do EWS do Exchange
manager: sethgros
ms.date: 3/11/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: b26f67aa-7c66-4d7d-98b3-746f26ab37f4
description: Saiba mais sobre as considerações de design para o desenvolvimento com o EWS para Exchange.
ms.openlocfilehash: ea0e1ad3f8402d19a6163f3320a2a17f08f3ea2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750663"
---
# <a name="ews-client-design-overview-for-exchange"></a>Visão geral de design de cliente do EWS do Exchange

Saiba mais sobre as considerações de design para o desenvolvimento com o EWS para Exchange. 
  
Este artigo fornece informações gerais sobre como criar um aplicativo de serviços Web do Exchange (EWS). Você pode usar essas informações para determinar se o EWS é a API correta para o seu aplicativo, e se precisar, qual tipo de implementação de cliente que você deve usar. Este artigo também fornece informações e práticas recomendadas para projetar aplicativos que podem direcionar o Office 365, Exchange Online e versões do Exchange começando com o Exchange 2007, em uma base de código e pontos de decisão importantes para direcionamento Exchange local servidores versus direcionamento Exchange Online.
  
## <a name="is-ews-the-right-api-for-your-application"></a>É o EWS a API correta para seu aplicativo?
<a name="IsEWSRight"> </a>

Antes de começar a projetar seu aplicativo, é importante considerar se o EWS é a API certa para você. Se você estiver desenvolvendo contra o Exchange Server ou o Exchange Online, o EWS é a tecnologia de acesso de cliente preferencial. Desenvolvimento do acesso de cliente para versões do Exchange, começando com o Exchange 2007 tenha sido focalizado principalmente nas EWS. Nova funcionalidade de acesso de cliente que é implementada no Outlook usa o EWS, incluindo os recursos de disponibilidade e ausência temporária escritório (OOF) introduzidos no Exchange 2007 e a funcionalidade de dicas de email e salas de obter introduzidos no Exchange 2010. Isso representa um investimento confirmado no EWS para parceiros internos e externos que desenvolvem aplicativos cliente do Exchange.
  
EWS é o acesso de cliente principal API para seus aplicativos de cliente do Exchange. No entanto, em alguns casos, você pode considerar outras APIs do Exchange para o desenvolvimento de aplicativos do cliente. Por exemplo, o Exchange ActiveSync oferece as seguintes vantagens sobre o EWS:
  
- A estrutura XML tiver sido tokenizada para tornar o Exchange ActiveSync um protocolo mais compacto.  
- Exchange ActiveSync contém um mecanismo de política para controlar o acesso do cliente e fornecer outra empresarial robusta soluções móveis de mensagens.
    
> [!NOTE]
> Você precisa de uma licença para desenvolver clientes do Exchange ActiveSync. Para saber mais sobre as diferenças entre o Exchange ActiveSync e EWS, consulte [escolher entre o Exchange ActiveSync e serviços Web do Exchange (EWS)](http://msdn.microsoft.com/en-us/library/dn144954%28v=exchg.140%29.aspx). 
  
MAPI RPC sobre HTTP é outra opção de programação de aplicativos de cliente do Exchange. No entanto, MAPI RPC sobre HTTP não fornece uma interface intuitiva para a comunicação entre clientes e o servidor.
  
Para obter mais informações sobre tecnologias de desenvolvimento do Exchange, consulte a [explorar o EWS Managed API, EWS e web services no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).
  
## <a name="options-for-ews-client-development"></a>Opções para o desenvolvimento do cliente EWS
<a name="EWSClientOptions"> </a>

Várias opções estão disponíveis para o desenvolvimento no Exchange usando o EWS. A melhor opção para você dependerá a plataforma de desenvolvimento, ferramentas, implementações disponíveis e os requisitos de aplicativos para sua organização. A seguir estão as quatro opções principais que estão disponíveis para criação de aplicativos de cliente do EWS:
  
- A API gerenciada do EWS
- A API Java EWS
- Os proxies do EWS gerada automaticamente
- Um cliente personalizado do EWS API
    
### <a name="ews-managed-api"></a>API Gerenciada do EWS

A [API gerenciada de EWS](http://aka.ms/ews-managed-api-readme) é um cliente de serviços web personalizados. É a API de acesso de cliente padrão para aplicativos do .NET Framework. 
  
Estes são alguns dos benefícios do uso da API gerenciada de EWS:
  
- Ele fornece um modelo de objeto intuitivo.   
- Ele abstrai a complexidade da descrição do serviço nos arquivos de esquema e WSDL.   
- Inclui a lógica de negócios do cliente.   
- Ele lida com as solicitações da web e a respostas e a serialização de objeto e a desserialização.   
- É com suporte da Microsoft.
    
No entanto, observe que a API gerenciada de EWS não é uma solução completa. Algumas funcionalidades podem não foi implementada o EWS Managed API. Embora a API gerenciada de EWS não implementa todas as funcionalidades do EWS, talvez seja a melhor escolha para o desenvolvimento de aplicativos do cliente, pelos seguintes motivos:
  
- Você pode usar o .NET Framework para desenvolvimento.
- Ele implementa a descoberta automática, além da maioria das partes do modelo de objeto do EWS.
- Ele implementa a lógica de negócios do cliente para trabalhar com o EWS, na classe [ExchangeService](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) . 
    
Você pode optar por usar a API do serviço web EWS, em vez do EWS Managed API para qualquer um dos seguintes motivos:
  
- Seu aplicativo não usa o .NET Framework. 
- Você não quer distribuir o assembly do EWS Managed API. 
- Seu aplicativo usa os recursos que não são implementados na API gerenciada do EWS.
    
Para saber mais, consulte [Introdução ao aplicativos cliente do EWS Managed API](get-started-with-ews-managed-api-client-applications.md).
  
> [!NOTE]
> A API gerenciada de EWS agora está disponível como um projeto de código aberto no [GitHub](http://aka.ms/ews-managed-api-github). Você pode usar a biblioteca de código aberto: 
> - Contribui com correções de bug e melhorias à API. 
> - Obtenha correções e melhorias antes que estejam disponíveis em uma versão oficial.
> - Acesse a implementação mais abrangente e atualizada da API, para usar como referência ou criar novas bibliotecas em novas plataformas. 
> 
> Agradecemos suas [contribuições](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub. 
  
### <a name="ews-java-api"></a>EWS Java API

A API Java EWS é um projeto de código aberto no [GitHub](https://github.com/OfficeDev/ews-java-api) que podem ser atualizadas e estendido pela comunidade. Ele é stylistically semelhante à [API gerenciada de EWS](http://msdn.microsoft.com/en-us/library/office/jj220535%28v=exchg.80%29.aspx) e usa o EWS SOAP solicitações e respostas durante a transmissão. Embora você não puder acessar todas as [operações do EWS SOAP](http://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) , usando a API Java EWS, com a [criação de recente](http://blogs.office.com/2014/08/28/open-sourcing-exchange-web-services-ews-java-api/) do projeto Abrir fonte, estamos observando na comunidade preencher essa lacuna. Observe que Microsoft Support, com um contrato de suporte apropriado, abordará perguntas relacionadas ao protocolo SOAP EWS, mas não a API Java EWS em si. A API Java EWS está disponível para download e comunidade contribuição no [GitHub](https://github.com/OfficeDev/ews-java-api).
  
### <a name="ews-autogenerated-proxies"></a>Proxies do EWS gerada automaticamente

APIs do cliente gerada automaticamente são geradas a partir do EWS WSDL e definições de esquema XML. Geradores de modelo de objeto do cliente estão disponíveis para vários idiomas. Em geral, os modelos de objeto gerada automaticamente gerenciam objeto serialização e desserialização. Eles não incluir lógica de negócios e o processo de geração automática frequentemente cria artefatos que tornam o modelo de objeto menos intuitivo usar. Suporte do Exchange abrange o XML que é enviado e recebido pelo cliente, mas não o modelo de objeto.
  
### <a name="custom-ews-client-api"></a>Sinalizador de API do cliente EWS

Para alguns aplicativos que usam um pequeno conjunto de funcionalidades EWS, você pode criar um cliente personalizado API para se comunicar com o Exchange. Isso permite que você consumir menos recursos do sistema. Isso é útil para clientes que executam em dispositivos com restrição de memória, como clientes executando o Micro do .NET Framework.
  
## <a name="ews-client-features"></a>Recursos do cliente EWS
<a name="EWSFeatures"> </a>

Independentemente da opção de desenvolvimento que você escolher, considere como os recursos do EWS são implementados no seu cliente. Disponibilidade de recurso baseia-se na versão do esquema de EWS que suas metas de aplicativo. Como os esquemas EWS são e encaminhar-compatível, se você criar um aplicativo que se destina a uma versão anterior do esquema, como o Exchange Server 2007 SP1, seu aplicativo também funcionará em relação a uma versão posterior do esquema, como o Exchange Server 2013 SP1 serviço, bem como o Exchange Online. 
  
Porque os recursos e as atualizações de recurso são acionadas pelo esquema, recomendamos que você use a base de código comum primeira voltado para os recursos do EWS que você deseja implementar no seu aplicativo cliente. Muitos aplicativos podem direcionar a versão Exchange2007_SP1, porque o esquema do Exchange 2007 SP1 contém quase todas a funcionalidade básica do Exchange para trabalhar com itens e pastas do Exchange Store. Recomendamos que você mantenha bifurcações de código para cada versão de esquema do EWS. Estas são as versões de esquema que estão disponíveis no momento. 
  
```XML
  <xs:simpleType name="ExchangeVersionType">
    <xs:restriction base="xs:string">
      <xs:enumeration value="Exchange2007" />
      <xs:enumeration value="Exchange2007_SP1" />
      <xs:enumeration value="Exchange2010" />
      <xs:enumeration value="Exchange2010_SP1" />
      <xs:enumeration value="Exchange2010_SP2" />
      <xs:enumeration value="Exchange2013" />
      <xs:enumeration value="Exchange2013_SP1" />
    </xs:restriction>
  </xs:simpleType>
```

As versões de esquema são mantidas no tipo **ExchangeVersionType** simple. 
  
Para obter informações sobre os recursos que estão disponíveis em cada versão de esquema do EWS, consulte [versões de esquema do EWS no Exchange](ews-schema-versions-in-exchange.md).
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Disponibilidade de recursos do Web service API no Exchange e a API gerenciada de EWS](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)
    
- [Versões de esquema do EWS no Exchange](ews-schema-versions-in-exchange.md)
    
- [Opções de configuração para o EWS no Exchange](configuration-options-for-ews-in-exchange.md)
    
- [Comparando o Exchange Online e programação do cliente do Exchange local](comparing-exchange-online-and-exchange-on-premises-client-programming.md)
    
- [EWS limitação no Exchange](ews-throttling-in-exchange.md)
    
- [Requisitos de redistribuição para a API gerenciada de EWS](redistribution-requirements-for-the-ews-managed-api.md)
    
- [Instrumentação solicitações de clientes para o EWS e REST no Exchange](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
## <a name="see-also"></a>Confira também
 
- [Start using web services in Exchange](start-using-web-services-in-exchange.md)
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md) 
- [Tipos de aplicativos do EWS](ews-application-types.md)
    

