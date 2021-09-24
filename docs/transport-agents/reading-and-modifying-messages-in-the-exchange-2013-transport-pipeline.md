---
title: Leitura e modificação de mensagens no pipeline de transporte Exchange 2013
manager: sethgros
ms.date: 09/17/2021
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b53ed47a-3d01-4c4e-ad32-fb0532872aad
description: Saiba mais sobre as .NET Framework que você pode usar no seu Exchange de transporte 2013 para ler, gravar e modificar mensagens.
ms.openlocfilehash: 5bf4406f7ca82512bb55388e0865e0d343cae66e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537233"
---
# <a name="reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline"></a>Leitura e modificação de mensagens no pipeline de transporte Exchange 2013

Saiba mais sobre as .NET Framework que você pode usar no seu Exchange de transporte 2013 para ler, gravar e modificar mensagens.
  
**Aplica-se a:** Exchange Server 2013
  
- Classes usadas para ler, gravar ou modificar mensagens
- Namespace de codificadores
- Namespace iCalendar
- Namespace MIME
- Namespace TextConverters
- Namespace Tnef
- namespace vCard
  
À medida que as mensagens passam pelo pipeline de transporte, seu agente de transporte pode ler, gravar e converter conteúdo de mensagem entre diferentes formatos de dados. Por exemplo, você pode ler e gravar dados MIME, identificar mensagens de entrada que estão no formato Uuencoded ou Quoted-printable (qp) e convertê-las em um padrão usado pela sua organização, ou ler e salvar informações de calendário ou contato associadas a mensagens de entrada. 
  
Você também pode identificar o conteúdo que representa uma ameaça de segurança e mover ou excluir o conteúdo ou as mensagens que os contêm; por exemplo, removendo links em uma mensagem HTML.
  
Este artigo fornece informações sobre as .NET Framework que você pode usar para ler, gravar e modificar mensagens.
  
> [!CAUTION]
> Muitas das propriedades e parâmetros nas APIs de conversão de conteúdo permitem valores grandes o suficiente para causar problemas de desempenho, incluindo negação de serviço. Ao usar as APIs de conversão de conteúdo em um agente de transporte, você deve implementar limites nos tamanhos de valor da propriedade e dos parâmetros que você suporta ao ler ou escrever para limitar o consumo de recursos pelo seu agente. 

<a name="Namespaces"> </a>

## <a name="classes-used-to-read-write-or-modify-messages"></a>Classes usadas para ler, gravar ou modificar mensagens

A tabela a seguir lista as .NET Framework que você pode usar para ler, gravar e modificar mensagens de email.
  
**.NET Framework namespaces de processamento de mensagens**

|**.NET Framework namespace**|**Aulas**|
|:-----|:-----|
|[Microsoft. Exchange. Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |Contém classes para codificação e decodificação na memória, uma classe de fluxo de codificador que aceita uma das classes de codificador ou decodificador contidas em uma enumeração associada, e a classe base [ByteEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoder.aspx) e a classe de exceção [ByteEncoderException](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoderException.aspx) para os codificadores e decodificadores.  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |Contém tipos que permitem ler e gravar fluxos de dados que contêm informações de calendário. Inclui um leitor de calendário e um escritor, um objeto de exceção, um objeto de recorrência e estruturas e enumerações que ajudam você a retornar informações de propriedade sobre itens de calendário.  <br/> |
|[Microsoft. Exchange. Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |Contém classes, estruturas, enumerações e representantes que você pode usar para criar, ler, gravar, percorrer, codificar e decodificar dados MIME. Inclui um leitor e um escritor baseado em fluxo que oferece acesso somente de leitura e gravação de encaminhamento a fluxos de dados MIME, bem como métodos e classes baseados em DOM que você pode usar em documentos MIME.  <br/> |
|[Microsoft. Exchange. Data.TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |Contém classes, estruturas, enumerações e representantes que permitem que você leia e escreva um fluxo de dados e execute conversões entre tipos de dados específicos; por exemplo, HTML para Rich Text Format (RTF). Os conversores de texto permitem alterar o formato de um fluxo de documento de um formulário para outro, bem como remover seletivamente elementos de um documento que podem representar um risco de segurança.  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |Contém um leitor e um escritor de fluxo somente de encaminhamento, uma classe de exceção e estruturas e enumerações que facilitam a leitura e a escrita de dados TNEF (Transport Neutral Encapsulation Format).  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |Contém um leitor e um escritor de fluxo somente de encaminhamento, uma classe de exceção e estruturas e enumerações que facilitam a leitura e a escrita de dados de contato formatados por vCard.  <br/> |
   
## <a name="encoders-namespace"></a>Namespace de codificadores
<a name="Encoders"> </a>

O namespace Encoders contém classes para codificação e decodificação na memória. Eles herdam da classe base [ByteEncoder.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoder.aspx) Classes codificam e decodificam Base64, BinHex, Quoted-printable (qp) e Unix-to-Unix (Uu). As seguintes classes são usadas para codificação e decodificação na memória: 
  
- [Base64Encoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.Base64Encoder.aspx)
    
- [Base64Decoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.Base64Decoder.aspx)
    
- [BinHexEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.BinHexEncoder.aspx)
    
- [BinHexDecoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.BinHexDecoder.aspx)
    
- [QPEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.QPEncoder.aspx)
    
- [QPDecoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.QPDecoder.aspx)
    
- [UUEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.UUEncoder.aspx)
    
- [UUDecoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.UUDecoder.aspx)
    
Os codificadores e decodificadores herdam da classe base [ByteEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoder.aspx) e usam a classe de exceção [ByteEncoderException](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.ByteEncoderException.aspx) para tratamento de erros. 
  
Além disso, o namespace contém a classe [MacBinaryHeader,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.MacBinaryHeader.aspx) que identifica arquivos codificados macBinary e lê seu header de arquivo associado. 
  
Por fim, a [classe EncoderStream](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.EncoderStream.aspx) executa uma conversão em um fluxo de dados em vez de um objeto na memória. Esta classe aceita uma das classes codificador ou decodificador e lê ou grava de acordo com a enumeração [EncoderStreamAccess](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.EncoderStreamAccess.aspx) associada. 
  
## <a name="icalendar-namespace"></a>Namespace iCalendar
<a name="iCalendar"> </a>

O namespace iCalendar fornece um leitor e um escritor somente de encaminhamento para dados iCalendar, além de suportar estruturas e classes para criar, acessar e modificar fluxos iCalendar.
  
As [classes CalendarReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.aspx) e [CalendarWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarWriter.aspx) são usadas para ler e gravar dados de fluxo iCalendar. 
  
O CalendarReader assume um [Stream](https://msdn.microsoft.com/library/System.IO.Stream.aspx) legível como um argumento para seus construtores. Em seguida, você pode usar os métodos [ReadFirstChildComponent,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ReadFirstChildComponent.aspx) [ReadNextSiblingComponent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ReadNextSiblingComponent.aspx)e [ReadNextComponent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ReadNextComponent.aspx) para acessar sequencialmente os componentes iCalendar no fluxo de dados. Com base no valor que você definiu para a propriedade [ComplianceMode,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ComplianceMode.aspx) erros no fluxo iCalendar causarão uma exceção a ser lançada ou fará com que a propriedade [ComplianceStatus](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarReader.ComplianceStatus.aspx) seja definida como um valor diferente de [Compatível](https://msdn.microsoft.com/library/microsoft.exchange.data.contenttypes.icalendar.calendarcompliancestatus.aspx). Você pode verificar essa propriedade para descobrir quaisquer problemas com dados iCalendar de entrada. 
  
A [classe CalendarWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarWriter.aspx) tem um [Stream](https://msdn.microsoft.com/library/System.IO.Stream.aspx) writable como um argumento para seus construtores. 
  
## <a name="mime-namespace"></a>Namespace MIME
<a name="MIME"> </a>

O namespace MIME fornece classes que permitem criar, acessar e modificar documentos MIME. Você pode trabalhar com documentos MIME usando um método baseado em stream ou dom.
  
### <a name="mimedocument-class-and-the-mime-dom"></a>Classe MimeDocument e o MIME DOM

A [classe MimeDocument](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.aspx) habilita o acesso dom a um documento MIME. Use objetos desse tipo quando você tiver a memória disponível para carregar um DOM inteiro e você deve ter acesso aleatório aos headers e ao conteúdo da mensagem. 
  
Você carrega dados em [um objeto MimeDocument](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.aspx) usando os [métodos GetLoadStream](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.GetLoadStream.aspx) ou [Load.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.Load.aspx) Em seguida, você pode seguir a hierarquia DOM e criar, modificar ou remover dados MIME. Depois de modificar os dados MIME, você pode gravar em um fluxo usando um dos métodos [WriteTo.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeNode.WriteTo.aspx) 
  
A figura a seguir mostra a estrutura de dados dentro de [um objeto MimeDocument.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.aspx) 
  
**Figura 1. Estrutura de objetos MimeDocument**

![MIME DOM Architecture](media/MimeDomArchitecture.gif)
  
### <a name="mimereader-and-mimewriter-classes-and-stream-based-mime-parsing"></a>Classes MimeReader e MimeWriter e análise MIME baseada em fluxo

As [classes MimeReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.aspx) [e MimeWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeWriter.aspx) permitem acesso somente encaminhamento a fluxos MIME. Use essas classes quando você não precisa alterar os dados MIME que exigem dados que já foram lidos ou gravados. Por exemplo, se você quiser imprimir mensagens que se ajustam a um formato predefinido, a [classe MimeWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeWriter.aspx) pode ser ideal. 
  
A [classe MimeDocument](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeDocument.aspx) encapsula um DOM. As [classes MimeReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.aspx) [e MimeWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeWriter.aspx) representam computadores de estado. Seus estados mudam com base na entrada recebida e nos métodos chamados. As figuras 2 a 5 são diagramas simplificados de transição de estado que mostram, para o [objeto MimeReader,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.aspx) quais métodos são válidos para chamar de cada estado e o estado que resultará. 
  
Para usar esses diagramas, siga as setas de um estado para o próximo, notando as chamadas de método ou retornando valores que causam a alteração do estado. Por exemplo, no primeiro diagrama, suponha que você está no início do fluxo que pertence ao MimeReader que você criou. Para chegar ao estado de Headers de Parte, chame um [dos ReadNextPart](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.ReadNextPart.aspx) ou [ReadFirstChildPart](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeReader.ReadFirstChildPart.aspx), nessa ordem. Se houver headers (ou seja, se o MIME estiver bem formado), você entrará no estado De Headers de Partes. Caso contrário, uma exceção será lançada. 
  
**Figura 2. Diagrama de transição de estado simplificado para objetos MimeReader**

![MimeReader State Diagram](media/MimeReader_StateDiagram_01.gif)
  
> [!NOTE]
> As figuras 3, 4 e 5 expandem-se em estados mostrados em cada um dos diagramas anteriores. 
  
**Figura 3. Expansão do estado de Headers de Parte da Figura 2**

![Expansion of 'Part Headers' state](media/MimeReader_StateDiagram_02.gif)
  
**Figura 4. Expansão do estado do Header da Figura 3 quando um parâmetro foi encontrado em um header**

![Expansão do estado 'Headers de parte' quando um parâmetro é encontrado em um header](media/MimeReader_StateDiagram_03.gif)
  
> [!NOTE]
> O estado representado pela Figura 5 é recursivo porque, se um grupo de endereços for encontrado, você poderá usar a propriedade [GroupRecipientReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeAddressReader.GroupRecipientReader.aspx) para ler os endereços no grupo. 
  
**Figura 5. Expansão do estado do Header da Figura 3 quando um endereço ou grupo de endereços é encontrado**

![Expansion of 'Header' state for address or group](media/MimeReader_StateDiagram_04.gif)
  
As figuras 6 e 7 mostram diagramas simplificados de transição de estado para o [objeto MimeWriter.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeWriter.aspx) 
  
> [!NOTE]
> A Figura 7 se expande no estado de Headers de Partes mostrado na Figura 6. 
  
**Figura 6. Diagrama de transição de estado simplificado para objetos MimeWriter**

![State Transition Diagram for MimeWriter](media/MimeWriter_TopLevel.gif)
  
**Figura 7. Expansão do estado de Headers de Parte da Figura 6**

![State Transition Diagram Expansion for MimeWriter](media/MimeWriter_Diagram_Expansion.gif)
  
## <a name="textconverters-namespace"></a>Namespace TextConverters
<a name="TextConverters"> </a>

O namespace TextConverters contém tipos que suportam a conversão do conteúdo das mensagens de email. Esses tipos podem executar a conversão de página de código, remover HTML que não seja seguro e realizar outras transformações em corpos de mensagens de email. [Microsoft.Exchange. O namespace Data.TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) inclui as seguintes classes derivadas da [classe abstrata TextConverter:](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextConverter.aspx) 
  
- [EnrichedToHtml](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.EnrichedToHtml.aspx)
    
- [EnrichedToText](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.EnrichedToText.aspx)
    
- [HtmlToEnriched](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlToEnriched.aspx)
    
- [HtmlToHtml](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlToHtml.aspx)
    
- [HtmlToRtf](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlToRtf.aspx)
    
- [HtmlToText](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlToText.aspx)
    
- [RtfCompressedToRtf](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfCompressedToRtf.aspx)
    
- [RtfToHtml](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfToHtml.aspx)
    
- [RtfToRtf](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfToRtf.aspx)
    
- [RtfToRtfCompressed](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfToRtfCompressed.aspx)
    
- [RtfToText](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.RtfToText.aspx)
    
- [TextToHtml](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextToHtml.aspx)
    
- [TextToRtf](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextToRtf.aspx)
    
- [TextToText](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextToText.aspx)
    
Esses conversores de texto permitem alterar o formato de um fluxo de documentos ou remover elementos que não estão seguros de um documento HTML. Essas classes podem ser usadas por conta própria para executar uma conversão usando uma única chamada para um dos métodos Convert na classe base [TextConverter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.TextConverter.aspx) ou podem ser passadas para um construtor do conversor, que a usa para executar leituras ou gravações convertidas. 
  
A funcionalidade herdada da classe base é útil para executar conversões quando você tem espaço suficiente para armazenar o documento original e sua saída convertida, ou quando você deseja armazenar os resultados da conversão. O **método Convert** aceita fluxos de entrada e saída, leitores de texto ou autores de texto e converte o conteúdo da entrada na saída associada. 
  
Também estão incluídas no namespace as seguintes classes de leitor de texto, escritor e fluxo:
  
- [ConverterReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.ConverterReader.aspx) — Derivado de **System.IO.TextReader**. 
    
- [ConverterWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.ConverterWriter.aspx) — Derivado de **System.IO.TextWriter**. 
    
- [ConverterStream](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.ConverterStream.aspx) — Derivado de **System.IO.Stream**. 
    
Elas são usadas para executar conversões quando você não tem espaço para armazenar a saída original ou convertida, quando você recebe a entrada ou envia a saída para um fluxo ou quando você deseja a saída apenas para fins de indexação ou pesquisa e, portanto, não deseja armazenar o resultado de uma conversão.
  
## <a name="tnef-namespace"></a>Namespace Tnef
<a name="TNEF"> </a>

O namespace Tnef contém classes e tipos que permitem a leitura e a escrita de dados TNEF somente para encaminhamento. O TNEF é um formato de dados usado para encapsular propriedades MAPI para clientes que não podem interpretar MAPI.
  
As [classes TnefReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.aspx) e [TnefWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefWriter.aspx) fornecem a funcionalidade principal no [Microsoft.Exchange. Namespace Data.ContentTypes.Tnef.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) 
  
A [classe TnefReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.aspx) tem um fluxo legível como um argumento para seus construtores. Em seguida, use o [método ReadNextAttribute](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.ReadNextAttribute.aspx) para ler sequencialmente os atributos no fluxo TNEF. Depois de ler um atributo, você pode acessar informações sobre o atributo usando qualquer uma das propriedades somente leitura no [objeto TnefReader,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.aspx) além de obter um [TnefPropertyReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefPropertyReader.aspx) para ler a propriedade atual. Você também pode acessar diretamente o atributo atual usando o [método ReadAttributeRawValue.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.ReadAttributeRawValue.aspx) 
  
A [classe TnefWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefWriter.aspx) assume um [Stream](https://msdn.microsoft.com/library/System.IO.Stream.aspx) writable como um argumento para seus construtores. A [classe TnefWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefWriter.aspx) fornece várias maneiras de gravar dados nesse fluxo. 
  
## <a name="vcard-namespace"></a>namespace vCard
<a name="vCard"> </a>

O namespace vCard contém classes, estruturas e enumerações usadas para ler e gravar informações de contato contidas em uma mensagem de email que está no formato de dados vCard. O namespace contém um leitor de contatos e um escritor, uma classe de exceção, um leitor de propriedades, um leitor de parâmetros e enumerações de suporte que permitem ler dados vCard associados a uma mensagem de email.
  
## <a name="see-also"></a>Confira também

- [Agentes de transporte no Exchange](transport-agents-in-exchange-2013.md)  
- [Conceitos de agente de transporte no Exchange 2013](transport-agent-concepts-in-exchange-2013.md) 
- [Referência do agente de transporte Exchange 2013](transport-agent-reference-for-exchange-2013.md)
- [Tipos de mídia MIME](http://www.iana.org/assignments/media-types)
    

