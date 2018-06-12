---
title: Aplicativos do EWS e arquitetura do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c10f308a-65bb-4a0b-8fdd-b4a61503f0fd
description: Saiba mais sobre o funcionamento do EWS dentro da arquitetura do Exchange e descubra quais protocolos depende do EWS.
ms.openlocfilehash: 1fbc1e68edbca829555fbbf1b9f0bc4723da9524
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750669"
---
# <a name="ews-applications-and-the-exchange-architecture"></a>Aplicativos do EWS e arquitetura do Exchange

Saiba mais sobre o funcionamento do EWS dentro da arquitetura do Exchange e descubra quais protocolos depende do EWS.
  
Serviços Web do Exchange (EWS) é uma API de plataforma cruzada que permite aos aplicativos acessar itens de caixa de correio, como mensagens de email, reuniões e contatos do Exchange Online, Exchange Online como parte do Office 365, ou versões do Exchange começando com local Exchange Server 2007. [Aplicativos do EWS](ews-application-types.md) podem acessar os itens de caixa de correio local ou remotamente enviando uma solicitação em uma mensagem SOAP com base em XML. A mensagem SOAP está incorporada em uma mensagem de HTTP enviadas entre o aplicativo e servidor, o que significa que seu aplicativo pode postar XML via HTTP, desde que ela pode usar o EWS para acessar o Exchange. 
  
## <a name="exchange-architecture-overview"></a>Visão geral da arquitetura do Exchange
<a name="bk_techarch"> </a>

Os diagramas a seguir mostram os métodos de autenticação e os caminhos de comunicação usados pelos aplicativos do EWS durante a comunicação com o Exchange 2013 e Exchange Online. Da perspectiva de aplicativos do EWS, os caminhos de comunicação são idênticos e os métodos de autenticação apenas variam; a principal diferença é que a visibilidade que você tem o back-end do Exchange.
  
**Figura 1. Aplicativos do EWS e a arquitetura do Exchange local**

![Uma ilustração que mostra um aplicativo EWS no contexto de arquitetura local do Exchange. Para obter uma descrição dos componentes do diagrama, consulte os itens 1-8 no texto que segue esta e a próxima imagem.](media/Ex2013_ArchitecturesOverview.png)
  
A Figura 2 mostra os mesmos caminhos de comunicação mostrados na Figura 1, conforme usado pelos aplicativos do EWS durante a comunicação com o Exchange Online.
  
**Figura 2. Aplicativos do EWS e a arquitetura do Exchange Online**

![Uma ilustração que mostra um aplicativo EWS no contexto de arquitetura do Exchange Online para um aplicativo EWS. Para obter uma descrição dos componentes do diagrama, consulte os itens 1, 2, 3, 6 e 9 no texto que segue a imagem.](media/Ex2013_Architectures_Online.png)
  
Estes são os componentes que são mostrados nos diagramas a:
  
1. Aplicativos do EWS — isso pode ser um [cliente, o portal ou o aplicativo de serviço](ews-application-types.md) e pode ser instalado em um cliente ou em um servidor de acesso para cliente do Exchange local. Se você usar a API gerenciada de EWS para desenvolver o aplicativo do EWS, os assemblies de API gerenciada de EWS precisam ser instalado no cliente e [redistribuídos pelo seu aplicativo](redistribution-requirements-for-the-ews-managed-api.md).
    
2. A mensagem SOAP XML — mensagem An XML, em um envelope SOAP, incorporado em uma mensagem HTTP/S que está em conformidade com o arquivo Services.wsdl no servidor de acesso para cliente. HTTPS é recomendado para o Exchange local e é necessário para o Exchange Online. 
    
3. Métodos de autenticação — mensagens EWS incluem básica, as informações de autenticação NTLM (autenticação integrada do Windows) ou OAuth como parte da carga do HTTP. 
    
4. Balanceador de carga — o balanceador de carga distribui a mensagem para um servidor de acesso para cliente pela matriz de servidores de acesso para cliente. Esse componente só estará visível na arquitetura de local do Exchange.
    
5. Matriz de servidores de acesso do cliente — servidores de acesso para cliente são organizados em um grupo com balanceamento de carga chamado uma matriz de servidores de acesso para cliente. Servidores de acesso para cliente individuais fornecem autenticação, limitado de redirecionamento e proxy serviços. Os próprios servidores de acesso para cliente não fazem qualquer processamento de dados e nenhum dado é colocada em fila ou armazenado em um servidor de acesso para cliente - é fina e estado; ele simplesmente autentica a solicitação, executa uma pesquisa de descoberta automática e, em seguida, proxies a solicitação para o servidor de caixa de correio. O servidor de acesso para cliente manter uma relação de 1:1 com o servidor de caixa de correio que hospeda os dados do usuário. O protocolo HTTP (protegido por meio de SSL usando um certificado autoassinado) é usado entre o servidor de acesso para cliente e o servidor de caixa de correio. Esse componente só estará visível na arquitetura de local do Exchange.
    
6. Serviço de descoberta automática — serviço de descoberta automática a executa uma descoberta de serviço acessando os serviços de domínio Active Directory (AD DS) para recuperar a versão de caixa de correio e o local do servidor de caixa de correio que está hospedando a cópia ativa dos dados do usuário.
    
7. Serviço EWS — serviço o EWS é descrito por três arquivos: Services.wsdl, Messages.xsd e Types.xsd, bem como os assemblies de API gerenciada de EWS. Services.WSDL descreve o contrato entre o cliente e servidor, Messages.xsd define as mensagens de solicitação e resposta SOAP e Types.xsd define os elementos usados nas mensagens SOAP. Messages.xsd e Types.xsd sempre contenham as versões mais recentes do esquema, embora existam de versões anteriores do esquema. Observe que Services.wsdl, Messages.xsd e Types.xsd são disponibilizados no servidor de acesso para cliente, mas não são usados para a validação de esquema realmente — eles são fornecidos apenas para referência. Os assemblies de API gerenciada de EWS são fornecidos para aplicativos de cliente do EWS do servidor e são implantados em todas as funções do Exchange Server, não apenas os servidores de acesso para cliente. Esse componente só estará visível na arquitetura de local do Exchange.
    
    Disponibilidade de recurso baseia-se na versão do esquema de EWS que suas metas de aplicativo. Como os esquemas EWS são e encaminhar-compatível, se você criar um aplicativo que tem como destino uma versão anterior do esquema, como o Exchange 2007 SP1, seu aplicativo também funcionará em relação a uma versão posterior do esquema, como o serviço do Exchange 2010 SP2, bem como Exchange Online. Porque os recursos e as atualizações de recurso são acionadas pelo esquema, recomendamos que você use a base de código comum primeira voltado para os recursos do EWS que você deseja implementar no seu aplicativo cliente. Muitos aplicativos podem direcionar a versão Exchange2007_SP1, porque o esquema do Exchange 2007 SP1 contém quase todas a funcionalidade básica do Exchange para trabalhar com itens e pastas do Exchange Store. Para obter mais informações, consulte [recursos do cliente EWS](ews-client-design-overview-for-exchange.md#EWSFeatures).
    
8. Grupo de disponibilidade de banco de dados (DAG) — Servidores de caixa de correio são organizados em um DAG altamente disponível, que pode ser implantado em um ou mais centros de dados. O servidor de caixa de correio contém o banco de dados de caixa de correio e lida com todas as atividades para as caixas de correio ativas no servidor. Todos os componentes que processam, renderizam e armazenam os dados estão no servidor de caixa de correio. Os clientes não são conectadas diretamente ao servidor de caixa de correio; todas as conexões são manipuladas pelo servidor de acesso para cliente. Esse componente só estará visível na arquitetura de local do Exchange.
    
9. O Exchange Online e o Exchange Online como parte do Office 365 — a solução de mensagens hospedada que fornece recursos do Exchange como um serviço baseado em nuvem.
    
Quando uma aplicativo da EWS solicitar informações do armazenamento do Exchange, uma mensagem de solicitação XML em conformidade com o SOAP padrão é criada e enviada ao servidor do Exchange. Quando o Exchange server recebe a solicitação, ele verifica as credenciais que são fornecidas pelo cliente e analisa automaticamente o XML para os dados solicitados. O servidor, em seguida, cria uma resposta SOAP que contém os dados XML que representa os objetos fortemente tipados solicitados e suas propriedades. Os dados XML serão enviados para o aplicativo em uma resposta HTTP. Em seguida, o aplicativo desserializa o XML e usa os dados para os objetos fortemente tipados a reforma.
  
## <a name="protocols-and-standards-that-ews-applications-must-support"></a>Protocolos e padrões que devem oferecer suporte a aplicativos de EWS
<a name="bk_standards"> </a>

Para se comunicar com um servidor Exchange, aplicativos de EWS devem suportar os seguintes protocolos e padrões.
  
**Tabela 1. Protocolos**

|**Protocolo**|**Como ele é usado**|
|:-----|:-----|
|HTTP/S  <br/> |Permite que aplicativos de EWS acessar o banco de dados do Exchange na rede, independentemente se o cliente está na Internet ou intranet.  <br/> |
|SOAP 1.0  <br/> |Um envelope ao redor da carga de mensagens de formulários. EWS implementa o protocolo SOAP com o uso de diferentes partes do envelope SOAP para habilitar a funcionalidade de diferente. O cabeçalho SOAP é usado para representação e fornecer dados de controle de versão. O corpo SOAP fornece informações sobre a operação a ser executada e os dados que serão enviados para a operação. Depende do SOAP WSDL para descrever as operações para chamar.  <br/> |
|WSDL 1.0  <br/> |Descreve as propriedades que são usadas para chamar operações EWS, no arquivo Services.wsdl, as operações e as associações. Esse arquivo, junto com os arquivos de esquema referenciado, compreende o contrato entre um aplicativo do EWS e Exchange server e é frequentemente usado juntamente com as ferramentas específicas de fornecedor para criar aplicativos específicos de plataforma. O arquivo WSDL está localizado no diretório virtual EWS, que está na raiz do site.  <br/> |
|Transport Layer Security (TLS) / SSL  <br/> |Fornece comunicações seguras na web na Internet ou na intranet. O TLS permite que os aplicativos autenticar servidores ou, opcionalmente, para autenticar os aplicativos do EWS. Ele também fornece um canal de segurança ao criptografar as comunicações. O TLS é a versão mais recente do protocolo Secure Sockets Layer (SSL).  <br/> |
|XSD/XML  <br/> |Fornece um formato de mensagem universal para a troca de informações entre o Exchange server e o cliente. XML fornece dados de banco de dados do Exchange complexos para aplicativos clientes, mas em uma estrutura definida. A vantagem do XML é que ele permite que o intercâmbio de dados para o mesmo quando um aplicativo do EWS e o servidor não compartilharem uma plataforma comum.  <br/> |
   
Além disso, os aplicativos do EWS devem suportar os padrões de autenticação a seguir:
  
- Autenticação básica sobre SSL, para aplicativos que visam o Exchange Online ou Exchange local.
    
- Autenticação NTLM sobre SSL, para aplicativos que suportam o Exchange local.
    
- OAuth 2.0 autenticação de token, para aplicativos de parceiros confiáveis e interoperabilidade com o Lync Server 2013 e SharePoint Server 2013.
    
## <a name="see-also"></a>Confira também


- [Start using web services in Exchange](start-using-web-services-in-exchange.md)
    
- [Tipos de aplicativos do EWS](ews-application-types.md)
    
- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md)
    

