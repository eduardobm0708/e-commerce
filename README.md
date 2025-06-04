# Página de Produto E-commerce

Este projeto implementa uma página de produto de e-commerce utilizando React e Tailwind CSS, conforme as especificações solicitadas.

## Funcionalidades Implementadas

- **Galeria de Imagens**: Uma imagem principal que ocupa cerca de 35% da tela, com miniaturas abaixo que, ao serem clicadas, alteram a imagem principal.
- **Informações do Produto**: Título, descrição e preço do produto com formatação adequada.
- **Seletores de Variantes**: Campos dinâmicos para seleção de tamanho e cor, gerados a partir de arrays de dados.
- **Consulta de CEP**: Campo que formata e verifica o CEP digitado, exibindo o endereço completo quando o CEP existe, utilizando a API ViaCEP.
- **Persistência de Dados**: Todas as ações do usuário são salvas no localStorage e mantidas por 15 minutos, mesmo após a atualização da página.

## Tecnologias Utilizadas

- React com TypeScript
- Tailwind CSS para estilização
- Hooks personalizados para gerenciamento de estado e persistência
- Integração com API ViaCEP

## Como Executar o Projeto

1. Clone o repositório
2. Instale as dependências:
   ```
   cd my-ecommerce
   pnpm install
   ```
3. Execute o servidor de desenvolvimento:
   ```
   pnpm run dev
   ```
4. Acesse o projeto em seu navegador: `http://localhost:5173`

## Estrutura do Projeto

- `src/components/`: Componentes React da aplicação
  - `ProductPage.tsx`: Componente principal que organiza a página
  - `ImageGallery.tsx`: Galeria de imagens com miniaturas
  - `ProductInfo.tsx`: Informações do produto (título, preço)
  - `VariantSelector.tsx`: Seletores dinâmicos de variantes
  - `ShippingCalculator.tsx`: Consulta de CEP e exibição de endereço
- `src/hooks/`: Hooks personalizados
  - `useLocalStorageCleanup.tsx`: Hook para gerenciar a expiração de dados no localStorage

## Observações

- O projeto foi desenvolvido com foco em responsividade, funcionando bem em dispositivos móveis e desktop.
- A persistência de dados é limitada a 15 minutos conforme solicitado, com limpeza automática após esse período.
- Os seletores de variantes são gerados dinamicamente a partir de arrays de dados, permitindo fácil manutenção e expansão.
