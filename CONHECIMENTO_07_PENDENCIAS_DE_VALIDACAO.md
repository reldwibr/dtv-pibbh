# Pendências de validação técnica

Este arquivo impede que o agente trate lacunas como fatos. Os itens abaixo não são necessariamente erros; são informações ausentes ou que precisam ser confirmadas com o responsável técnico.

## Áudio e Dante
- [ ] Modelo exato da interface Dante Universal Audio.
- [ ] Como o LUNA envia o mix estéreo para a interface Dante (driver, dispositivo e roteamento).
- [ ] Modelo e função exata da interface Dante no fluxo.
- [ ] Qual dispositivo atua como clock leader Dante e qual configuração foi aprovada.
- [ ] Nome da interface de rede dedicada ao Dante no computador.
- [ ] Topologia física: ligação direta ou via switch; modelo do switch, se houver.
- [ ] Confirmação de que `192.168.1.52` é o endereço Dante atual da Midas M32.
- [ ] Subscriptions Dante atuais e nomes exatos dos dispositivos/canais.
- [ ] Saída física Output 1/2 L/R: modelo, conectores e destino.
- [ ] Entrada física usada na Behringer UMC202HD e configuração de nível.
- [ ] Input/driver exato selecionado no vMix.

## Vídeo e câmeras
- [ ] Confirmação dos modelos e quantidade de câmeras em uso.
- [ ] Formato de saída de cada câmera: resolução, frame rate e padrão SDI.
- [ ] Formato configurado em cada input da DeckLink Duo 2.
- [ ] Modelo do distribuidor SDI e sua alimentação.
- [ ] Diagrama de distribuição SDI para as TVs de retorno.
- [ ] Comprimentos e identificação dos cabos SDI.
- [ ] Configuração de exposição aprovada para cada câmera e lente.

## vMix e transmissão
- [ ] Versão atual do vMix.
- [ ] Resolução e frame rate do projeto.
- [ ] Encoder e parâmetros detalhados de cada destino.
- [ ] Confirmação de que YouTube 4K H.264 a 35.000 kbps continua sendo o perfil aprovado.
- [ ] Confirmação de que Restream Full HD a 6.500 kbps continua sendo o perfil aprovado.
- [ ] Como Instagram e Rede Minas recebem o sinal do Restream atualmente.
- [ ] Upload medido em condições de evento e margem de segurança aprovada.
- [ ] Procedimento autorizado para contingência de um único destino.
- [ ] Local seguro de backup do projeto/template do vMix.

## Governança operacional
- [ ] Quem pode autorizar reinicialização de cada equipamento.
- [ ] Quem pode alterar rede, Dante, câmeras, encoder e destinos.
- [ ] Quem assume a operação em caso de falha crítica.
- [ ] Procedimento de contato/escalonamento durante o evento.
- [ ] Janela de manutenção e política de atualização.

## Regra para o agente
Até que um item seja confirmado, informe que ele está pendente. Faça perguntas ao responsável técnico para preencher a documentação. Não invente respostas nem transforme recomendações genéricas em configuração local.
