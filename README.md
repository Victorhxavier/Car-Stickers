# Política de Privacidade — Car Stickers

**Última atualização:** 17 de agosto de 2026
**Aplicável ao app:** Car Stickers (Android e iOS)

Esta política explica, em linguagem direta, quais dados o Car Stickers coleta, por que coleta, com quem compartilha e como você pode pedir a exclusão da sua conta. Se algum trecho não ficar claro, é só escrever pra gente — o contato está no final da página.

## Sumário

1. [Quem somos](#1-quem-somos)
2. [Dados que coletamos](#2-dados-que-coletamos)
3. [Fotos de carros e reconhecimento por IA](#3-fotos-de-carros-e-reconhecimento-por-ia)
4. [Com quem compartilhamos dados](#4-com-quem-compartilhamos-dados)
5. [Anúncios (AdMob)](#5-anúncios-admob)
6. [O que é público dentro do app](#6-o-que-é-público-dentro-do-app)
7. [Como protegemos seus dados](#7-como-protegemos-seus-dados)
8. [Por quanto tempo guardamos os dados](#8-por-quanto-tempo-guardamos-os-dados)
9. [Seus direitos e exclusão de conta](#9-seus-direitos-e-exclusão-de-conta)
10. [Uso por menores de idade](#10-uso-por-menores-de-idade)
11. [Mudanças nesta política](#11-mudanças-nesta-política)
12. [Contato](#12-contato)

## 1. Quem somos

O Car Stickers é um aplicativo de coleção de figurinhas de carros: você fotografa veículos, uma inteligência artificial identifica o modelo e, ao confirmar, a figurinha entra na sua coleção com pontos de experiência (XP). Esta política cobre o app mobile e o backend que ele consulta.

## 2. Dados que coletamos

Coletamos apenas o necessário para o app funcionar. Nada de rastreamento entre apps, nada de venda de dados a terceiros.

| Dado | Quando | Para quê |
|---|---|---|
| Nome e e-mail | Criação de conta | Login, identificação no ranking, suporte |
| Senha | Criação de conta | Login — guardamos só o *hash* (bcrypt), nunca o texto em claro |
| Fotos de carros | Uso da câmera do app | Reconhecimento do modelo por IA (ver seção 3) |
| Progresso no jogo | Uso contínuo | XP, nível, coleção, missões, sequência de dias, ranking |
| Identificador de publicidade | Exibição de anúncios | Google AdMob — ver seção 5 |

Não coletamos localização, contatos, lista de outros apps instalados, nem usamos SDKs de analytics ou rastreamento de comportamento fora do app.

## 3. Fotos de carros e reconhecimento por IA

Quando você fotografa um carro, a foto é enviada aos nossos servidores e, de lá, para a **API Gemini do Google** (processamento de imagem por IA), que devolve marca, modelo e ano prováveis. Isso acontece em toda foto enviada para reconhecimento.

**O que acontece com a foto depois:**

- Se o carro **não é identificado**, a foto é usada só na chamada à IA e descartada — não fica salva nos nossos servidores.
- Se o resultado **precisa de confirmação manual** (confiança média) ou se o modelo do carro é **novo no catálogo**, a primeira foto é guardada como referência, para nossa equipe validar o cadastro do modelo — não para identificar você pessoalmente.

> **Sobre exclusão dessas fotos:** hoje não temos um processo automático de expurgo dessas fotos de referência após a validação. Se você quiser que uma foto sua seja removida dos nossos servidores, pode pedir a qualquer momento pelo contato da seção 12 — atendemos manualmente.

## 4. Com quem compartilhamos dados

Compartilhamos dados só com os serviços abaixo, cada um com sua própria política de privacidade:

- **Google (API Gemini)** — recebe as fotos enviadas para reconhecimento (seção 3).
- **Google AdMob** — veicula os anúncios do app (seção 5).

Não vendemos dados pessoais a terceiros, sob nenhuma circunstância.

## 5. Anúncios (AdMob)

O app exibe anúncios em banner e vídeos recompensados (que liberam fotografias extras por dia) através do **Google AdMob**. O AdMob pode coletar identificadores de publicidade do dispositivo e dados técnicos (modelo do aparelho, versão do sistema) para exibir e medir anúncios, conforme a [política de privacidade do Google](https://policies.google.com/privacy).

Você pode gerenciar a personalização de anúncios nas configurações de privacidade do seu Google/dispositivo.

## 6. O que é público dentro do app

O **ranking** do app mostra seu **nome** e seu **XP total** para os demais usuários — é a única informação sua visível a outras pessoas dentro do app. Seu e-mail, suas fotos e o restante da sua conta nunca são exibidos publicamente.

## 7. Como protegemos seus dados

- Senhas armazenadas com *hash* bcrypt — nunca em texto simples.
- Sessão autenticada por token (JWT), guardado no dispositivo em armazenamento seguro do sistema operacional (Keychain/Keystore via `expo-secure-store`).
- Comunicação entre o app e nossos servidores é criptografada (HTTPS).

## 8. Por quanto tempo guardamos os dados

Dados de conta e de jogo (nome, e-mail, coleção, XP) ficam guardados enquanto sua conta existir. Fotos de referência para validação de catálogo seguem a política descrita na seção 3. Ao excluir sua conta (seção 9), removemos os dados de identificação associados a ela.

## 9. Seus direitos e exclusão de conta

Nos termos da LGPD (Lei Geral de Proteção de Dados) e de legislações equivalentes, você pode a qualquer momento:

- Pedir uma cópia dos dados que temos sobre você;
- Corrigir dados incorretos ou desatualizados;
- Pedir a exclusão da sua conta e dos dados associados a ela.

**Como pedir:** envie um e-mail para [privacidade@carstickers.app](mailto:privacidade@carstickers.app) a partir do endereço cadastrado na sua conta, com o assunto "Exclusão de conta". Confirmamos o recebimento e removemos seus dados de identificação em até 30 dias. Dados que precisamos manter por obrigação legal (ex.: registros fiscais, se houver) podem ser retidos pelo prazo exigido por lei.

Hoje esse pedido é feito por e-mail — ainda não existe um botão de "excluir conta" dentro do app.

## 10. Uso por menores de idade

O Car Stickers não é direcionado a crianças menores de 13 anos e não coletamos intencionalmente dados de menores dessa idade. Se você acredita que uma criança nos forneceu dados pessoais, entre em contato pela seção 12 para que possamos removê-los.

## 11. Mudanças nesta política

Podemos atualizar esta política conforme o app evolui. Mudanças relevantes serão refletidas na data no topo da página. Recomendamos revisitar esta página periodicamente.

## 12. Contato

Dúvidas sobre esta política ou sobre seus dados? Escreva para [privacidade@carstickers.app](mailto:privacidade@carstickers.app).

---

Car Stickers — Política de Privacidade · versão de 17/08/2026
