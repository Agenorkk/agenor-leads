# Agenor Leads

Aplicativo web responsivo para pesquisar empresas mapeadas no OpenStreetMap e organizar oportunidades de venda de sites.

## Funcionalidades desta primeira versão
- Busca por cidade, estado e categoria usando Nominatim e Overpass API do OpenStreetMap.
- Resultados com fonte consultável; não cria nomes ou contatos fictícios.
- Cadastro e edição manual de leads, status do funil, responsável, valor e notas.
- Gerador de mensagem para revisar e enviar manualmente.
- Exportação de backup JSON e importação de JSON/CSV.
- Layout responsivo e suporte básico a instalação como PWA.

## Publicar gratuitamente com GitHub Pages
1. Abra **Settings** deste repositório.
2. Entre em **Pages**.
3. Em **Build and deployment**, selecione **Deploy from a branch**.
4. Escolha a branch **main** e a pasta **/(root)** e clique em **Save**.
5. Aguarde o GitHub gerar o endereço do site. Normalmente será `https://agenorkk.github.io/agenor-leads/`.

## Instalar no iPhone
Depois de publicar, abra o endereço no Safari, toque em **Compartilhar** e escolha **Adicionar à Tela de Início**.

## Limites importantes
- A busca depende da cobertura dos dados abertos no OpenStreetMap; nem toda empresa está cadastrada, e os dados podem estar incompletos/desatualizados.
- Faça pesquisas pequenas, uma cidade por vez. Nominatim e Overpass são serviços públicos com limites; não use para raspagem massiva nem faça pesquisas repetidas em alta frequência.
- Não há scraping do Google Maps nem disparo automático de WhatsApp.
- Os leads desta versão ficam no armazenamento local do navegador. Não existe ainda login, banco de dados compartilhado ou sincronização entre os quatro integrantes/dispositivos. Exporte backups regularmente.
- Antes de contatar uma empresa, confirme a informação e respeite solicitações para não receber mensagens.

## Arquitetura
HTML, CSS e JavaScript sem dependências de build, para facilitar manutenção e hospedagem estática.
