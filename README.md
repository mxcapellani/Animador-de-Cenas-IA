# Cinematic Scene Animator Ultimate

Versão 1.0.0 — repositório Animador-de-Cenas-IA.

Professional Agent Skill for cinematic image-to-video animation prompts, advanced camera movements, visual storytelling, scene continuity, realistic motion and creative filmmaking direction.

## Finalidade
Transformar imagem ou descrição de cena em direção cinematográfica textual, com prompts em inglês. Comunicação no idioma do usuário. Manter identidade, composição e coerência física sem redesenhar a referência.

## Funcionalidades preservadas e Ultimate
O núcleo incorpora integralmente a especificação operacional fornecida: interpretação de cenas, câmera, movimento, atmosfera, variações e formato copiável. Inclui os 12 modos e todo o vocabulário de movimentos/efeitos do anexo. Controle de continuidade, conflito, intensidade, planejamento temporal, sequência e revisão são capacidades Ultimate especificadas, ainda sem validação comportamental comparativa.

Padrão: cinco alternativas distintas — Balanced, Atmospheric, Dynamic, Poetic e High Impact. Quantidade explícita tem prioridade, inclusive pedido de um único prompt. Text to Motion aceita descrição sem exigir imagem.

## Uso
- “Anime esta imagem com movimento suave.”
- “Crie um único Dolly In em plano contínuo.”
- “Planeje três cenas mantendo roupa e direção de deslocamento.”
- “Corrija os movimentos contraditórios deste prompt.”

## Instalação
Ver [instalação](docs/INSTALLATION.md). Núcleo em [.agents/skills/cinematic-scene-animator/SKILL.md](.agents/skills/cinematic-scene-animator/SKILL.md). Publicação no GitHub não instala automaticamente a Skill no ChatGPT.

## Estrutura
Núcleo autossuficiente, duas referências, documentação, fonte integral, exemplos, quinze testes comparativos, validador, testes do validador e CI. Ver [exemplos](examples/EXAMPLES.md), [auditoria](docs/AUDIT.md) e [testes](docs/COMPARATIVE-TESTS.md).

## Dependências e limites
Texto não exige APIs ou geração de vídeo. Visão é necessária apenas para observar imagens reais; vídeo final requer ferramenta externa. Não há renderização automática, publicação em redes ou garantia de identidade perfeita. Nomes de movimentos e efeitos não são presets universais. Não alegar suporte técnico de uma plataforma sem confirmação.

## Validação
```bash
python -m pip install -r tests/requirements.txt
python tests/validate.py
python tests/test_validator.py
```
Python 3.9+ e PyYAML 6.x; instalação inicial pode precisar de rede. Verificações locais não exigem credenciais. CI em push e pull request tem acesso somente de leitura ao conteúdo. Esses testes medem estrutura e detecção de falhas, não qualidade de animação.

## Atualização e licença
Consultar [changelog](CHANGELOG.md) e [contribuições](CONTRIBUTING.md). Preservar recursos, registrar regressões e repetir casos relevantes. MIT, copyright 2026 mxcapellani. Equivalência ao original e compatibilidade dos geradores permanecem não demonstradas.
