# Azure_Vision

## Detectar Rostos no Vision Studio

Soluções de visão frequentemente requerem IA para detectar rostos humanos. Suponha que a fictícia empresa de varejo Northwind Traders deseja localizar onde os clientes estão em uma loja para melhor atendê-los. Uma maneira de fazer isso é determinar se há rostos nas imagens e, se houver, retornar as coordenadas da caixa delimitadora que mostram sua localização.

Para testar as capacidades de detecção de rostos do serviço Azure AI Face, você usará o Azure Vision Studio. Esta é uma plataforma baseada em UI que permite explorar os recursos de visão da Azure AI sem a necessidade de escrever código.

### Criar um Recurso de Serviços de IA da Azure

Você pode usar o serviço Azure AI Face com um recurso de serviços de IA da Azure. Se ainda não o fez, crie um recurso de serviços de IA da Azure em sua assinatura Azure.

Em outra guia do navegador, abra o portal Azure em [https://portal.azure.com](https://portal.azure.com), faça login com a conta Microsoft associada à sua assinatura Azure.

Clique no botão ＋Criar um recurso e pesquise por Serviços de IA da Azure. Selecione criar um plano de serviços de IA da Azure. Você será levado a uma página para criar um recurso de serviços de IA da Azure. Configure-o com as seguintes configurações:
- Assinatura: Sua assinatura Azure.
- Grupo de recursos: Selecione ou crie um grupo de recursos com um nome exclusivo.
- Região: Leste dos EUA.
- Nome: Insira um nome exclusivo.
- Nível de Preço: Standard S0.
- Ao marcar esta caixa, reconheço que li e compreendi todos os termos abaixo: Selecionado.
Selecione Revisar + criar e, em seguida, Criar e aguarde o término da implantação.
## Conectar seu recurso de serviço Azure AI ao Vision Studio

A seguir, conecte o recurso de serviços Azure AI que você provisionou acima ao Vision Studio.

Em outra guia do navegador, acesse o Vision Studio em [https://portal.vision.cognitive.azure.com](https://portal.vision.cognitive.azure.com).

Faça login com sua conta e certifique-se de estar usando o mesmo diretório onde você criou seu recurso de serviços Azure AI.

Na página inicial do Vision Studio, selecione Visualizar todos os recursos sob o título Começando com Visão.

## Selecionar um recurso para trabalhar

Na página Selecionar um recurso para trabalhar, passe o cursor do mouse sobre o recurso que você criou acima na lista e, em seguida, marque a caixa à esquerda do nome do recurso e selecione Selecionar como recurso padrão.

Nota: Se o seu recurso não estiver listado, pode ser necessário atualizar a página.

A caixa de diálogo Selecionar um recurso para trabalhar é exibida com o recurso de Serviços Cognitivos cog-ms-learn-vision-SUFFIX destacado e marcado. O botão Selecionar como recurso padrão está destacado.

Feche a página de configurações selecionando o “x” no canto superior direito da tela.

## Detectar faces no Vision Studio

Em um navegador da web, acesse o Vision Studio em [https://portal.vision.cognitive.azure.com](https://portal.vision.cognitive.azure.com).

Na página inicial Começando com Visão, selecione a guia Rosto e depois selecione o azulejo Detectar Rostos em uma imagem.

Sob o subtítulo Experimente, reconheça a política de uso do recurso lendo e marcando a caixa.

Selecione cada uma das imagens de exemplo e observe os dados de detecção de rosto que são retornados.

Agora vamos tentar com algumas de nossas próprias imagens. Selecione [https://aka.ms/mslearn-detect-faces](https://aka.ms/mslearn-detect-faces) para baixar detect-faces.zip. Em seguida, abra a pasta no seu computador.

Localize o arquivo chamado store-camera-1.jpg; que contém a seguinte imagem:
