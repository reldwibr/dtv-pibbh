# Infraestrutura geral e áudio

## 1. Visão geral documentada

### Cadeia de áudio descrita

Midas M32 → rede Cat6 dedicada/Dante → computador de áudio → Universal Audio LUNA → interface Dante da Universal Audio → saída física estéreo Output 1/2 L/R → entrada estéreo da Behringer UMC202HD → USB → computador do vMix.

**Importante:** esta é a arquitetura descrita no documento original. A identificação exata do modelo da interface Dante Universal Audio, a configuração de driver/roteamento e o modo como a saída do LUNA chega à interface precisam ser confirmados localmente.

## 2. Equipamentos e informações documentadas

- Console: Midas M32.
- IP Dante informado: `192.168.1.52`.
- Transporte: cabo Cat6 em rede dedicada Dante.
- Computador de áudio: duas conexões descritas — Wi-Fi para atualizações/software e rede cabeada dedicada para Dante.
- DAW: Universal Audio LUNA.
- Interface: interface de áudio Dante da Universal Audio, modelo não especificado.
- Saída física indicada: Output 1/2 L/R.
- Interface no computador de vídeo: Behringer UMC202HD via USB.
- Software de transmissão: vMix.

Não presuma que o IP indicado é endereço de controle remoto da M32; o documento o identifica como IP Dante. Não altere endereços IP.

## 3. Patch de canais documentado

| Canal | Fonte | Observação |
|---:|---|---|
| 01 | Bumbo | Bateria |
| 02 | Caixa | Bateria |
| 03 | Vago | Não utilizado |
| 04 | Tom | Bateria |
| 05 | Surdo | Bateria |
| 06 | Over L | Pratos/ambiência |
| 07 | Over R | Pratos/ambiência |
| 08 | Contrabaixo elétrico | Linha/DI |
| 09 | Teclado L | Estéreo |
| 10 | Teclado R | Estéreo |
| 11 | Violão | Linha/DI |
| 12 | Guitarra | Linha/microfone |
| 13 | Piano | Linha/DI |
| 14 | Livre | Reserva |
| 15 | Livre | Reserva |
| 16 | Livre | Reserva |
| 17 | Microfone 01 | Voz geral/equipe |
| 18 | Microfone 02 | Voz geral/equipe |
| 19 | Microfone 03 | Voz geral/equipe |
| 20 | Microfone 04 | Voz geral/equipe |
| 21 | Vago | Não utilizado |
| 22 | Microfone Shure | Microfone principal/referência |

O documento diz que a numeração das pistas do LUNA espelha o patch físico da Midas M32. Trate isso como referência documentada, mas confirme o patch atual antes de orientar mudanças.

## 4. Diagnóstico: áudio no LUNA, mas ausente no vMix

### Objetivo
Descobrir se o sinal deixa de existir na saída do LUNA, na interface Dante/saída física, na Behringer ou na entrada selecionada no vMix.

### Perguntas iniciais
1. A transmissão está ao vivo?
2. Os medidores do LUNA se movimentam?
3. Os medidores da Behringer/entrada correspondente no vMix se movimentam?
4. O problema começou após alguma alteração ou reinicialização?

### Verificações seguras
- Observe se o medidor do LUNA se movimenta.
- Observe se a entrada correspondente à Behringer no vMix apresenta sinal.
- Confirme visualmente se os cabos de áudio estão firmes, sem desconectar nada durante a transmissão.
- Verifique se o input de áudio correto está selecionado no projeto, sem alterar configurações se estiver ao vivo.

### Procedimento original registrado
O manual original propõe salvar a sessão no LUNA, fechar o programa, reiniciar a interface Dante Universal Audio e abrir o LUNA novamente. **Esse procedimento é disruptivo e não deve ser recomendado como primeira ação durante uma transmissão.** Use-o somente fora do ar, após confirmar o modelo e o procedimento correto da interface e com autorização do responsável.

## 5. Diagnóstico: Midas M32 não chega ao LUNA

### Objetivo
Delimitar se a origem está na captação/console, no transporte Dante ou na recepção/processamento do computador.

### Perguntas iniciais
1. A Midas está ligada e operando normalmente?
2. O problema afeta todos os canais ou apenas alguns?
3. Os medidores dos canais na Midas mostram sinal?
4. O LUNA recebe algum canal?
5. O Dante Controller mostra os dispositivos esperados?

### Verificações seguras
- Observe os medidores na Midas.
- Observe os medidores de entrada no computador/DAW.
- Se autorizado e fora de risco operacional, consulte o Dante Controller para verificar se os dispositivos aparecem e se há indicação de erro.
- Não altere subscriptions, clock, endereços IP, interfaces de rede ou roteamento sem o responsável técnico.

### Procedimento original registrado
O manual original sugere abrir o Dante Controller, verificar Routing e a presença da Midas M32 (`192.168.1.52`) e da interface Universal Audio, e, se um dispositivo estiver ausente ou em vermelho, verificar o Cat6 e reiniciar o computador receptor Dante.

**Ressalva:** não assuma que a cor/ícone isolado identifica a causa. Registre o status e a mensagem apresentada. Reiniciar o computador pode interromper o serviço; não faça durante a transmissão sem avaliar o impacto e obter autorização.

## 6. Limites e pendências
Consulte `08_PENDENCIAS_DE_VALIDACAO.md` para identificar dados ainda não confirmados. Não invente:
- modelo da interface Dante Universal Audio;
- configuração de clock Dante;
- nome da placa de rede usada pelo Dante;
- subscriptions e roteamentos;
- configuração de saída do LUNA;
- canal/entrada física exata da UMC202HD;
- configuração de driver e input no vMix.
