---
title: Visão geral do design de cliente do EWS para Exchange
manager: sethgros
ms.date: 3/11/2016
ms.audience: Developer
ms.assetid: b26f67aa-7c66-4d7d-98b3-746f26ab37f4
description: Saiba mais sobre as considerações de design para desenvolvimento com o EWS para Exchange.
localization_priority: Priority
ms.openlocfilehash: 0ac4fe1be0800008af572ebc296e004aa29d8daf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455419"
---
# <a name="ews-client-design-overview-for-exchange"></a>Visão geral do design de cliente do EWS para Exchange

Saiba mais sobre as considerações de design para desenvolvimento com o EWS para Exchange. 
  
Este artigo fornece informações gerais sobre como criar um aplicativo de serviços Web do Exchange (EWS). Você pode usar essas informações para determinar se o EWS é a API correta para seu aplicativo e, em caso afirmativo, qual tipo de implementação de cliente você deve usar. Este artigo também fornece informações de práticas recomendadas para projetar aplicativos que podem direcionar o Office 365, o Exchange Online e versões do Exchange a partir do Exchange 2007, em uma base de código e importantes pontos de decisão para direcionar servidores locais do Exchange versus direcionar o Exchange Online.
  
## <a name="is-ews-the-right-api-for-your-application"></a>O EWS é a API certa para seu aplicativo?
<a name="IsEWSRight"> </a>

Antes de começar a criar seu aplicativo, é importante considerar se o EWS é a API correta para você. Se você estiver desenvolvendo no Exchange Server ou no Exchange Online, o EWS é a tecnologia de acesso para cliente preferencial. O desenvolvimento de acesso para cliente para versões do Exchange a partir do Exchange 2007 tem o foco principalmente no EWS. A nova funcionalidade de acesso para cliente implementada no Outlook usa o EWS, incluindo os recursos de ausência temporária (OOF) e disponibilidade introduzidos no Exchange 2007, e as funcionalidades dicas de correio e obter salas introduzidas no Exchange 2010. Isso representa um investimento confirmado no EWS para parceiros internos e externos que desenvolvem aplicativos cliente do Exchange.
  
O EWS é a API de acesso para cliente principal para seus aplicativos cliente do Exchange. No entanto, em alguns casos, você pode considerar outras APIs do Exchange para o desenvolvimento de aplicativos cliente. Por exemplo, o Exchange ActiveSync oferece as seguintes vantagens sobre o EWS:
  
- A estrutura XML foi indexada para tornar o Exchange ActiveSync um protocolo mais compacto.  
- O Exchange ActiveSync contém um mecanismo de política para controlar o acesso do cliente e fornecer outras soluções de mensagens móveis corporativas robustas.
    
> [!NOTE]
> Você precisa de uma licença para desenvolver clientes do Exchange ActiveSync. Para saber mais sobre as diferenças entre o Exchange ActiveSync e o EWS, consulte [escolhendo entre Exchange ActiveSync e serviços Web do Exchange (EWS)](https://msdn.microsoft.com/library/dn144954%28v=exchg.140%29.aspx). 
  
MAPI RPC sobre HTTP é outra opção de programação para aplicativos cliente do Exchange. No entanto, MAPI RPC sobre HTTP não fornece uma interface intuitiva para comunicação entre clientes e o servidor.
  
Para obter mais informações sobre as tecnologias de desenvolvimento do Exchange, consulte [explorar a API gerenciada do EWS, EWS e serviços Web no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).
  
## <a name="options-for-ews-client-development"></a>Opções para o desenvolvimento de cliente do EWS
<a name="EWSClientOptions"> </a>

Várias opções estão disponíveis para desenvolvimento no Exchange usando o EWS. A melhor opção para você dependerá da plataforma de desenvolvimento, das ferramentas, das implementações disponíveis e dos requisitos de aplicativo para sua organização. Veja a seguir as quatro opções principais que estão disponíveis para a criação de aplicativos clientes do EWS:
  
- A API gerenciada do EWS
- A API Java do EWS
- Os proxies gerados automaticamente pelo EWS
- Uma API de cliente EWS personalizada
    
### <a name="ews-managed-api"></a>API Gerenciada do EWS

A [API gerenciada do EWS](https://aka.ms/ews-managed-api-readme) é um cliente de serviço Web personalizado. É a API de acesso para cliente padrão para aplicativos do .NET Framework. 
  
A seguir estão alguns dos benefícios de usar a API gerenciada do EWS:
  
- Ele fornece um modelo de objeto intuitivo.   
- Ele abstrai as complexidades da descrição do serviço nos arquivos WSDL e de esquema.   
- Ele inclui a lógica de negócios do lado do cliente.   
- Ele lida com as solicitações e respostas da Web e serialização e desserialização de objetos.   
- É compatível com a Microsoft.
    
No entanto, observe que a API gerenciada do EWS não é uma solução completa. Algumas funcionalidades não são implementadas na API gerenciada do EWS. Embora a API gerenciada do EWS não implemente toda a funcionalidade do EWS, ela pode ser a melhor opção para o desenvolvimento de aplicativos cliente, pelos seguintes motivos:
  
- Você pode usar o .NET Framework para desenvolvimento.
- Ele implementa a descoberta automática além da maioria das partes do modelo de objeto do EWS.
- Ele implementa a lógica de negócios do lado do cliente para trabalhar com o EWS, na classe [ExchangeService](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) . 
    
Você pode optar por usar a API do serviço Web EWS em vez da API gerenciada do EWS por qualquer um dos seguintes motivos:
  
- O aplicativo não usa o .NET Framework. 
- Você não deseja distribuir o assembly da API gerenciada do EWS. 
- Seu aplicativo usa recursos que não são implementados na API gerenciada do EWS.
    
Para saber mais, confira [introdução aos aplicativos clientes de API gerenciada do EWS](get-started-with-ews-managed-api-client-applications.md).
  
> [!NOTE]
> A API gerenciada do EWS já está disponível como um projeto de código-fonte aberto no [GitHub](https://aka.ms/ews-managed-api-github). É possível usar a biblioteca de software livre para: 
> - Contribui com correções de bug e melhorias à API. 
> - Obtenha correções e melhorias antes que estejam disponíveis em uma versão oficial.
> - Acesse a implementação mais abrangente e atualizada da API, para usar como referência ou criar novas bibliotecas em novas plataformas. 
> 
> Agradecemos suas [contribuições](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via github. 
  
### <a name="ews-java-api"></a>EWS Java API

A API Java do EWS é um projeto de código aberto no [GitHub](https://github.com/OfficeDev/ews-java-api) que pode ser atualizado e estendido pela Comunidade. É de formalmente semelhante à [API gerenciada do EWS](https://msdn.microsoft.com/library/office/jj220535%28v=exchg.80%29.aspx) e usa solicitações e respostas do EWS SOAP em relação à conexão. Embora você não possa acessar todas as [operações do EWS SOAP](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) usando a API Java do EWS, com a [criação recente](https://blogs.office.com/2014/08/28/open-sourcing-exchange-web-services-ews-java-api/) do projeto de código-fonte aberto, estamos procurando a Comunidade para preencher essa lacuna. Observe que o suporte da Microsoft, com um contrato de suporte apropriado, tratará de qualquer pergunta relacionada ao protocolo do EWS SOAP, mas não à API Java do EWS. A API Java do EWS está disponível para download e contribuição da Comunidade no [GitHub](https://github.com/OfficeDev/ews-java-api).

  
### <a name="ews-autogenerated-proxies"></a>Proxies gerados automaticamente pelo EWS

As APIs de cliente geradas automaticamente são geradas a partir das definições de esquema de WSDL e XML do EWS. Os geradores de modelos de objeto do cliente estão disponíveis para vários idiomas. Em geral, os modelos de objeto gerados automaticamente gerenciam a serialização e a desserialização de objetos. Eles não incluem a lógica de negócios, e o processo de geração automática geralmente cria artefatos que tornam o modelo de objeto menos intuitivo para usar. O suporte do Exchange cobre o XML que é enviado e recebido pelo cliente, mas não pelo modelo de objeto.
  
### <a name="custom-ews-client-api"></a>API de cliente EWS personalizada

Para alguns aplicativos que usam um pequeno conjunto de funcionalidades do EWS, você pode criar uma API de cliente personalizada para se comunicar com o Exchange. Isso permite que você consuma menos recursos do sistema. Isso é útil para clientes que são executados em dispositivos restritos à memória, como clientes que executam o .NET micro Framework.
  
## <a name="ews-client-features"></a>Recursos do cliente EWS
<a name="EWSFeatures"> </a>

Independentemente da opção de desenvolvimento escolhida, você deve considerar como os recursos do EWS são implementados no cliente. A disponibilidade de recursos é baseada na versão do esquema do EWS que seu aplicativo direciona. Como os esquemas do EWS são compatíveis com versões anteriores e posteriores, se você criar um aplicativo que tenha como destino uma versão de esquema anterior, como o Exchange Server 2007 SP1, seu aplicativo também funcionará com uma versão de esquema posterior, como o serviço do Exchange Server 2013 SP1, bem como o Exchange Online. 
  
Como recursos e atualizações de recurso são orientados pelo esquema, recomendamos que você use a base de código comum mais antiga que direciona os recursos do EWS que você deseja implementar no seu aplicativo cliente. Muitos aplicativos podem se concentrar na versão do Exchange2007_SP1, porque o esquema do Exchange 2007 SP1 contém quase todas as funcionalidades principais do Exchange para trabalhar com itens e pastas no repositório do Exchange. Recomendamos que você mantenha as bifurcações de código para cada versão do esquema do EWS. Veja a seguir as versões de esquema que estão disponíveis no momento. 
  
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

As versões do esquema são mantidas no tipo simples **ExchangeVersionType** . 
  
Para obter informações sobre os recursos disponíveis em cada versão do esquema do EWS, consulte [EWS Schema Versions in Exchange](ews-schema-versions-in-exchange.md).
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Disponibilidade de recursos da API do serviço Web no Exchange e na API gerenciada do EWS](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)   
- [Versões de esquema do EWS no Exchange](ews-schema-versions-in-exchange.md)  
- [Opções de configuração do EWS no Exchange](configuration-options-for-ews-in-exchange.md)  
- [Comparando a programação de cliente local do Exchange Online e do Exchange](comparing-exchange-online-and-exchange-on-premises-client-programming.md)   
- [Limitação do EWS no Exchange](ews-throttling-in-exchange.md)  
- [Requisitos de redistribuição para a API gerenciada do EWS](redistribution-requirements-for-the-ews-managed-api.md)  
- [Instrumentação de solicitações de cliente para EWS e REST no Exchange](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
## <a name="see-also"></a>Confira também
 
- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md) 
- [Tipos de aplicativo do EWS](ews-application-types.md)
    

