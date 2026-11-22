# Vídeo, câmeras e monitoramento

## 1. Arquitetura documentada

- Câmeras: Blackmagic Cinema Camera 2.5K (modelo 2014).
- Saída das câmeras: SDI.
- Captura: Blackmagic DeckLink Duo 2, Inputs 1 e 2, no computador de transmissão.
- Distribuição auxiliar: distribuidor SDI alimenta televisões de retorno local.

Este documento não especifica o modelo do distribuidor, os formatos SDI, as resoluções, as taxas de quadros, o comprimento dos cabos ou o padrão de referência/sincronismo.

## 2. Câmera sem imagem no vMix

### Primeiro, determine o cenário
- Estamos ao vivo?
- A câmera 1 continua funcionando?
- O Input 2 está preto, sem sinal, ou a imagem está congelada?
- A câmera mostra imagem em algum retorno local?
- O problema começou após alguma mudança?

### Verificações não invasivas
1. Observe se a câmera está ligada e apresenta indicação normal.
2. Confira visualmente se o cabo SDI está conectado e travado nas duas extremidades.
3. Observe se o retorno local correspondente tem imagem, se isso puder ser verificado sem desconectar nada.
4. Observe no vMix se o Input 1 funciona e se o Input 2 indica ausência de sinal ou imagem congelada.
5. Registre qualquer mensagem apresentada.

Não troque cabos ou entradas durante a transmissão se isso puder derrubar outro sinal. Não remova inputs, reinicie o vMix ou crie um projeto novo durante o evento como primeira tentativa.

### Procedimento original registrado
O manual original sugere remover os inputs das câmeras, fechar o template, iniciar projeto novo e adicionar novamente a DeckLink Duo 2 Inputs 1 e 2, reconfigurando as transmissões.

**Uso restrito:** este é um procedimento de recuperação para preparação ou manutenção, não uma primeira resposta durante transmissão. Pode interromper a saída, perder configuração e exigir chaves de transmissão. Só executar fora do ar, com backup do projeto e responsável autorizado. Nunca peça ao voluntário para inserir ou compartilhar stream keys no chat.

## 3. Câmera: exposição e movimento

O documento original define:
- Shutter Angle: 180° como valor de referência travado.
- Abertura da lente: controle principal de luz.
- ISO nativo: 800 como referência e último recurso para aumentar.

### Explicação ao voluntário
- **Abertura/íris:** controla quanta luz entra pela lente. Um número f menor significa abertura maior.
- **ISO:** altera a sensibilidade/ganho do sensor; aumentar demais pode deixar a imagem granulada.
- **Shutter angle:** influencia o aspecto do movimento. A orientação local documentada é manter 180°.

### Cuidados
- Não altere parâmetros de câmera durante a transmissão sem autorização.
- Antes de orientar ajustes, confirme qual câmera está sendo usada e se o operador tem autorização.
- Não afirme que ISO 800 é sempre correto para qualquer condição; é o valor nativo indicado no documento local, mas a condição real precisa ser avaliada.
- Não confunda imagem escura com falha de sinal.

## 4. Televisões de retorno sem imagem

O manual original indica como causa possível mau contato ou travamento do distribuidor SDI.

### Diagnóstico seguro
1. Determine se a transmissão pública continua normal.
2. Confirme se o problema está apenas nas TVs de retorno.
3. Observe se o distribuidor está energizado e se há indicadores.
4. Verifique visualmente os conectores SDI/BNC, sem desconectar cabos em uso.
5. Se a falha persistir, acione o responsável técnico.

### Procedimento original registrado
O manual original sugere desligar o distribuidor SDI da fonte, aguardar cinco segundos e religar.

**Ressalva:** isso interrompe o retorno local. Só faça se o retorno puder ficar temporariamente indisponível, o modelo do distribuidor e sua alimentação forem conhecidos e houver autorização. Não confunda retorno local com transmissão pública.

## 5. Distinção importante
- **Sem imagem no vMix:** investigar câmera → SDI → DeckLink → configuração do input.
- **Sem imagem apenas nas TVs:** investigar distribuidor SDI e ramais de retorno.
- **Imagem escura ou estourada:** investigar exposição, não tratar como falha de cabo ou captura.
- **Imagem congelada:** distinguir congelamento da fonte, captura e software antes de reiniciar qualquer coisa.
