# Protocolos de emergência e diagnóstico

## Regra zero
Antes de sugerir qualquer ação: **a transmissão está ao vivo?** Se sim, preserve tudo que ainda funciona. Não reinicie, feche, desconecte, remova ou reconfigure componentes sem avaliar o impacto.

## Protocolo 1 — Câmera sem imagem no vMix

**Objetivo:** separar falha da câmera, cabo SDI, captura ou input.

1. Pergunte se a transmissão está ao vivo.
2. Pergunte se a outra câmera continua funcionando.
3. Pergunte se a imagem está preta, sem sinal ou congelada.
4. Confirme visualmente energia e conectores, sem desconectar.
5. Se disponível, verifique se há imagem no retorno local.
6. Registre o status/mensagem do Input correspondente no vMix.
7. Se persistir, encaminhe ao responsável técnico.

**Não fazer como primeira ação:** remover inputs, fechar vMix, iniciar projeto novo, trocar cabos durante o ar.

**Fora do ar:** o responsável pode avaliar o procedimento documentado de reconstruir inputs no projeto, preservando backup e configurações aprovadas.

## Protocolo 2 — LUNA tem sinal, vMix não tem áudio

1. Pergunte se está ao vivo.
2. Confirme se os medidores do LUNA se movimentam.
3. Confirme se os medidores da entrada de áudio do vMix se movimentam.
4. Observe se o input correto está selecionado.
5. Verifique visualmente os cabos entre a saída física e a UMC202HD, sem desconectar durante o ar.
6. Se o LUNA tem sinal e o vMix não, delimite a falha entre saída/interface/cabo/entrada/seleção no vMix.
7. Escalone se exigir reiniciar interface, fechar LUNA ou alterar roteamento.

**Procedimento original fora do ar:** salvar sessão LUNA, fechar LUNA, reiniciar a interface Dante Universal Audio e reabrir LUNA. Confirmar modelo e procedimento da interface antes de executar.

## Protocolo 3 — Midas M32 não chega ao LUNA

1. Pergunte se todos os canais foram afetados ou apenas alguns.
2. Verifique se os medidores da Midas mostram sinal.
3. Verifique se o LUNA recebe algum canal.
4. Se autorizado, consulte Dante Controller e registre dispositivos/status/mensagens.
5. Verifique visualmente o cabo Cat6 dedicado.
6. Não altere IP, clock, subscriptions, interfaces de rede ou roteamento.
7. Escalone ao responsável técnico.

**Procedimento original:** o manual cita Midas M32 com IP Dante `192.168.1.52`, Dante Controller e computador receptor. Não assuma que o endereço ou a topologia permanecem iguais sem validação.

## Protocolo 4 — TVs de retorno sem imagem

1. Determine se a transmissão pública continua normal.
2. Confirme se a falha afeta apenas as TVs.
3. Observe alimentação e indicadores do distribuidor SDI.
4. Verifique visualmente os conectores.
5. Se necessário, peça ao responsável técnico para avaliar o reinício do distribuidor, sabendo que isso interrompe o retorno local.
6. Não reinicie vMix ou câmeras se a transmissão pública estiver funcionando e o problema estiver restrito ao retorno.

**Procedimento original:** desligar a alimentação do distribuidor SDI por cinco segundos e religar. Usar somente com autorização e confirmação de que a interrupção do retorno é aceitável.

## Protocolo 5 — Transmissão instável ou engasgando

1. Pergunte se YouTube, Restream ou ambos estão afetados.
2. Confirme se o vMix local continua fluido.
3. Registre mensagem/status de cada saída.
4. Verifique visualmente conexões de rede.
5. Se houver teste de upload confiável, registre valor e horário.
6. Não reinicie roteador, switch ou computador durante o ar sem avaliar impacto.
7. Se um destino continuar funcionando, preserve-o.
8. A contingência documentada é pausar temporariamente a saída 4K e manter Full HD a 6.500 kbps, mas somente após explicar qual destino será afetado e obter autorização do operador/responsável.

O valor aproximado de 50 Mbps de upload livre consta do manual original e deve ser tratado como referência a validar, não como garantia.

## Protocolo 6 — Problema não previsto

1. Pergunte: “Estamos ao vivo agora?”
2. Pergunte: “O que exatamente parou de funcionar?”
3. Pergunte: “O que ainda está funcionando normalmente?”
4. Pergunte: “Quando começou e o que aconteceu imediatamente antes?”
5. Identifique a parte da cadeia de sinal relacionada.
6. Proponha uma verificação visual ou observacional de baixo risco.
7. Explique o que o resultado significa.
8. Faça apenas a próxima pergunta necessária.
9. Se a próxima ação for disruptiva ou não documentada, pare e escale.

## Mensagem de escalonamento pronta

“Precisamos de apoio técnico. O problema começou às [horário]. O sintoma é [descrição]. Está afetando [destino/equipamento]. Continua funcionando [itens]. Já verificamos [testes]. A mensagem apresentada foi [texto]. Não fizemos alterações avançadas.”

Não inclua senhas, tokens ou stream keys.
