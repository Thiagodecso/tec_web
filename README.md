<img width="2168" height="331" alt="KeppLog" src="https://github.com/user-attachments/assets/b25fc5ef-c580-4350-a465-8204ea8e38e0" />

> Status: Em desenvolvimento  ⚠️

O **KeepLog** é uma plataforma web desenvolvida para a disciplina de **Tecnologias Web** da **Universidade Federal do Ceará (UFC) – Campus Sobral (2026)**. O sistema propõe a modernização do controle de insumos e ferramentas utilizados nos laboratórios acadêmicos, substituindo registros manuais ou planilhas descentralizadas por uma solução digital integrada. A nomenclatura do projeto baseia-se na fusão dos conceitos de **Keep** (guardar, reter e proteger o patrimônio) e **Log** (histórico imutável e rastreável de eventos).

##  Problemática

Os laboratórios do campus possuem um fluxo contínuo de materiais, ferramentas e componentes de alto valor educativo e financeiro. A ausência de um sistema centralizado de controle resulta em cenários de incerteza, como a dificuldade para rastrear com precisão a entrada e a saída de materiais. Essa falta de acompanhamento gera perdas frequentes de itens e ineficiência operacional, visto que estudantes e técnicos gastam tempo procurando insumos ou são surpreendidos pelo desabastecimento de componentes essenciais de última hora. O KeepLog atua diretamente como uma ferramenta de governança para mitigar essas falhas, garantindo transparência, sustentabilidade e organização em tempo real.

## Interface do Catálogo
<img width="1881" height="748" alt="image" src="https://github.com/user-attachments/assets/d2bb2b91-89f6-430b-8d6a-a52563cbe1e1" />
<p> </p>

- **Métricas em Tempo Real:** Cartões exibem o total de tipos, como no exemplo: (22) itens em estoque (1.532), baixo estoque (5) e indisponíveis (2).
- **Busca e Categorias:** Uma barra de pesquisa textual atua em conjunto com abas de filtros rápidos para segmentar os componentes.
- **Cards de Itens:** Cada bloco exibe o nome, a descrição técnica, a quantidade, a localização física exata e uma barra gráfica de progresso do estoque.
- 
## 🛠️ Tecnologias Utilizadas

- **HTML5:** Estruturação semântica da interface, menus e janelas modais.
- **CSS3:** Design responsivo via Grid/Flexbox e estilização condicional para os status de criticidade.
- **JavaScript:** Lógica em memória para busca reativa, manipulação do DOM e gerenciamento de estado do inventário.

## 📁 Estrutura de Dados do Inventário

Os componentes estão mapeados internamente sob a seguinte estrutura de objetos JSON:

```javascript
{
  nome: 'Arduino Uno',
  categoria: 'Microcontroladores',
  desc: 'Microcontrolador ATmega328P, 14 I/O digitais',
  qtd: 12,
  max: 20,
  local: 'Prateleira D1, Gaveta 1',
  status: 'disponivel' // Opções: disponivel | baixo | indisponivel
}
