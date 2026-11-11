# Painel do Síndico

Aplicativo visual de administração de condomínio. É um único arquivo (`index.html`), sem instalação: basta abrir no navegador.

## Módulos

- **Painel**: arrecadação do mês, inadimplência, saldo em caixa, ocorrências abertas, fachada dos blocos colorida pela situação de cada unidade e gráfico de receitas × despesas dos últimos 6 meses.
- **Unidades**: fachada interativa e lista com busca e filtros. Ao abrir uma unidade: fração ideal, taxa, histórico de cobranças, registro de pagamento e edição dos dados do morador.
- **Financeiro**: cobranças por mês (registrar pagamento, estornar, gerar cobranças do mês) e despesas por categoria com lançamento de novas despesas. Débitos em atraso são atualizados com multa de 2% e juros de 1% ao mês, proporcionais aos dias.
- **Ocorrências**: quadro com Abertas, Em andamento e Resolvidas, com prioridade e local.
- **Reservas**: calendário das áreas comuns (salão, churrasqueira, espaço gourmet, quadra), com bloqueio de conflito de horário e de unidades inadimplentes.
- **Avisos**: mural com avisos fixados e botão para copiar o texto e colar no grupo dos moradores.

## Interações

- **Busca rápida** (`Ctrl K` ou `/`): unidades, moradores, ocorrências, avisos e ações.
- **Desfazer**: toda alteração mostra um aviso com o botão Desfazer.
- **Fachada interativa**: colorir por pagamento, ocorrências, vínculo ou encomendas; detalhes ao passar o mouse.
- **Gráfico clicável**: cada barra abre o mês no Financeiro.
- **Baixa em lote**: selecione várias cobranças e registre os pagamentos de uma vez.
- **Ocorrências**: arraste os cartões entre colunas; cada uma tem histórico com atualizações.
- **Reservas**: clique num dia do calendário e escolha um horário livre na grade de disponibilidade; filtre por espaço.
- **Unidade**: navegue com ← e →, copie a mensagem de cobrança para o WhatsApp, reserve, registre ocorrência ou encomenda.
- **Portaria**: encomendas (chegada e retirada) e visitantes (entrada e saída).
- **Tema** claro, escuro ou automático.

## Dados

O conteúdo inicial é de exemplo (48 unidades em 2 blocos). As alterações ficam salvas no navegador (`localStorage`). O botão **Restaurar exemplo** volta ao estado inicial.

## Próximos passos sugeridos

- Banco de dados compartilhado (por exemplo, Supabase) e login para síndico, conselho e moradores.
- Emissão de boletos/Pix e conciliação bancária.
