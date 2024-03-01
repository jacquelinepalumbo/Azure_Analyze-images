# Analyze images in Vision Studio

Understanding image content and context and extracting information from images.



3. **Ao marcar esta caixa, reconheço que li e entendi todos os termos abaixo**: _Selecionado_.
   
Selecione **Revisar** + **criar** e, em seguida, Criar e aguarde a conclusão da implantação.

## Conectar seu recurso de serviço de IA do Azure ao Vision Studio

Em seguida, conecte o recurso de serviços de IA do Azure provisionado acima ao Vision Studio.

1. Em outra guia do navegador, navegue até **o Vision Studio** em [https://portal.vision.cognitive.azure.com](https://portal.vision.cognitive.azure.com).

2. Entre com sua conta e verifique se você está usando o mesmo diretório em que criou seu recurso de serviços de IA do Azure.

3. Na home page do Vision Studio, selecione **Exibir todos os recursos** no cabeçalho **Introdução ao Vision**.

<img width="626" alt="image" src="https://github.com/jacquelinepalumbo/Azure_Detect-Faces/assets/119548193/5bb0961c-9003-4e29-872e-b7aae15e4fb5">

4. Na página **Selecione um recurso para trabalhar**, passe o cursor do mouse sobre o recurso criado acima na lista e marque a caixa à esquerda do nome do recurso e selecione **Selecionar como recurso padrão**.

<img width="933" alt="image" src="https://github.com/jacquelinepalumbo/Azure_Detect-Faces/assets/119548193/e6e8a1e0-ff03-4986-b6e1-a79d09d57481">

5. Feche a página de configurações selecionando o "x" no canto superior direito da tela.


## Gerar legendas para uma imagem

Agora você está pronto para usar o Vision Studio para analisar imagens tiradas por uma câmera na loja _Northwind Traders_.

Vejamos a funcionalidade de legendagem de imagem do Azure AI Vision. As legendas de imagem estão disponíveis por meio dos recursos **Legenda** e **Legendas densas**.

1. Em um navegador da Web, navegue até o [Vision Studio](https://portal.vision.cognitive.azure.com/gallery/featured).

2. Na página **inicial Introdução ao Vision**, selecione a guia **Análise de imagem** e selecione o bloco **Adicionar legendas a imagens**.

   <img width="388" alt="image" src="https://github.com/jacquelinepalumbo/Azure_Analyze-images/assets/119548193/6d9086e0-5183-46c9-9850-fe4ec7447e68">

3. No subtítulo **Experimentar**, reconheça a política de uso de recursos lendo e marcando a caixa.

4. Selecione [https://aka.ms/mslearn-images-for-analysis](https://aka.ms/mslearn-images-for-analysis) para baixar **image-analysis.zip**. Abra a pasta em seu computador e localize o arquivo chamado **store-camera-1.jpg**; que contém a seguinte imagem:

<img width="452" alt="image" src="https://github.com/jacquelinepalumbo/Azure_Analyze-images/assets/119548193/5b7000a6-2e67-4afd-a016-5473c679b189">

5. Carregue a imagem **store-camera-1.jpg** arrastando-a para a caixa **Arrastar e soltar arquivos aqui** ou navegando até ela em seu sistema de arquivos.

6. Observe o texto da legenda gerado, visível no painel **Atributos detectados** à direita da imagem.

A funcionalidade **Legenda** fornece uma única frase em inglês legível por humanos que descreve o conteúdo da imagem.

7. Em seguida, use a mesma imagem para executar **legendas densas**. Retorne à home page do **Vision Studio** e, como fez antes, selecione a guia **Análise de imagem** e, em seguida, selecione o bloco **Legenda densa**.

O recurso **Legendas densas** difere do recurso **Legenda** porque fornece várias legendas legíveis por humanos para uma imagem, uma descrevendo o conteúdo da imagem e outras, cada uma cobrindo os objetos essenciais detectados na imagem. Cada objeto detectado inclui uma caixa delimitadora, que define as coordenadas de pixel dentro da imagem associada ao objeto.

8. Passe o mouse sobre uma das legendas na lista **Atributos detectados** e observe o que acontece na imagem.

   <img width="566" alt="image" src="https://github.com/jacquelinepalumbo/Azure_Analyze-images/assets/119548193/de1af567-8b56-4d56-b04a-d8f61d05d1da">

   Mova o cursor do mouse sobre as outras legendas da lista e observe como a caixa delimitadora muda na imagem para realçar a parte da imagem usada para gerar a legenda.


# Marcação de imagens

O próximo recurso que você tentará é a funcionalidade **Extrair tags**. As tags de extração são baseadas em milhares de objetos reconhecíveis, incluindo seres vivos, cenários e ações.

1. Retorne à home page do Vision Studio e selecione o bloco **Extrair marcas comuns de imagens** na guia **Análise de imagem**.

2. Em **Escolha o modelo que você deseja experimentar**, deixe **Produto pré-criado versus modelo de intervalo selecionado**. 

Em **Escolha seu idiom**a, selecione **Inglês** ou um idioma de sua preferência.

3. Abra a pasta que contém as imagens que você baixou e localize o arquivo chamado **store-image-2.jpg**, que tem a seguinte aparência:
   <img width="448" alt="image" src="https://github.com/jacquelinepalumbo/Azure_Analyze-images/assets/119548193/610e8a50-1b01-411a-8fe4-bba03cbff0a9">


4. Carregue o arquivo **store-camera-2.jpg**.

5. Revise a lista de tags extraídas da imagem e a pontuação de confiança para cada uma no painel de atributos detectados. Aqui, o escore de confiança é a probabilidade de que o texto para o atributo detectado descreva o que realmente está na imagem. Observe na lista de tags que ela inclui não apenas objetos, mas ações, como _comprar, vender e ficar em pé_.

    <img width="653" alt="image" src="https://github.com/jacquelinepalumbo/Azure_Analyze-images/assets/119548193/04be6f74-c039-4abe-9ed1-45b58e15f276">


# Detecção de objetos

Nesta tarefa, você usa o recurso **de detecção de objeto** da análise de imagem. A detecção de objetos detecta e extrai caixas delimitadoras com base em milhares de objetos reconhecíveis e seres vivos.

1. Retorne à home page do Vision Studio e selecione o bloco **Detectar objetos comuns em imagens** na guia **Análise de imagem**.

2. Em **Escolha o modelo que você deseja experimentar**, deixe **Produto pré-criado versus modelo de intervalo selecionado**.

3. Abra a pasta que contém as imagens que você baixou e localize o arquivo chamado **store-camera-3.jpg**, que tem a seguinte aparência:

<img width="425" alt="image" src="https://github.com/jacquelinepalumbo/Azure_Analyze-images/assets/119548193/bb466996-c2ba-4647-9bf9-7d8484b213c6">


4. Carregue o arquivo **store-camera-3.jpg**.

5. Na caixa **Atributos detectados**, observe a lista de objetos detectados e suas pontuações de confiança.

6. Passe o cursor do mouse sobre os objetos na lista **Atributos detectados** para realçar a caixa delimitadora do objeto na imagem.

7. Mova o controle deslizante **Valor de limite** até que um valor de 70 seja exibido à direita do controle deslizante. Observe o que acontece com os objetos na lista. O controle deslizante de limite especifica que somente objetos identificados com uma pontuação de confiança ou probabilidade maior que o limite devem ser exibidos.


<img width="704" alt="image" src="https://github.com/jacquelinepalumbo/Azure_Analyze-images/assets/119548193/d5efe137-146d-4203-9186-8caf33764524">

<img width="757" alt="image" src="https://github.com/jacquelinepalumbo/Azure_Analyze-images/assets/119548193/92ce6c0a-d5b2-410b-80d7-4feac52eff17">

<img width="739" alt="image" src="https://github.com/jacquelinepalumbo/Azure_Analyze-images/assets/119548193/c24504bb-3bb7-4ef5-9355-53011c15aa19">

<img width="689" alt="image" src="https://github.com/jacquelinepalumbo/Azure_Analyze-images/assets/119548193/d01ffd5d-fd47-4d33-884f-229bbe4a17b2">


