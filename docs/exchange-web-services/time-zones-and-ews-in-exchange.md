---
title: Fusos horários e EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 0e0a666c-0541-414b-a7fb-297d94f692e6
description: Descubra como os fusos horários funcionam com a API gerenciada do EWS e o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: 8435087d7709b77e7562e2b9d50ece58377dd8db
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463745"
---
# <a name="time-zones-and-ews-in-exchange"></a>Fusos horários e EWS no Exchange

Descubra como os fusos horários funcionam com a API gerenciada do EWS e o EWS no Exchange.
  
Os fusos horários não são algo que a maioria das pessoas concede muito. No entanto, eles são um conceito importante ao especificar datas e horas usando a API gerenciada do EWS ou o EWS. A indisponibilidade de fusos horários em uma API gerenciada do EWS ou em um aplicativo EWS pode produzir resultados inesperados. É fácil lidar com fusos horários de forma adequada, contanto que você saiba como.
  
## <a name="handling-time-zones-in-the-ews-managed-api"></a>Manipulação de fusos horários na API gerenciada do EWS

Se você estiver usando a API gerenciada do EWS, os fusos horários são, na maioria das vezes, tratados automaticamente. Sem qualquer ação explícita em sua parte, a API usa o fuso horário local do computador cliente e lida com todas as conversões necessárias em segundo plano. Isso é ótimo quando esse é o efeito desejado, mas você tem outras opções.
  
Uma opção é definir a propriedade [ExchangeService. TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) . Essa propriedade controla o fuso horário de todas as solicitações executadas pela API gerenciada do EWS. Essa propriedade é somente leitura; a única maneira de definir isso é por meio do construtor de classe. Se você usar o [ExchangeService (System. TimeZoneInfo)](https://msdn.microsoft.com/library/dd635875%28v=exchg.80%29.aspx) ou o construtor [ExchangeService (ExchangeVersion, System. TimeZoneInfo)](https://msdn.microsoft.com/library/dd636248%28v=exchg.80%29.aspx) , você pode especificar um fuso horário específico como um objeto [System. TimeZoneInfo](https://msdn.microsoft.com/library/system.timezoneinfo%28v=vs.110%29.aspx) . Se você usar um dos outros construtores que não usam um objeto **TimeZoneInfo** como um parâmetro, a classe **ExchangeService** define a propriedade **timezone** como o fuso horário atual do computador cliente. 
  
Se você definir um fuso horário específico ou deixá-lo como o fuso horário do computador cliente, todas as datas e horas serão expressas no fuso horário representado pela propriedade **timezone** . A API gerenciada do EWS expõe todas as propriedades de data/hora como estruturas [System. DateTime](https://msdn.microsoft.com/library/system.datetime%28v=vs.110%29.aspx) . Portanto, se você definir as propriedades date/time, lembre-se de que a hora especificada será interpretada de acordo com o valor da propriedade [DateTime. Kind](https://msdn.microsoft.com/library/system.datetime.kind%28v=vs.110%29.aspx) no objeto **DateTime** . Se o valor da propriedade **Kind** for definido como **não especificado**, o valor de **DateTime** será interpretado como estando no fuso horário especificado pela propriedade **timezone** . Se você estiver lendo as propriedades de data/hora, todas as propriedades **DateTime** serão expressas nesse fuso horário. 
  
Se você estiver [criando novos compromissos ou reuniões](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md) ou [atualizando compromissos ou reuniões existentes](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md), você terá a capacidade de substituir o fuso horário especificado no **fuso horário** dos novos objetos de [compromisso](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) . No entanto, exatamente o que você pode substituir depende da [versão do esquema do EWS](ews-schema-versions-in-exchange.md) que você está direcionando. Para todos os valores da propriedade [ExchangeService. RequestedServerVersion](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) , você pode definir o [compromisso. StartTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) para usar um fuso horário específico para esse compromisso ou reunião. Se você estiver usando um valor para a propriedade **ExchangeService. RequestedServerVersion** maior que **Exchange2007_SP1**, você também pode definir a propriedade [compromisso. endtimezone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) , permitindo que você especifique um fuso horário para a propriedade [compromisso. end](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.end%28v=exchg.80%29.aspx) . No entanto, lembre-se de que essas propriedades só afetam a interpretação da data/hora para a solicitação de criação. Se você recuperar o compromisso, as horas de início e de término ainda serão expressas no fuso horário especificado pela propriedade **timezone** . 
  
Se estiver atualizando compromissos ou reuniões existentes, você poderá alterar o fuso horário de um objeto de **compromisso** definindo a propriedade **StartTimeZone** e/ou a propriedade **endtimezone** . Isso fará com que os tempos aplicáveis sejam deslocados de acordo. Se você definiu o **ExchangeService. RequestedServerVersion** como **Exchange2007_SP1**, não é possível definir a propriedade **endtimezone** ; o valor da propriedade **StartTimeZone** será usado em seu lugar. 
  
**Tabela 1. Propriedades de fuso horário na API gerenciada do EWS**

|**Propriedade de fuso horário**|**Versão mínima de solicitação do servidor**|**Descrição**|
|:-----|:-----|:-----|
|[TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) <br/> |**Exchange2007_SP1** <br/> |Se não for definida por meio do construtor da classe **ExchangeService** , essa propriedade será definida como o fuso horário do computador cliente. Todas as propriedades **DateTime** ao criar itens e ao recuperar itens existentes são expressas neste fuso horário. Esse fuso horário pode ser substituído em criar solicitações de compromissos e reuniões, configurando a propriedade **compromisso. StartTimeZone** e/ou **compromisso. endtimezone** . Se não for substituído pela propriedade **compromisso. StartTimeZone** , esse fuso horário é considerado o fuso horário de criação para compromissos e reuniões.  <br/> |
|[StartTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) <br/> |**Exchange2007_SP1** <br/> |Se definido em novos objetos **compromisso** , esse fuso horário é usado para interpretar as propriedades de [compromisso. Start](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.start%28v=exchg.80%29.aspx) e [compromisso. ReminderDueBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.reminderdueby%28v=exchg.80%29.aspx) . Esse fuso horário também é considerado o fuso horário de criação do objeto **compromisso** .  <br/> Ao recuperar itens existentes, essa propriedade é apenas informativa. Os valores das propriedades **DateTime** no compromisso existente são sempre expressos no fuso horário especificado pela propriedade **ExchangeService. TimeZone** .  <br/> |
|[EndTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) <br/> |**Exchange2010** <br/> |Se definido em novos objetos **compromisso** , esse fuso horário é usado para interpretar a propriedade [compromisso. end](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.end%28v=exchg.80%29.aspx) .  <br/> Ao recuperar itens existentes, essa propriedade é apenas informativa. Os valores das propriedades **DateTime** no compromisso existente são sempre expressos no fuso horário especificado pela propriedade **ExchangeService. TimeZone** .  <br/> |
   
## <a name="handling-time-zones-in-ews"></a>Tratamento de fusos horários no EWS

Se você estiver usando o EWS, os fusos horários não serão tratados automaticamente e as coisas serão um pouco mais complicadas. Como os fusos horários afetam as solicitações e respostas do EWS depende de vários fatores:
  
- A versão do Exchange especificada no elemento [RequestServerVersion](https://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx) 
    
- O fuso horário especificado no elemento [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) (se houver) 
    
- O fuso horário especificado nos elementos [MeetingTimeZone](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx), [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx)ou [endtimezone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) (se estiver presente em compromissos ou reuniões) 
    
- O fuso horário especificado nos elementos **DateTime** XML (se houver) 
    
O fuso horário especificado no valor dos elementos **DateTime** pode ter três formas. Você pode ler todos os detalhes no [esquema XML parte 2: datatypes segunda edição](http://www.w3.org/TR/xmlschema-2/#dateTime), mas parafraset:
  
- **UTC (tempo Universal Coordenado):** Especificado por ' Z '. Por exemplo,  `2014-06-06T19:00:00.000Z`
    
- **Fuso horário específico:** Especificado por ' + ' ou '-' seguido por horas e minutos. Por exemplo,  `2014-06-06T19:00:00.000-08:00`
    
- **Sem fuso horário:** Especificado pela ausência de qualquer fuso horário. Por exemplo,  `2014-06-06T19:00:00.000`
    
Se um fuso horário estiver presente em um valor de **Data/** hora (UTC ou um fuso horário específico), esse valor sempre será interpretado como esse fuso horário. Se nenhum fuso horário estiver presente, a interpretação do valor dependerá da combinação específica dos outros elementos relacionados ao fuso horário. 
  
**Tabela 2. Elementos de fuso horário no EWS e seus efeitos**

|**RequestServerVersion**|**TimeZoneContext presente?**|**MeetingTimeZone, StartTimeZone ou endtimezone presente (CalendarItem e MeetingRequest somente)?**|**dateTime em UTC**|**dateTime em fuso horário específico**|**dateTime sem fuso horário**|**Fuso horário de criação de compromisso e reunião**|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|**Exchange2007_SP1** <br/> |Sim  <br/> |Sim ( **MeetingTimeZone** )  <br/> |Interpretado como UTC  <br/> |Interpretado como o fuso horário indicado no valor  <br/> |Elementos dentro do elemento [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) ou [MeetingRequest](https://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) que contém o elemento **MeetingTimeZone** são interpretados como o fuso horário no elemento **MeetingTimeZone** , todos os outros interpretados como UTC  <br/> |Fuso horário no elemento **MeetingTimeZone**  <br/> |
|**Exchange2007_SP1** <br/> |Sim  <br/> |Não  <br/> |Interpretado como UTC  <br/> |Interpretado como o fuso horário indicado no valor  <br/> |Interpretado como UTC  <br/> |UTC  <br/> |
|**Exchange2007_SP1** <br/> |Não  <br/> |Sim ( **MeetingTimeZone** )  <br/> |Interpretado como UTC  <br/> |Interpretado como o fuso horário indicado no valor  <br/> |Elementos dentro do elemento [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) ou [MeetingRequest](https://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) que contém o elemento **MeetingTimeZone** são interpretados como o fuso horário no elemento **MeetingTimeZone** , todos os outros interpretados como UTC  <br/> |Fuso horário no elemento **MeetingTimeZone**  <br/> |
|**Exchange2007_SP1** <br/> |Não  <br/> |Não  <br/> |Interpretado como UTC  <br/> |Interpretado como o fuso horário indicado no valor  <br/> |Interpretado como UTC  <br/> |UTC  <br/> |
|**Exchange2010** e posterior  <br/> |Sim  <br/> |Sim ( **StartTimeZone** e/ou **endtimezone** )  <br/> |Interpretado como UTC  <br/> |Interpretado como o fuso horário indicado no valor  <br/> |Se o elemento **StartTimeZone** estiver presente, o valor dos elementos [Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) e [ReminderDueBy](https://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx) será interpretado como o fuso horário no elemento **StartTimeZone** . Caso contrário, o valor desses elementos será interpretado como o fuso horário no elemento **TimeZoneContext** .  <br/> Se o elemento **endtimezone** estiver presente, o valor do elemento [Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) será interpretado como o fuso horário no elemento **endtimezone** . Caso contrário, o valor do elemento **final** será interpretado como o fuso horário no elemento **TimeZoneContext** .  <br/> Elementos fora de [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) ou [MeetingRequest](https://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) são interpretados como o fuso horário no elemento **TimeZoneContext** .  <br/> |Fuso horário no elemento **StartTimeZone** se presente, fuso horário no elemento **TimeZoneContext** , se não  <br/> |
|**Exchange2010** e posterior  <br/> |Sim  <br/> |Não  <br/> |Interpretado como UTC  <br/> |Interpretado como o fuso horário indicado no valor  <br/> |Interpretado como o fuso horário no elemento **TimeZoneContext**  <br/> |Fuso horário no elemento **TimeZoneContext**  <br/> |
|**Exchange2010** e posterior  <br/> |Não  <br/> |Sim ( **StartTimeZone** e/ou **endtimezone** )  <br/> |Interpretado como UTC  <br/> |Interpretado como o fuso horário indicado no valor  <br/> |Se o elemento **StartTimeZone** estiver presente, o valor dos elementos [Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) e [ReminderDueBy](https://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx) será interpretado como o fuso horário no elemento **StartTimeZone** . Caso contrário, o valor desses elementos será interpretado como UTC.  <br/> Se o elemento **endtimezone** estiver presente, o valor do elemento [Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) será interpretado como o fuso horário no elemento **endtimezone** . Caso contrário, o valor do elemento **final** será interpretado como UTC.  <br/> Elementos fora de [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) ou [MeetingRequest](https://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) são interpretados como UTC.  <br/> |Fuso horário no elemento **StartTimeZone** , se presente, UTC se não  <br/> |
|**Exchange2010** e posterior  <br/> |Não  <br/> |Não  <br/> |Interpretado como UTC  <br/> |Interpretado como o fuso horário indicado no valor  <br/> |Interpretado como UTC  <br/> |UTC  <br/> |
   
Ao interpretar respostas do servidor, você sempre deve verificar o valor de cada elemento e interpretar o valor de acordo. O Exchange sempre inclui um fuso horário (UTC ou um fuso horário específico) no valor.
  
## <a name="additional-time-zone-considerations-when-creating-appointments-and-meetings"></a>Considerações adicionais de fuso horário ao criar compromissos e reuniões

Ao criar um compromisso ou reunião, o fuso horário que se aplica ao horário de início é considerado o fuso horário de criação do compromisso. Além de controlar como a data/horas são interpretadas quando um compromisso ou reunião é criado, o fuso horário de criação tem os seguintes efeitos no item:
  
- Se o item for um evento de dia inteiro, ele poderá ser exibido de modo inesperado se for exibido a partir de um cliente que esteja usando um fuso horário diferente do fuso horário de criação. Isso ocorre porque [quando um evento de dia inteiro é criado](how-to-create-all-day-events-by-using-ews-in-exchange.md), a hora de início e de término dos eventos de dia inteiro são ajustadas à meia-noite do fuso horário de criação. Esse horário será exibido como uma hora diferente da meia-noite em um fuso horário diferente, portanto, o item pode parecer ocupar dias extras. Por causa disso, recomendamos que você use o fuso horário configurado para o cliente de calendário principal do usuário para criar eventos de dia inteiro, sempre que possível.
    
- Se o item for uma reunião, o fuso horário de criação será exibido na barra de informações do Outlook nas solicitações de reunião recebidas pelos participantes, se esse fuso horário for diferente do fuso horário de seu cliente.
    
## <a name="in-this-section"></a>Nesta seção

- [Criar compromissos em um fuso horário específico usando o EWS no Exchange](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)
    
- [Atualizar o fuso horário de um compromisso usando o EWS no Exchange](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Versões de esquema do EWS no Exchange](ews-schema-versions-in-exchange.md)
    
- [Criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Atualizar compromissos e reuniões usando o EWS no Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Criar eventos de dia inteiro usando o EWS no Exchange](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [Estrutura DateTime](https://msdn.microsoft.com/library/system.datetime%28v=vs.110%29.aspx)
    
- [Classe TimeZoneInfo](https://msdn.microsoft.com/library/system.timezoneinfo%28v=vs.110%29.aspx)
    

