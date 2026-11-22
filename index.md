DIRETOR TÉCNICO — PACOTE COPILOT / AGENT BUILDER

PASSOS
1. Abra Microsoft 365 Copilot no navegador ou Teams.
2. Selecione Novo agente (New agent).
3. Escolha Configurar (Configure) / Ignorar para configurar (Skip to configure).
4. Nome: Diretor Técnico.
5. Descrição: Assistente da equipe de transmissão para orientar preparação, operação e diagnóstico seguro da infraestrutura audiovisual documentada.
6. Cole INSTRUCOES_PARA_COPILOT.txt no campo Instructions.
7. Em Knowledge, carregue os sete arquivos CONHECIMENTO_*.txt.
8. Adicione prompts iniciais:
   - Estou preparando a transmissão. Faça comigo o checklist.
   - A câmera 2 está sem imagem.
   - O áudio aparece no LUNA, mas não chega ao vMix.
   - A transmissão está travando. Ajude-me a diagnosticar.
   - Ative o Modo Responsável Técnico.
9. Teste no painel Try it com TESTES_08_CENARIOS_DE_VALIDACAO.txt.
10. Crie e compartilhe inicialmente apenas com um pequeno grupo piloto.

NOTAS
- Agent Builder aceita .txt como conhecimento; .md não aparece entre os formatos de upload incorporado documentados. Os arquivos foram convertidos para .txt preservando o conteúdo.
- O campo Instructions do Agent Builder tem limite documentado de 8.000 caracteres; o prompt foi reduzido para caber.
- Agent Builder permite compartilhar com pessoas/grupos específicos. Compartilhamento amplo depende das políticas do administrador. Para canais e publicação institucional mais avançados, use Copilot Studio.
- Recursos dependem da licença e das políticas do tenant Microsoft 365.
- O modo Responsável Técnico é uma seleção conversacional, não autenticação de identidade.
- Não inclua credenciais, senhas ou stream keys nos arquivos.
