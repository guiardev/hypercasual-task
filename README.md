# Menu Game

O menu do jogo vai ter só botão play quando o jogador clicar nesse o jogo começa.

<h3>StarScream</h3>

+ No canvas do menu vai estar com StarScream que vai esta como BG tem imagem que escurece tela e botão play.

<h3>BG_RectTransform_Image e BtnPlay</h3>

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_menu.gif" width="450" height="650"/></td>
      <td>
          <img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_BG_RectTransform_Image.png" width="470" height="400"/>
          <img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_BtnPlay.png" width="470" height="160"/>
      </td>
    </tr>
</table>

# Controler player touch

<h3>playerController</h3>

+ O script playerController vai cuidar toda configurações do player como animação e lerp e limites e também VFX, e o script bounceHelper fazer animação do player utilizando biblioteca DG.Tweening.

<h3>TouchController</h3>

+ O TouchController vai ser responsável pela movimentação segurando o clique do mouse no smartphone com toque do dedo do jogador, o player vai seguir game objeto positionController.

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_playerController_bounceHelper_SphereCollider.png" width="490" height="700"/></td>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_TouchController.png" width="495" height="90"/></td>
    </tr>
</table>

# Moedas

<h3>ItemCollectableCoin</h3>

+ As moedas do jogo vão ser criadas redondamente no cenário e quando a personagem encostar nela vai ela vai ser destruída e vai aparecer um efeito em VFX com várias moedas caindo no chão.

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_coins.gif" width="450" height="650"/></td>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_SphereCollider_ItemCollectableCoin.png" width="495" height="430"/></td>
    </tr>
</table>

<h3>CoinCollector</h3>

+ No player vai ter um gameobject chamado CoinCollector que vai Sphere collider vai ser responsável pelas coleta das moedas e script itemCollectableCoin administrar os comportamento das moedas.

<h3>CoinsAnimationManager</h3>

+ O script CoinsAnimationManager vai cuidar de animações quando o player pegar elas, e variável List que vai acumular todas as moedas do jogo quando game estiverem ligados.

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_CoinCollector.png" width="495" height="350"/></td>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_CoinsAnimationManager.png" width="495" height="209"/></td>
    </tr>
</table>

# obstáculos

<h3>Enemy_MovimentHelper</h3>

+ O jogo vai ter obstáculos que vão se movimentar de um lado para outro seguindo objectos A e B, se o jogador encostar nos obstáculos da gameover.

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_Death.gif" width="450" height="650"/></td>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Enemy_MovimentHelper.png" width="480" height="300"/></td>
    </tr>
</table>

# gameover

<h3>BtnRestart</h3>

+ A tela gameover vai estar com as mesmas objectos como BG tem imagem que escurece tela e botão restart.

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_Death.gif" width="450" height="650"/></td>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_BtnRestart.png" width="480" height="500"/></td>
    </tr>
</table>

# PowerUps

<ol>

<li><h3>PowerUp Coins</h3></li>

+ Quando o powerUp coins for ativado as moedas do jogo seguir personagem em um distância por uns segundos. O script do PowerUpCoin herda todas variáveis e classe PowerBase e BoxCollider ativado Trigger.</br>

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_PowerUpCoins.gif" width="450" height="650"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_BoxCollider_PowerUpCoin.png" width="480" height="380"/></td>
    </tr>
</table>

<h3>CoinCollector</h3>
    
+ Quando o player pegar power up coins objecto que está no personagem é chamado CoinCollector vai aumentar o SpheneCollider que está com Trigger ativado.
    
<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_CoinCollector_active.png" width="600" height="550"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_CoinCollector.png" width="480" height="350"/></td>
    </tr>
</table>
    
<li><h3>PowerUp Speed</h3></li>

+ O power up speed vai aumentar a velocidade do player por um segundos.
    
<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_PowerUpSpeed.gif" width="450" height="650"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_BoxCollider_PowerUpSpeedUp.png" width="480" height="350"/></td>
    </tr>
</table>

<li><h3>PowerUp Invencivel</h3></li>

+ O power up invincible vai deixar o personagem invencível e não vai morrer de bater no obstáculo por uns segundos.
    
<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_PowerUpInvincible.gif" width="450" height="650"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_BoxCollider_PowerUpInvincible.png" width="480" height="350"/></td>
    </tr>
</table>
    
<li><h3>PowerUp Fly</h3></li>

+ O power up height vai fazer o player voar por segundos e depois voltar para o chão. 
    
<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_PowerUpHeight.gif" width="450" height="650"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_BoxCollider_PowerUpHeight.png" width="480" height="350"/></td>
    </tr>
</table>

</ol>
    
# Animation

<h3>Animator</h3>

+ O animador tem 3 parâmetros Idle quando personagem estiver parado, Run quando player estiver correto e Dead quando jogador perder o jogo.

<td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Animator.png" width="1100" height="340"/></td>

<h3>Animator Manager</h3>

+ O script AnimatorManager vai administrar animações do personagem.

<td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_AnimatorManager.png" width="480" height="350"/></td>

# Level Manager

<h3>Level Manager</h3>

 + O script level manager vai gerenciar as peças que vai montar a fase, a variável lista levelPieceBasedSetups que vai carregar os scripts configurações do level o script que vai esta lista vai ser um tipo scriptable, 
que vai estar todas as configurações das peças e definindo que tipo de peças vai esta no celario.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/record_LevelManager.gif" width="530" height="550"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_LevelManager.png" width="480" height="350"/></td>
    </tr>
</table>

<h3>Scriptable LevelPieceBasedSetup e ArtManager</h3>

 + O scriptable level 1 e todas configurações vão criar a fase do jogo. O script ArtManager vai responsavel colocar arte do cenário no seus lugares.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_LevelPieceBasedSetup.png" width="480" height="470"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_ArtManager.png" width="480" height="220"/></td>
    </tr>
</table>

<h3>Rondom Cores</h3>

 + O script color manager vai randomizando cores das peças e os materiais do level.

<img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_ColorManager.png" width="480" height="450"/>

# poling game

<h3>corotinas</h3>

<h3>tweens</h3>

# VFX and Particulas.
