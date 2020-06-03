---
title: Aplicativos EWS e a arquitetura do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: c10f308a-65bb-4a0b-8fdd-b4a61503f0fd
description: Saiba mais sobre como o EWS funciona dentro da arquitetura do Exchange e descubra em quais protocolos o EWS se baseia.
localization_priority: Priority
ms.openlocfilehash: 15f396664ea46e53a4603a617c9bf679400af160
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456072"
---
# <a name="ews-applications-and-the-exchange-architecture"></a>Aplicativos EWS e a arquitetura do Exchange

Saiba mais sobre como o EWS funciona dentro da arquitetura do Exchange e descubra em quais protocolos o EWS se baseia.
  
O EWS (serviços Web do Exchange) é uma API de plataforma cruzada que permite que os aplicativos acessem itens de caixa de correio, como mensagens de email, reuniões e contatos do Exchange Online, do Exchange Online como parte do Office 365 ou de versões locais do Exchange a partir do Exchange Server 2007. [Os aplicativos EWS](ews-application-types.md) podem acessar itens de caixa de correio local ou remotamente enviando uma solicitação em uma mensagem XML baseada em SOAP. A mensagem SOAP é incorporada em uma mensagem HTTP quando enviada entre o aplicativo e o servidor, o que significa que, desde que o aplicativo possa postar XML através de HTTP, ele pode usar o EWS para acessar o Exchange. 
  
## <a name="exchange-architecture-overview"></a>Visão geral da arquitetura do Exchange
<a name="bk_techarch"> </a>

Os diagramas a seguir mostram os métodos de autenticação e os caminhos de comunicação usados pelos aplicativos do EWS durante a comunicação com o Exchange 2013 e o Exchange Online. Da perspectiva do aplicativo EWS, os caminhos de comunicação são idênticos e os métodos de autenticação variam apenas um pouco; a principal diferença é a visibilidade que você tem no back-end do Exchange.
  
**Figura 1. Aplicativo EWS e arquitetura local do Exchange**

![Uma ilustração que mostra um aplicativo EWS no contexto de arquitetura local do Exchange. Para obter uma descrição dos componentes do diagrama, consulte os itens 1-8 no texto que segue esta e a próxima imagem.](media/Ex2013_ArchitecturesOverview.png)
  
A Figura 2 mostra os mesmos caminhos de comunicação mostrados na Figura 1, conforme usado pelos aplicativos EWS ao se comunicar com o Exchange Online.
  
**Figura 2. Aplicativo EWS e arquitetura do Exchange Online**

![Uma ilustração que mostra um aplicativo EWS no contexto de arquitetura do Exchange Online para um aplicativo EWS. Para obter uma descrição dos componentes do diagrama, consulte os itens 1, 2, 3, 6 e 9 no texto que segue a imagem.](media/Ex2013_Architectures_Online.png)
  
Estes são os componentes mostrados nos diagramas:
  
1. Aplicativo EWS — pode ser um [cliente, portal ou aplicativo de serviço](ews-application-types.md) e que pode ser instalado em um cliente ou em um servidor de acesso para cliente local do Exchange. Se você usar a API gerenciada do EWS para desenvolver o aplicativo EWS, os assemblies da API gerenciada do EWS precisam ser instalados no cliente e [redistribuídos pelo seu aplicativo](redistribution-requirements-for-the-ews-managed-api.md).
    
2. A mensagem XML do SOAP — uma mensagem XML, em um envelope SOAP, incorporada em uma mensagem HTTP/S que está de acordo com o arquivo Services. WSDL no servidor de acesso para cliente. O HTTPS é recomendado para o Exchange local e é necessário para o Exchange Online. 
    
3. Métodos de autenticação – as mensagens do EWS incluem as informações de autenticação básica, NTLM (autenticação integrada do Windows) ou OAuth como parte da carga HTTP. 
    
4. Balanceador de carga — o balanceador de carga distribui a mensagem para um servidor de acesso para cliente na matriz de servidor de acesso para cliente. Este componente só é visível na arquitetura local do Exchange.
    
5. Matriz de servidor de acesso para cliente — os servidores de acesso para cliente são organizados em um grupo com balanceamento de carga chamado matriz de servidor de acesso para cliente. Os servidores de acesso para cliente individuais fornecem autenticação, redirecionamento limitado e serviços de proxy. Os servidores de acesso para cliente propriamente ditos não fazem renderização de dados, e nenhum dado é enfileirado ou armazenado em um servidor de acesso para cliente, ele é thin e sem estado; Ele simplesmente autentica a solicitação, realiza uma pesquisa de descoberta automática e, em seguida, faz a proxy da solicitação para o servidor de caixa de correio. O servidor de acesso para cliente mantém uma relação 1:1 com o servidor de caixa de correio que hospeda os dados do usuário. O protocolo HTTP (protegido via SSL usando um certificado autoassinado) é usado entre o servidor de acesso para cliente e o servidor de caixa de correio. Este componente só é visível na arquitetura local do Exchange.
    
6. Serviço de descoberta automática – o serviço de descoberta automática realiza uma descoberta de serviço acessando os serviços de domínio do Active Directory (AD DS) para recuperar a versão da caixa de correio e o local do servidor de caixa de correio que hospeda a cópia ativa dos dados do usuário.
    
7. Serviço EWS — o serviço EWS é descrito por três arquivos: Services. WSDL, messages. xsd, e Types. xsd, bem como os assemblies da API gerenciada do EWS. Services. WSDL descreve o contrato entre o cliente e o servidor, messages. xsd define as mensagens SOAP de solicitação e resposta e Types. xsd define os elementos usados nas mensagens SOAP. Messages. xsd e Types. xsd sempre contêm as versões mais recentes do esquema, embora existam versões anteriores do esquema. Observe que Services. WSDL, messages. xsd e Types. xsd são disponibilizados no servidor de acesso para cliente, mas que não são realmente usados para validação de esquema, são fornecidos apenas para referência. Os assemblies da API gerenciada do EWS são fornecidos para aplicativos clientes do EWS do servidor e são implantados em todas as funções do Exchange Server, não apenas nos servidores de acesso para cliente. Este componente só é visível na arquitetura local do Exchange.
    
    A disponibilidade de recursos é baseada na versão do esquema do EWS que seu aplicativo direciona. Como os esquemas do EWS são compatíveis com versões anteriores e posteriores, se você criar um aplicativo que tenha como destino uma versão de esquema anterior, como o Exchange 2007 SP1, seu aplicativo também funcionará com uma versão de esquema posterior, como o serviço do Exchange 2010 SP2, bem como o Exchange Online. Como recursos e atualizações de recurso são orientados pelo esquema, recomendamos que você use a base de código comum mais antiga que direciona os recursos do EWS que você deseja implementar no seu aplicativo cliente. Muitos aplicativos podem se concentrar na versão do Exchange2007_SP1, porque o esquema do Exchange 2007 SP1 contém quase todas as funcionalidades principais do Exchange para trabalhar com itens e pastas no repositório do Exchange. Para obter mais informações, consulte [EWS Client Features](ews-client-design-overview-for-exchange.md#EWSFeatures).
    
8. Grupo de disponibilidade de banco de dados (DAG) — os servidores de caixa de correio são organizados em um DAG altamente disponível, que pode ser implantado em um ou mais datacenters. O servidor de caixa de correio contém o banco de dados de caixa de correio e lida com todas as atividades das caixas de correio ativas nesse servidor. Todos os componentes que processam, colocam e armazenam dados estão no servidor de caixa de correio. Os clientes não se conectam diretamente ao servidor de caixa de correio; todas as conexões são tratadas pelo servidor de acesso para cliente. Este componente só é visível na arquitetura local do Exchange.
    
9. Exchange Online e Exchange Online como parte do Office 365 — a solução de mensagens hospedada que fornece recursos do Exchange como um serviço baseado em nuvem.
    
Quando um aplicativo EWS solicita informações do armazenamento do Exchange, uma mensagem de solicitação XML que está em conformidade com o padrão SOAP é criada e enviada ao servidor Exchange. Quando o servidor do Exchange recebe a solicitação, ele verifica as credenciais fornecidas pelo cliente e analisa automaticamente o XML para os dados solicitados. O servidor então cria uma resposta SOAP que contém dados XML que representam os objetos fortemente tipados solicitados e suas propriedades. Os dados XML são enviados de volta para o aplicativo em uma resposta HTTP. O aplicativo, em seguida, desserializa o XML e usa os dados para reformular os objetos fortemente tipados.
  
## <a name="protocols-and-standards-that-ews-applications-must-support"></a>Protocolos e padrões que os aplicativos EWS devem suportar
<a name="bk_standards"> </a>

Para se comunicar com um servidor Exchange, os aplicativos EWS devem oferecer suporte aos seguintes protocolos e padrões.
  
**Tabela 1. Protocolos**

|**Protocolo**|**Como ela é usada**|
|:-----|:-----|
|HTTP/S  <br/> |Permite que os aplicativos EWS acessem os dados do banco de dados do Exchange através da rede, independentemente se o cliente está na Internet ou na intranet.  <br/> |
|SOAP 1,0  <br/> |Forma um envelope em torno da carga de mensagens. O EWS implementa o protocolo SOAP usando partes diferentes do envelope SOAP para habilitar funcionalidades diferentes. O cabeçalho SOAP é usado para representação e para fornecer dados de controle de versão. O corpo SOAP fornece informações sobre a operação a ser executada e os dados que são enviados para a operação. O SOAP se baseia no WSDL para descrever as operações a serem chamadas.  <br/> |
|WSDL 1,0  <br/> |Descreve as associações, as operações e as propriedades que são usadas para chamar as operações do EWS, no arquivo Services. WSDL. Este arquivo, junto com os arquivos de esquema referenciados, abrange o contrato entre um aplicativo EWS e o servidor Exchange e é geralmente usado junto com ferramentas específicas do fornecedor para criar aplicativos específicos da plataforma. O arquivo WSDL está localizado no diretório virtual do EWS, que está na raiz do site.  <br/> |
|Segurança da camada de transporte (TLS)/SSL  <br/> |Fornece comunicações da Web seguras na Internet ou na intranet. O TLS permite que os aplicativos autentiquem servidores ou, opcionalmente, que os servidores autentiquem aplicativos do EWS. Ele também fornece um canal de segurança com a criptografia de comunicações. TLS é a versão mais recente do protocolo SSL (Secure Sockets Layer).  <br/> |
|XML/XSD  <br/> |Fornece um formato de mensagem universal para a troca de informações entre o servidor Exchange e o cliente. O XML fornece dados complexos do banco de dados do Exchange para aplicativos cliente, mas em uma estrutura definida. A beleza do XML é que ele permite a troca de dados mesmo quando um aplicativo e um servidor do EWS não compartilham uma plataforma comum.  <br/> |
   
Além disso, os aplicativos EWS devem suportar os seguintes padrões de autenticação:
  
- Autenticação básica sobre SSL, para aplicativos direcionados para o Exchange Online ou o Exchange no local.
    
- Autenticação NTLM sobre SSL, para aplicativos que dão suporte ao Exchange no local.
    
- Autenticação de token 2,0 OAuth, para aplicativos de parceiros confiáveis e interoperabilidade com o Lync Server 2013 e o SharePoint Server 2013.
    
## <a name="see-also"></a>Confira também


- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
    
- [Tipos de aplicativo do EWS](ews-application-types.md)
    
- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)
    

