---
title: Fusos horários e EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0e0a666c-0541-414b-a7fb-297d94f692e6
description: Descubra como os fusos horários funcionam com o API gerenciada de EWS e EWS no Exchange.
ms.openlocfilehash: fcc8b00acf2b63de04718e13b82191de95bbf2b7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750963"
---
# <a name="time-zones-and-ews-in-exchange"></a>Fusos horários e EWS no Exchange

Descubra como os fusos horários funcionam com o API gerenciada de EWS e EWS no Exchange.
  
Fusos horários não são algo que fornecem a maioria das pessoas muito abstração para. No entanto, eles são um conceito importante ao se especificar datas e horas usando a API gerenciada de EWS ou EWS. Má gestão fusos horários em uma API gerenciada de EWS ou EWS aplicativo pode gerar resultados inesperados. Manipulação de fusos horários adequadamente é fácil, desde que você saiba como.
  
## <a name="handling-time-zones-in-the-ews-managed-api"></a>Manipulação de fusos horários na API gerenciada do EWS

Se você estiver usando a API gerenciada de EWS, fusos horários são, na maioria das vezes, manipulados para você automaticamente. Sem qualquer ação explícita de sua parte, a API usa o fuso horário local do computador cliente e lida com todas as conversões necessárias em segundo plano. Isso é ótimo quando que é o efeito desejado, mas você tiver outras opções.
  
Uma opção é a configuração da propriedade de [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) . Esta propriedade controlará o fuso horário para todas as solicitações executado pelo EWS Managed API. Essa propriedade é somente leitura; a única maneira de defini-la é via o construtor de classe. Se você usar o [ExchangeService(System.TimeZoneInfo)](http://msdn.microsoft.com/en-us/library/dd635875%28v=exchg.80%29.aspx) ou o construtor de [ExchangeService (ExchangeVersion, System.TimeZoneInfo)](http://msdn.microsoft.com/en-us/library/dd636248%28v=exchg.80%29.aspx) , você pode especificar um fuso horário específico como um objeto [System.TimeZoneInfo](http://msdn.microsoft.com/en-us/library/system.timezoneinfo%28v=vs.110%29.aspx) . Se você usar um dos outros construtores que não têm um objeto **TimeZoneInfo** como um parâmetro, a classe **ExchangeService** define a propriedade de **fuso horário** para o fuso horário atual do computador cliente. 
  
Se você definir um fuso horário específico ou deixá-lo como o fuso horário do cliente do computador, todas as datas e horas são expressas no fuso horário representado pela propriedade **TimeZone** . A API gerenciada de EWS expõe todas as propriedades de data/hora como estruturas de [DateTime](http://msdn.microsoft.com/en-us/library/system.datetime%28v=vs.110%29.aspx) . Isso se você definir as propriedades de data/hora, lembre-se de que o tempo que você especificar será interpretado de acordo com o valor da propriedade [Kind](http://msdn.microsoft.com/en-us/library/system.datetime.kind%28v=vs.110%29.aspx) no objeto **DateTime** . Se o valor da propriedade **tipo** é definido como **não especificado**, o valor de **DateTime** será interpretado como sendo no fuso horário especificado pela propriedade **TimeZone** . Se você estiver lendo propriedades de data/hora, todas as propriedades de **DateTime** são expressos nesse fuso horário. 
  
Se você estiver [Criando novos compromissos ou reuniões](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md) ou [atualização de compromissos ou reuniões existentes](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md), você tem a capacidade de substituir o fuso horário especificado no **fuso horário** para novos objetos de [compromisso](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) . No entanto, exatamente o que você pode substituir depende da [versão do esquema do EWS](ews-schema-versions-in-exchange.md) que você está direcionando. Todos os valores da propriedade [ExchangeService.RequestedServerVersion](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) , você pode definir o [Appointment.StartTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) usar um fuso horário específico para essa reunião ou compromisso. Se você estiver usando um valor da propriedade **ExchangeService.RequestedServerVersion** maior **Exchange2007_SP1**, você pode também definir a propriedade [Appointment.EndTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) , permitindo que você especifique um fuso horário para o [ Appointment.End](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.end%28v=exchg.80%29.aspx) propriedade. No entanto, tenha em mente que essas propriedades só afetam a data/hora para a solicitação de criar a interpretação. Se você recuperar o compromisso, os horários de início e término ainda serão expressos no fuso horário especificado pela propriedade **TimeZone** . 
  
Se você estiver atualizando compromissos ou reuniões existentes, você pode alterar o fuso horário para um objeto de **compromisso** , definindo a propriedade **StartTimeZone** e/ou a propriedade **EndTimeZone** . Isso fará com que os tempos de aplicáveis deslocar adequadamente. Se você definiu o **ExchangeService.RequestedServerVersion** como **Exchange2007_SP1**, você não pode definir a propriedade **EndTimeZone** ; o valor da propriedade **StartTimeZone** será usado em seu lugar. 
  
**Tabela 1. Propriedades de fuso horário na API gerenciada do EWS**

|**Propriedade de fuso horário**|**Versão de solicitação mínima do servidor**|**Descrição**|
|:-----|:-----|:-----|
|[Fuso horário](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) <br/> |**Exchange2007_SP1** <br/> |Se não definida via construtor para a classe **ExchangeService** , essa propriedade é definida para o fuso horário do computador cliente. Todas as propriedades de **data/hora** ao criar itens e ao recuperar existente itens são expressas neste fuso horário. Neste momento zona pode ser substituída em criar solicitações de compromissos e reuniões, definindo o **Appointment.StartTimeZone** e/ou a propriedade **Appointment.EndTimeZone** . Se não é substituída pela propriedade **Appointment.StartTimeZone** , este fuso horário é considerado o fuso horário de criação de compromissos e reuniões.  <br/> |
|[StartTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) <br/> |**Exchange2007_SP1** <br/> |Se definido em novos objetos de **compromisso** , este fuso horário é usado para interpretar as propriedades [Appointment.Start](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.start%28v=exchg.80%29.aspx) e [Appointment.ReminderDueBy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.reminderdueby%28v=exchg.80%29.aspx) . Este fuso horário também é considerado o fuso horário de criação para o objeto de **compromisso** .  <br/> Ao recuperar itens existentes, essa propriedade é apenas informativa. Os valores das propriedades de **data/hora** no compromisso existente sempre são expressas no fuso horário especificado pela propriedade **ExchangeService.TimeZone** .  <br/> |
|[EndTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) <br/> |**Exchange2010** <br/> |Se definido em novos objetos de **compromisso** , este fuso horário é usado para interpretar a propriedade [Appointment.End](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.end%28v=exchg.80%29.aspx) .  <br/> Ao recuperar itens existentes, essa propriedade é apenas informativa. Os valores das propriedades de **data/hora** no compromisso existente sempre são expressas no fuso horário especificado pela propriedade **ExchangeService.TimeZone** .  <br/> |
   
## <a name="handling-time-zones-in-ews"></a>Manipulação de fusos horários no EWS

Se você estiver usando o EWS, fusos horários não são manipulados automaticamente para você e coisas são um pouco mais complicadas. Como os fusos horários afetam o EWS solicitações e respostas depende de vários fatores:
  
- A versão do Exchange especificada no elemento [RequestServerVersion](http://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx) 
    
- O fuso horário especificado no elemento [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) (se presente) 
    
- Fuso horário especificado nos elementos [MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx), [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx)ou [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) (se presente em compromissos ou reuniões) 
    
- Fuso horário especificado nos elementos XML **dateTime** (se houver) 
    
O fuso horário especificado no valor de **dateTime** elementos pode demorar três formas. Você pode ler todos os detalhes em [XML esquema parte 2: tipos de dados Second Edition](http://www.w3.org/TR/xmlschema-2/#dateTime), mas Parafraseando:
  
- **Universal Coordenado (UTC):** Especificado por 'Z'. Por exemplo,`2014-06-06T19:00:00.000Z`
    
- **Fuso horário específico:** Especificações de HttpCachePolicy '+' ou '-' seguido de horas e minutos. Por exemplo,`2014-06-06T19:00:00.000-08:00`
    
- **Nenhum fuso horário:** Especificado pela ausência de qualquer fuso horário. Por exemplo,`2014-06-06T19:00:00.000`
    
Se um fuso horário estiver presente em um valor de **data/hora** (UTC ou um fuso horário específico), esse valor sempre será interpretado como esse fuso horário. Se nenhum fuso horário estiver presente, em seguida, a interpretação do valor depende a combinação específica dos outros elementos relacionados fuso horário. 
  
**Tabela 2. Elementos de fuso horário no EWS e seus efeitos**

|**RequestServerVersion**|**TimeZoneContext presente?**|**MeetingTimeZone, StartTimeZone ou EndTimeZone presente (CalendarItem e MeetingRequest somente)?**|**Data e hora em UTC**|**dateTime no fuso horário específico**|**dateTime com nenhum fuso horário**|**Fuso horário de criação de compromissos e reuniões**|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|**Exchange2007_SP1** <br/> |Sim  <br/> |Sim ( **MeetingTimeZone** )  <br/> |Interpretada como UTC  <br/> |Interpretada como o fuso horário indicado no valor  <br/> |Elementos contidos no elemento [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) ou [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) que contém o elemento **MeetingTimeZone** são interpretados como o fuso horário no elemento **MeetingTimeZone** , todos os outros interpretada como UTC  <br/> |Fuso horário no elemento **MeetingTimeZone**  <br/> |
|**Exchange2007_SP1** <br/> |Sim  <br/> |Não  <br/> |Interpretada como UTC  <br/> |Interpretada como o fuso horário indicado no valor  <br/> |Interpretada como UTC  <br/> |UTC  <br/> |
|**Exchange2007_SP1** <br/> |Não  <br/> |Sim ( **MeetingTimeZone** )  <br/> |Interpretada como UTC  <br/> |Interpretada como o fuso horário indicado no valor  <br/> |Elementos contidos no elemento [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) ou [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) que contém o elemento **MeetingTimeZone** são interpretados como o fuso horário no elemento **MeetingTimeZone** , todos os outros interpretada como UTC  <br/> |Fuso horário no elemento **MeetingTimeZone**  <br/> |
|**Exchange2007_SP1** <br/> |Não  <br/> |Não  <br/> |Interpretada como UTC  <br/> |Interpretada como o fuso horário indicado no valor  <br/> |Interpretada como UTC  <br/> |UTC  <br/> |
|**Exchange2010** e posterior  <br/> |Sim  <br/> |Sim ( **StartTimeZone** e/ou **EndTimeZone** )  <br/> |Interpretada como UTC  <br/> |Interpretada como o fuso horário indicado no valor  <br/> |Se o elemento **StartTimeZone** estiver presente, o valor dos elementos [ReminderDueBy](http://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx) e [Iniciar](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) são interpretados como o fuso horário no elemento **StartTimeZone** . Caso contrário, o valor desses elementos são interpretadas como o fuso horário no elemento **TimeZoneContext** .  <br/> Se o elemento **EndTimeZone** estiver presente, o valor do elemento [Iniciar](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) será interpretado como o fuso horário no elemento **EndTimeZone** . Caso contrário, o valor do elemento **End** será interpretado como o fuso horário no elemento **TimeZoneContext** .  <br/> Elementos fora do [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) ou [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) são interpretados como o fuso horário no elemento **TimeZoneContext** .  <br/> |Fuso horário no elemento **StartTimeZone** se presente, o fuso horário no elemento **TimeZoneContext** se não  <br/> |
|**Exchange2010** e posterior  <br/> |Sim  <br/> |Não  <br/> |Interpretada como UTC  <br/> |Interpretada como o fuso horário indicado no valor  <br/> |Interpretada como o fuso horário no elemento **TimeZoneContext**  <br/> |Fuso horário no elemento **TimeZoneContext**  <br/> |
|**Exchange2010** e posterior  <br/> |Não  <br/> |Sim ( **StartTimeZone** e/ou **EndTimeZone** )  <br/> |Interpretada como UTC  <br/> |Interpretada como o fuso horário indicado no valor  <br/> |Se o elemento **StartTimeZone** estiver presente, o valor dos elementos [ReminderDueBy](http://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx) e [Iniciar](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) são interpretados como o fuso horário no elemento **StartTimeZone** . Caso contrário, o valor desses elementos são interpretadas como UTC.  <br/> Se o elemento **EndTimeZone** estiver presente, o valor do elemento [Iniciar](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) será interpretado como o fuso horário no elemento **EndTimeZone** . Caso contrário, o valor do elemento **End** será interpretado como UTC.  <br/> Elementos fora do [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) ou [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) são interpretados como UTC.  <br/> |Fuso horário no elemento **StartTimeZone** se presente, UTC se não  <br/> |
|**Exchange2010** e posterior  <br/> |Não  <br/> |Não  <br/> |Interpretada como UTC  <br/> |Interpretada como o fuso horário indicado no valor  <br/> |Interpretada como UTC  <br/> |UTC  <br/> |
   
Ao interpretar respostas do servidor, você deve verificar o valor de cada elemento e interpretar o valor de acordo. Exchange sempre incluirá um fuso horário (UTC ou um fuso horário específico) no valor.
  
## <a name="additional-time-zone-considerations-when-creating-appointments-and-meetings"></a>Considerações de fuso horário adicional ao criar compromissos e reuniões

Quando você cria um compromisso ou reunião, o fuso horário que se aplica à hora de início é considerado o fuso horário de criação para o compromisso. Além de controlar como o date/times são interpretadas quando um compromisso ou reunião é criado, o fuso horário de criação tem os seguintes efeitos no item:
  
- Se o item é um evento de dia inteiro, ela pode exibir de forma inesperada se exibidos a partir de um cliente que está usando um fuso horário diferente do fuso horário de criação. Isso ocorre porque a hora de [quando um evento de dia inteiro for criado](how-to-create-all-day-events-by-using-ews-in-exchange.md), o início e fim de eventos de dia inteiro são ajustados para meia-noite da zona de tempo de criação. Esse horário será exibido como um horário que não seja a meia-noite em um fuso horário diferente, portanto, o item pode aparecer autorizem os dias adicionais. Por isso, é recomendável que você use o fuso horário configurado para o cliente de calendário principal do usuário para criar eventos de dia inteiro quando possível.
    
- Se o item tem uma reunião, o fuso horário de criação será exibido na barra de informações do Outlook em que as solicitações de reunião recebidas pelos participantes, se esse fuso horário diferente do fuso horário do seu cliente.
    
## <a name="in-this-section"></a>Nesta se��o

- [Criar compromissos em um fuso horário específico usando o EWS no Exchange](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)
    
- [Atualizar o fuso horário para um compromisso usando o EWS no Exchange](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Versões de esquema do EWS no Exchange](ews-schema-versions-in-exchange.md)
    
- [Criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Atualizar compromissos e reuniões usando o EWS no Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Criar eventos de dia inteiro usando o EWS no Exchange](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [Estrutura DateTime](http://msdn.microsoft.com/en-us/library/system.datetime%28v=vs.110%29.aspx)
    
- [Classe TimeZoneInfo](http://msdn.microsoft.com/en-us/library/system.timezoneinfo%28v=vs.110%29.aspx)
    

