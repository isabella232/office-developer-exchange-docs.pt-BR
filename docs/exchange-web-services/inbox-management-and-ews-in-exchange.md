---
title: Gerenciamento de caixa de entrada e EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 3dfa0fc9-64bb-4d18-bff7-bf6b3bed4a0d
description: Descubra como gerenciar sua Caixa de Entrada em sua API Gerenciada EWS ou aplicativo EWS usando regras de Caixa de Entrada e a lista de envios bloqueados.
ms.openlocfilehash: 6dddb8d462276c4983fd04a0206d4d4a9be32df8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522212"
---
# <a name="inbox-management-and-ews-in-exchange"></a>Gerenciamento de caixa de entrada e EWS no Exchange

Descubra como gerenciar sua Caixa de Entrada em sua API Gerenciada EWS ou aplicativo EWS usando regras de Caixa de Entrada e a lista de envios bloqueados.
  
Exchange caixas de correio vêm equipadas com recursos para ajudar os usuários a organizar seus emails de entrada automaticamente. Todos esses recursos operam no servidor sem intervenção do usuário, mas atendem a necessidades diferentes. A API Gerenciada EWS e o EWS fornecem acesso a esses recursos, permitindo que seus usuários gerenciem suas Caixas de Entrada.
  
**Tabela 1. Recursos de gerenciamento de caixa de entrada**

|**Se você quiser...**|**Use...**|
|:-----|:-----|
|Tome medidas em mensagens de entrada (como movimentação para outra pasta ou exclusão delas) com base em critérios específicos (como remetente, assunto ou anexos)  <br/> |Regras da caixa de entrada  <br/> |
|Excluir todos os emails de entrada de um remetente específico  <br/> |Lista de Remetentes Bloqueados  <br/> |
   
## <a name="inbox-rules"></a>Regras da caixa de entrada
<a name="bk_InboxRules"> </a>

Vamos enfrentar isso: nem todas as mensagens de email são criadas igualmente. Para cada email que um usuário recebe de seu gerente, há um de uma lista de distribuição de vídeo de gato da Internet que ele ingressou anos atrás e nunca chegou a sair. Embora os vídeos de gatos da Internet sejam divertidos, a quantidade de tráfego que a lista de distribuição obtém pode sair do controle e mensagens importantes podem ser facilmente perdidas no mar de mensagens de lista de distribuição em uma Caixa de Entrada. Muitos usuários se voltaram para as regras de Caixa de Entrada para ajudar a parear essas mensagens e tornar sua Caixa de Entrada um lugar muito melhor para estar. Com Exchange Web Services (EWS), seu aplicativo pode trazer o poder das regras para suportar.
  
A API Gerenciada do EWS fornece os métodos [ExchangeService.GetInboxRules](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getinboxrules%28v=exchg.80%29.aspx) e [ExchangeService.UpdateInboxRules](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.updateinboxrules%28v=exchg.80%29.aspx) para trabalhar com regras. O EWS fornece as [operações GetInboxRules](https://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx) e [UpdateInboxRules](https://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx) para trabalhar com regras. No entanto, observe que a API Gerenciada EWS e o EWS têm as seguintes limitações ao trabalhar com regras de Caixa de Entrada: 
  
- O EWS não pode acessar ou criar regras ou regras "somente cliente" definidas no Outlook para executar "somente neste computador".
    
- Para alterar o conjunto atual de regras usando o EWS, você precisa remover o BLOB das regras Outlook, se ele estiver presente. Isso significa que o uso do EWS para modificar regras exclui todas as regras que foram desativadas anteriormente (desabilitadas) usando Outlook. 
    
### <a name="how-do-rules-work"></a>Como funcionam as regras?
<a name="bk_HowRulesWork"> </a>

O mecanismo de regras age como um gatekeeper para a caixa de correio de um usuário. Quando uma mensagem chega à caixa de correio do usuário, mas antes da mensagem aparecer na Caixa de Entrada, essa mensagem é avaliada em relação a uma lista ordenada de regras. Observe que isso só ocorre no momento da chegada e somente na Caixa de Entrada. Essas regras são compostas por três partes: [Condições,](#bk_Conditions) [Ações](#bk_Actions)e [Exceções.](#bk_Exceptions)
  
A partir da regra na parte superior da lista de regras, o mecanismo de regras executa as etapas a seguir até chegar ao final da lista de regras:
  
1. Verifica a mensagem para determinar se ela atende a todas as condições especificadas na regra.
    
1. Se atender a todas as condições, a avaliação continuará com a etapa 2.
    
2. Se ele não atender a todas as condições, o mecanismo de regras carregará a próxima regra na lista de regras e iniciará na etapa 1.
    
2. Verifica a mensagem para determinar se ela atende a qualquer uma das exceções especificadas na regra.
    
1. Se atender a qualquer uma das exceções, o mecanismo de regras carregará a próxima regra na lista de regras e iniciará na etapa 1.
    
2. Se ele não atender a nenhuma das exceções, a avaliação continuará com a etapa 3.
    
3. Executa as ações especificadas na regra na mensagem.
    
1. Se a ação "parar de processar mais regras" for especificada, o mecanismo de regras executará todas as outras ações na mensagem e sairá sem avaliar nenhuma regra adicional em relação à mensagem.
    
2. Se a ação "parar de processar mais regras" não for especificada, o mecanismo de regras carregará a próxima regra na lista de regras e começará na etapa 1.
    
A figura a seguir mostra o processo que o mecanismo de regras segue.
  
**Figura 1: Visão geral do mecanismo de regras**

![Um diagrama que mostra as etapas usadas pelo mecanismo de regras, começando pela avaliação da regra, determinando em seguida se os critérios da regra são atendidos e, por fim, executando a ação ou movendo para a regra seguinte até ser concluído.](media/Ex15_Rules_EngineOverview.png)
  
### <a name="putting-the-pieces-together---parts-of-a-rule"></a>Juntando as partes - partes de uma regra
<a name="bk_Pieces"> </a>

Uma maneira de visualizar as partes de uma regra é imaginar que você está dando instruções a alguém que tem a tarefa de organizar seu email de entrada. Você pode dizer a essa pessoa: "Quando uma mensagem chegar, faça , a \<insert conditions here\> menos que a mensagem \<insert actions here\> \<insert exceptions here\> . Vamos dar uma olhada mais de perto em cada parte.
  
#### <a name="conditions"></a>Condições
<a name="bk_Conditions"> </a>

[As](https://msdn.microsoft.com/library/f049a48c-9585-43f7-8549-0b8cb19a5eea%28Office.15%29.aspx) condições descrevem quando uma regra deve ser aplicada. Embora você possa omitir as condições de uma regra (resultando em uma regra que se aplica a cada mensagem recebida), é muito mais comum que as regras tenham condições que se apliquem a um subconjunto de mensagens de entrada. Alguns exemplos são "quando uma mensagem é de Sadie" ou "quando uma mensagem é enviada para a lista de distribuição "Gatos De Vídeo". As regras podem ter várias condições. Quando as regras têm mais de uma condição, todas as condições devem ser atendidas para que o mecanismo de regras tome a ação especificada. 
  
#### <a name="actions"></a>Ações
<a name="bk_Actions"> </a>

[As](https://msdn.microsoft.com/library/c5aa96b1-2d8b-422f-8c2f-f118572ab23f%28Office.15%29.aspx) ações descrevem o que acontece quando uma regra se aplica. Os exemplos são "mover a mensagem para a pasta 'Gatos'" ou "marcar a mensagem com importância 'Baixa'". As regras podem ter várias ações. Quando você especifica várias ações para uma regra, todas as ações são executadas quando a regra é aplicada. 
  
#### <a name="exceptions"></a>Exceções
<a name="bk_Exceptions"> </a>

[As exceções](https://msdn.microsoft.com/library/7cd63ac2-3441-4ed4-915b-6f90af4b28fc%28Office.15%29.aspx) descrevem quando uma regra não deve ser aplicada, mesmo que os critérios especificados nas condições sejam atendidos. Os exemplos são "exceto se a mensagem for enviada somente para mim" ou "exceto se a mensagem for de Mom". Uma regra pode ter várias exceções. Quando as regras têm mais de uma exceção e qualquer uma das exceções é atendida, a regra não é aplicada. 
  
### <a name="example-herding-those-cats"></a>Exemplo: herdando esses gatos
<a name="bk_Example"> </a>

Vamos ver como os usuários podem usar regras para eliminar o tráfego dessa lista de distribuição de vídeo de gato da Internet. Vamos supor o seguinte:
  
- Essas mensagens são enviadas para uma lista de distribuição chamada "Internet Cat Video Enthusiasts".
    
- Seus usuários querem ler essas mensagens eventualmente, mas não querem que eles atraplem sua Caixa de Entrada. Eles preferem arquivar em uma pasta chamada "Gatos".
    
- Seus usuários querem ler mensagens enviadas para essa lista de distribuição imediatamente pela sua mãe, pois a mãe envia os vídeos mais divertidos.
    
Isso informa ao mecanismo de regras o seguinte: "Quando uma mensagem é enviada para a lista de distribuição "Entusiastas de Vídeo de Gato da Internet", mova-a para a pasta "Gatos", a menos que a mensagem seja de Mom." 
  
**Tabela 2. Definição de regra**

|**Parte de regra**|**Value**|
|:-----|:-----|
|Condições  <br/> |Enviado para a lista de distribuição 'Internet Cat Video Enthusiasts'  <br/> |
|Ações  <br/> |Mover a mensagem para a pasta 'Gatos'  <br/> E parar de processar mais regras  <br/> |
|Exceções  <br/> |De 'Mom'  <br/> |
   
> [!NOTE]
> Observe que "parar de processar mais regras" é uma das ações na regra resultante. Em geral, é uma boa ideia incluir essa ação para evitar confusão sobre quais regras atuam em qualquer mensagem. No entanto, ao omitir essa ação e ordenar corretamente suas regras, você pode obter um processamento mais avançado do seu email de entrada. Nesse caso, provavelmente é uma aposta segura que as mensagens de vídeo de gato da Internet não exigem muito no modo de processamento avançado. 
  
Pouco depois de criar essa regra, uma nova mensagem entra. Um colega de trabalho, Hope, envia uma mensagem para a lista de distribuição. Se executarmos mentalmente o trabalho do mecanismo de regras, a mensagem atenderá a todas as condições (ela é enviada para "Entusiastas de Vídeos de Gato da Internet" e não atende a nenhuma das exceções (não é de 'Mom'), portanto, a regra se aplica e a mensagem é movida para a pasta 'Gatos'.
  
A figura a seguir mostra como a regra é aplicada a uma mensagem de email de entrada.
  
**Figura 2. A mensagem de entrada é processada por uma regra**

![Uma ilustração que mostra uma nova mensagem enviada à lista de distribuição de um colaborador. A mensagem atende a todas as condições e a nenhuma das exceções definidas na regra, e é movida para a pasta Cats.](media/Ex15_Rules_RuleEvaluationSample.png)
  
## <a name="blocking-senders"></a>Bloqueio de senders
<a name="bk_Blocking"> </a>

Embora você possa criar uma regra que mova todos os emails de um remetente específico para a pasta Lixo Eletrônico, você também pode fazer isso usando a Lista de Remetentes Bloqueados em suas opções de Lixo Eletrônico. Como há um limite para quantas regras um usuário pode ter, faz sentido usar a Lista de Envios Bloqueados. Você pode [adicionar ou remover](how-to-add-and-remove-email-addresses-from-blocked-senders-list-by-using-ews.md) endereços de email específicos da Lista de Envios Bloqueados usando o método [EXCHANGEService.MarkAsJunk](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) EWS Managed API ou a [operação EWS MarkAsJunk.](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) Observe que, para que o EWS acesse a Lista de Remetentes Bloqueados, a caixa de correio do usuário deve conter uma mensagem de email do endereço de email que você deseja adicionar ou remover. 
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_InThisSection"> </a>

- [Gerenciar regras de Caixa de Entrada usando o EWS Exchange](how-to-manage-inbox-rules-by-using-ews-in-exchange.md)
    
- [Adicionar e remover endereços de email da Lista de Envios Bloqueados usando o EWS no Exchange](how-to-add-and-remove-email-addresses-from-blocked-senders-list-by-using-ews.md)
    
## <a name="see-also"></a>Confira também


- [Desenvolver clientes do serviço Web para o Exchange](develop-web-service-clients-for-exchange.md)
    
- [Operação GetInboxRules](https://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx)
    
- [Operação UpdateInboxRules](https://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx)
    
- [Operação MarkAsJunk](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)
    

