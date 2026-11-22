# Transmissão e vMix

## 1. Configuração documentada

O documento original descreve duas transmissões simultâneas gerenciadas pelo vMix:

| Destino | Plataforma/caminho | Perfil documentado |
|---|---|---|
| Stream 1 | YouTube, sinal principal | 4K, H.264, 35.000 kbps |
| Stream 2 | Restream | Full HD, 6.500 kbps |

O Restream é descrito como distribuidor para Instagram e computadores da Rede Minas.

Esses dados são a configuração registrada no manual original, não confirmação de que os perfis atuais estejam iguais. O documento não especifica frame rate, resolução exata em pixels, preset de encoder, keyframe interval, áudio, protocolo ou configuração de cada destino externo.

## 2. Falha, queda ou engasgos na transmissão

### Perguntas essenciais
1. A transmissão está no ar em algum destino?
2. Qual destino falhou: YouTube, Restream ou ambos?
3. O vMix mostra erro? Qual é a mensagem exata?
4. A imagem local no vMix continua fluida?
5. O problema começou após mudança de rede, computador, perfil ou cena?
6. O upload está sendo medido? Qual valor e por qual ferramenta?

### Verificações não disruptivas
- Observe o status de cada saída no vMix.
- Identifique se o problema é de um destino ou de ambos.
- Observe se o preview/program do vMix continua fluido.
- Verifique visualmente os cabos de rede e indicadores do switch, sem desconectar nada.
- Se houver medição confiável de upload, registre o valor e o horário.
- Confirme se outros serviços de internet estão apresentando instabilidade.

### Contingência documentada
O manual original propõe pausar temporariamente a saída 4K e manter apenas a saída Full HD a 6.500 kbps se a internet estiver oscilando.

**Atenção:** pausar uma saída pode encerrar ou interromper aquele destino. Antes de orientar:
- confirme qual destino está afetado;
- confirme que o destino Full HD está funcionando;
- explique que o YouTube principal poderá ficar indisponível se for a saída pausada;
- peça autorização ao operador/responsável;
- não prometa que isso resolverá a instabilidade.

O manual cita necessidade de aproximadamente 50 Mbps de upload livre para as duas saídas. Trate como estimativa registrada no documento, não como garantia universal ou medição atual. O consumo real pode variar com overhead, estabilidade, outros usos da conexão e comportamento do encoder.

## 3. Validação externa

O checklist original pede conferir YouTube e Instagram em celular, preferencialmente fora do Wi-Fi local, para validar imagem e áudio.

Ao orientar:
- não peça ao usuário para compartilhar senhas ou links privados de administração;
- confirme separadamente cada destino;
- observe áudio, vídeo e sincronismo;
- diferencie atraso normal de transmissão de falha;
- registre horário e destino.

## 4. Proteção das credenciais
Nunca solicite stream keys, senhas, tokens ou códigos de autenticação no chat. Se houver necessidade de inserir ou renovar uma chave, instrua o operador autorizado a fazê-lo diretamente na interface oficial do serviço.
