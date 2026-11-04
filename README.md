# JARVIS IA

> Não só o seu agente, mas o seu amigo pessoal.

Assistente pessoal com inteligência artificial local, personalidade
adaptável, memória autorizada e uma interface futurista.

## Status do projeto

Fase 1 — Preparação e organização.

O projeto está em desenvolvimento. As funcionalidades descritas
abaixo são objetivos e ainda não estão implementadas.

## 1. Objetivo

Criar uma IA com identidade própria que combine:

- Assistente pessoal: ajudar em estudos, perguntas, planejamento
  e tarefas autorizadas.
- IA companheira: conversar naturalmente, conhecer preferências
  autorizadas e manter continuidade entre conversas.

A primeira versão será pessoal e executada no computador,
priorizando ferramentas gratuitas e processamento local.

No futuro, o projeto poderá evoluir para uma plataforma comercial.

## 2. Personalidade

O Jarvis deverá:

- Conversar em português brasileiro.
- Ser claro, respeitoso e natural.
- Utilizar humor quando adequado.
- Permitir ajustar formalidade, humor e tamanho das respostas.
- Reconhecer quando não souber alguma informação.
- Não fingir ter realizado ações.
- Identificar-se como inteligência artificial.
- Responder quando chamado por padrão.
- Iniciar conversas ou enviar lembretes somente com autorização.

## 3. Primeira versão — MVP

A primeira versão deverá permitir:

- Abrir a interface no computador.
- Enviar mensagens por texto.
- Receber respostas de um modelo local pelo Ollama.
- Conversar com a personalidade do Jarvis.
- Salvar memórias escolhidas e autorizadas pelo usuário.
- Consultar e apagar essas memórias.
- Utilizar uma interface futurista básica.

Voz, palavra de ativação, pesquisa na internet e execução de
tarefas serão implementadas em etapas posteriores.

## 4. Tecnologias planejadas

| Tecnologia | Finalidade |
|---|---|
| Python | Lógica principal |
| FastAPI | Comunicação entre interface e assistente |
| Ollama | Execução do modelo de IA local |
| HTML, CSS e JavaScript | Interface |
| SQLite | Memórias autorizadas |
| Faster-Whisper ou Whisper | Transcrição de voz |
| Piper | Geração de voz |
| openWakeWord | Detecção da palavra de ativação |
| Git e GitHub | Histórico e organização do código |

As ferramentas de voz serão avaliadas antes da implementação,
considerando compatibilidade, qualidade em português e licenças.

O modelo de IA será escolhido após verificar a memória RAM,
o processador e a placa de vídeo do computador.

## 5. Estrutura planejada

JARVIS-IA/
├── backend/
│   ├── main.py
│   ├── assistant.py
│   ├── personality.py
│   ├── ai/
│   │   └── model.py
│   ├── memory/
│   │   └── database.py
│   └── voice/
│       ├── listen.py
│       ├── speak.py
│       └── wake_word.py
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
├── data/
│   └── .gitkeep
├── requirements.txt
├── .gitignore
└── README.md

## 6. Responsabilidade dos arquivos

- main.py: iniciar o backend e definir os endpoints.
- assistant.py: organizar mensagens, personalidade e respostas.
- personality.py: definir as instruções de comportamento.
- ai/model.py: comunicar-se com o Ollama.
- memory/database.py: salvar, consultar e apagar memórias.
- voice/listen.py: transformar fala em texto.
- voice/speak.py: transformar texto em áudio.
- voice/wake_word.py: detectar a chamada de ativação.
- frontend/: apresentar a interface e suas interações.
- data/: armazenar dados locais que não serão enviados ao GitHub.
- requirements.txt: listar as dependências Python.

## 7. Etapas de desenvolvimento

### Fase 1 — Preparação pelo celular

- [ ] Criar o repositório privado.
- [ ] Adicionar este planejamento ao README.
- [ ] Criar a estrutura de arquivos.
- [ ] Configurar o .gitignore.
- [ ] Registrar as alterações com commits claros.

### Fase 2 — Primeira resposta local

- [ ] Verificar o hardware e o sistema do computador.
- [ ] Instalar Python e Ollama.
- [ ] Criar um ambiente virtual Python.
- [ ] Escolher e baixar um modelo compatível.
- [ ] Testar uma conversa diretamente no Ollama.
- [ ] Conectar Python ao Ollama.
- [ ] Receber uma resposta por texto.
- [ ] Tratar erros de conexão e modelo indisponível.

### Fase 3 — Personalidade

- [ ] Definir a identidade própria do Jarvis.
- [ ] Adicionar instruções de comportamento.
- [ ] Permitir configurar tom e tamanho das respostas.
- [ ] Testar a personalidade em diferentes conversas.

### Fase 4 — Memória

- [ ] Criar o banco SQLite.
- [ ] Implementar autorização explícita para salvar memórias.
- [ ] Permitir consultar as informações salvas.
- [ ] Permitir apagar uma memória ou todas.
- [ ] Recuperar memórias relevantes durante a conversa.
- [ ] Separar contexto temporário de memória permanente.

### Fase 5 — Interface do MVP

- [ ] Criar a tela de conversa.
- [ ] Conectar a interface ao backend.
- [ ] Exibir mensagens e respostas.
- [ ] Exibir estados de espera, processamento e erro.
- [ ] Adicionar configurações de personalidade e memória.
- [ ] Testar o fluxo completo do MVP.

### Fase 6 — Conversação por voz

- [ ] Implementar um botão para iniciar a escuta.
- [ ] Converter fala em texto.
- [ ] Gerar respostas em áudio.
- [ ] Avaliar uma voz em português brasileiro.
- [ ] Permitir interromper a reprodução.
- [ ] Exibir quando o microfone estiver ativo.

### Fase 7 — Ativação por voz

- [ ] Avaliar a detecção de “Ei, Jarvis”.
- [ ] Verificar a necessidade de um modelo de ativação próprio.
- [ ] Criar modos de espera e conversação.
- [ ] Permitir ativar e desativar a escuta.
- [ ] Testar falsas ativações e consumo de recursos.
- [ ] Avaliar um aplicativo desktop para abrir a janela
      quando chamado, conforme as permissões do sistema.

### Fase 8 — Integrações

- [ ] Selecionar as primeiras ferramentas úteis.
- [ ] Definir permissões para cada ferramenta.
- [ ] Pedir confirmação para ações sensíveis.
- [ ] Informar claramente quando uma ação falhar.
- [ ] Adicionar pesquisa online quando houver uma integração.
- [ ] Testar cada integração separadamente.

### Fase 9 — Evolução comercial

- [ ] Validar a utilidade e a estabilidade do produto.
- [ ] Revisar licenças de modelos, bibliotecas e vozes.
- [ ] Planejar cadastro e login.
- [ ] Separar dados e memórias por usuário.
- [ ] Avaliar PostgreSQL.
- [ ] Planejar hospedagem e custos de processamento.
- [ ] Implementar segurança, privacidade e exclusão de dados.
- [ ] Avaliar planos gratuitos e pagos.

## 8. Interface visual

A identidade visual deverá utilizar:

- Fundo azul-marinho escuro.
- Detalhes em azul elétrico e ciano.
- Núcleo central animado.
- Área de conversa legível.
- Histórico da sessão.
- Painel de configurações.
- Indicadores de escuta, processamento e resposta.
- Opção para reduzir animações.

A interface deverá mostrar apenas estados reais do sistema.
O indicador de escuta só aparecerá quando o microfone estiver ativo.

## 9. Privacidade e segurança

- Não salvar informações pessoais automaticamente.
- Solicitar autorização antes de criar memórias permanentes.
- Não manter histórico permanente por padrão.
- Permitir consultar e apagar os dados armazenados.
- Não enviar senhas, chaves, gravações ou bancos ao GitHub.
- Manter o microfone desligado até a ativação pelo usuário.
- Não executar comandos sugeridos pelo modelo sem controles.
- Manter o backend restrito ao computador no MVP.
- Informar quando uma integração precisar enviar dados externos.

O SQLite inicial não será considerado armazenamento criptografado.
Proteções adicionais deverão ser avaliadas antes de guardar
informações sensíveis ou atender outros usuários.

## 10. Regras do desenvolvimento

- Não utilizar APIs pagas inicialmente.
- Desenvolver uma funcionalidade de cada vez.
- Testar cada módulo antes de avançar.
- Evitar complexidade sem necessidade.
- Adicionar dependências somente quando forem utilizadas.
- Manter a documentação coerente com o que já funciona.
- Fazer commits pequenos e descritivos.
- Não confundir interface demonstrativa com funcionalidade pronta.

## 11. Limites da primeira versão

- O GitHub armazenará o código; ele não executará a IA local.
- O computador precisará estar ligado para o Jarvis funcionar.
- Instalações e downloads iniciais poderão exigir internet.
- O desempenho dependerá do hardware e do modelo escolhido.
- Pesquisa na internet dependerá de uma integração específica.
- Uma página web sozinha não garante ativação em segundo plano
  ou abertura da janela quando o sistema estiver bloqueado.
- “Ei, Jarvis” em português precisará ser validado na prática.

## 12. Critério de conclusão do MVP

O MVP estará concluído quando for possível:

1. Iniciar o Jarvis no computador.
2. Abrir a interface.
3. Enviar uma mensagem.
4. Receber uma resposta real do Ollama.
5. Aplicar a personalidade configurada.
6. Salvar uma memória com autorização.
7. Recuperar essa memória em uma nova conversa.
8. Consultar e apagar os dados salvos.
9. Ver mensagens claras quando ocorrer algum erro.

## Próximo passo

Concluir a estrutura inicial pelo celular.

Quando o computador estiver disponível, começar pela primeira
resposta em texto usando Python e Ollama.
