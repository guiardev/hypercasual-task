# Hypercasual

O jogo hypercasuals para celular no estilo corrida infinita com obstáculos e moedas e power ups.

<h2>Sumario</h2>
    <ol>
        <li><h4><a href="#C1">Menu Game</a></h4></li>
        <li><h4><a href="#C2">Controler player touch</a></h4></li>
        <li><h4><a href="#C3">Moedas</a></h4></li>
        <li><h4><a href="#C4">Obstáculos</a></h4></li>
        <li><h4><a href="#C5">Gameover</a></h4></li>
        <li><h4><a href="#C6">PowerUps</a></h4></li>
        <li><h4><a href="#C7">Animation</a></h4></li>
        <li><h4><a href="#C8">Level Manager</a></h4></li>
        <li><h4><a href="#C9">Level Manager Pieces</a></h4></li>
        <li><h4><a href="#C10">VFX and Particulas</a></h4></li>
    </ol>

<h1 id="C1">Menu Game</h1>

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

<h1 id="C2">Controler player touch</h1>

<h3>PlayerController</h3>

+ O script playerController vai cuidar toda configurações do player como animação e lerp e limites e também VFX, e o script bounceHelper fazer animação do player utilizando biblioteca DG.Tweening.

<h3>TouchController</h3>

+ O TouchController vai ser responsável pela movimentação segurando o clique do mouse no smartphone com toque do dedo do jogador, o player vai seguir game objeto positionController.

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_playerController_bounceHelper_SphereCollider.png" width="490" height="700"/></td>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_TouchController.png" width="495" height="90"/></td>
    </tr>
</table>

<h1 id="C3">Moedas</h1>

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

<h1 id="C4">Obstáculos</h1>

<h3>Enemy_MovimentHelper</h3>

+ O jogo vai ter obstáculos que vão se movimentar de um lado para outro seguindo objectos A e B, se o jogador encostar nos obstáculos da gameover.

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_Death.gif" width="450" height="650"/></td>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Enemy_MovimentHelper.png" width="480" height="300"/></td>
    </tr>
</table>

<h1 id="C5">Gameover</h1>

<h3>BtnRestart</h3>

+ A tela gameover vai estar com as mesmas objectos como BG tem imagem que escurece tela e botão restart.

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_Death.gif" width="450" height="650"/></td>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_BtnRestart.png" width="480" height="500"/></td>
    </tr>
</table>

<h1 id="C6">PowerUps</h1>

<ol>

<li><h3>PowerUp Coins</h3></li>

+ Quando o powerUp coins for ativado as moedas do jogo seguir personagem em um distância por uns segundos. O script do PowerUpCoin herda todas variáveis e classe PowerBase e BoxCollider ativado Trigger.

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
    
<h1 id="C7">Animation</h1>

<h3>Animator</h3>

+ O animador tem 3 parâmetros Idle quando personagem estiver parado, Run quando player estiver correto e Dead quando jogador perder o jogo.

<td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Animator.png" width="1100" height="340"/></td>

<h3>Animator Manager</h3>

+ O script AnimatorManager vai administrar animações do personagem.

<td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_AnimatorManager.png" width="480" height="350"/></td>

<h1 id="C8">Level Manager</h1>

<h3>Level Manager</h3>

 + O script level manager vai gerenciar as peças que vai montar a fase, a variável lista levelPieceBasedSetups que vai carregar os scripts configurações do level o script que vai esta lista vai ser um tipo scriptable, 
que vai estar todas as configurações das peças e definindo que tipo de peças vai esta no cenário.

+ Escalando objetos usando corrotinas assim as peças vão ser montadas aos poucos, a variável scaleDuration e a scaleTimeBetweenPieces que vai definir o tempo que as peças vão ser montadas.

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

<h1 id="C9">Level Manager Pieces</h1>

<h3>Piece 01 Start</h3>

+ Peça inicial que o jogo começa quando é criado o cenário.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Piece_01_Start.png" width="580" height="570"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Piece_01_Start_levelpieceBase_ColorChange.png" width="480" height="322"/></td>
    </tr>
</table>

<h3>Piece 01 End</h3>

+ Peça que vai ficar no final do jogo.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Piece_01_End.png" width="580" height="570"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Piece_01_End_levelpieceBase_ColorChange.png" width="480" height="322"/></td>
    </tr>
</table>

<h3>Piece 02 Coins e Piece 03 Coins</h3>

+ Peça que vai esta com moedas do jogo.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Piece_02_Coins.png" width="580" height="570"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Piece_03_Coins.png" width="580" height="570"/></td>
    </tr>
</table>

<h3>Scripts LevelPieceBase ColorChange, piece 2 e 3</h3>

+ O script LevelPieceBase vai cuidar onde vão começar monta peça que vai ficar atrás. E o ColorChange vai gerenciar as cores da peça.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Piece_02_Coins_LevelPieceBase_ColorChange.png" width="480" height="322"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Piece_03_Coins_LevelPieceBase_ColorChange.png" width="480" height="322"/></td>
    </tr>
</table>

<h3>Piece 04 Enemy e Piece 05 Enemy</h3>

+ Peça que vai estar com moedas e obstáculo do jogo.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Piece_04_Enemy.png" width="580" height="570"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Piece_05_Enemy.png" width="580" height="570"/></td>
    </tr>
</table>

<h3>Scripts LevelPieceBase ColorChange, piece 4 e 5</h3>

+ O script LevelPieceBase vai cuidar onde vão começar monta peça que vai ficar atrás. E o ColorChange vai gerenciar as cores da peça.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Piece_04_Enemy_LevelPieceBase_ColorChange.png" width="480" height="322"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Piece_05_Enemy_LevelPieceBase_ColorChange.png" width="480" height="322"/></td>
    </tr>
</table>

<h1 id="C10">VFX and Particulas</h1>

<h3>TrailRenderer</h3>

 + Trail vai criar um rastros no personagem quando ele estiver movimentando.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_menu.gif" width="450" height="650"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_TrailRenderer.png" width="480" height="650"/></td>
    </tr>
</table>

<h3>LineRenderer</h3>

+ A LineRenderer vai criar um line que traçada duas cilindro.

<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_LineRenderer.png" width="650" height="480"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_LineRendererObject.png" width="490" height="800"/></td>
    </tr>
</table>

<h3>Script LineRenderer</h3>

+ O script vai configurar onde posição dos pontos da linha onde elas vão passar e variável positions e lista que pode vários objetos onde a linha vai passar.

<img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Script_LineRenderer.png" width="490" height="161"/>

<h3>ItemCollectableCoin</h3>

+ O script ItemCollectableCoin vai cudar das configurações das moedas e efeitos delas.

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_coins.gif" width="450" height="650"/></td>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_SphereCollider_ItemCollectableCoin.png" width="495" height="430"/></td>
    </tr>
</table>

<h3>Particle System Coins</h3>

+ O particle system coins vai ser ativado quando o player pegar as moedas e vai desaparecer por uns segundos.

<table>
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_ParticleSystem_Coins_Emission.png" width="450" height="590"/></td>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_ParticleSystem_Coins_Shape..png" width="450" height="300"/></td>
    </tr>
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_ParticleSystem_Coins_Collision..png" width="450" height="330"/></td>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_ParticleSystem_Coins_Renderer..png" width="490" height="430"/></td>
    </tr>
</table>

<h3>Particle System VFX_Kill</h3>

+ O Particle System VFX_Kill vai aparecer quando o personagem morrer.

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_Death.gif" width="450" height="650"/></td> 
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_ParticleSystem_VFXKill_Emission.png" width="490" height="550"/></td>
    </tr>
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_ParticleSystem_VFXKill_Shape_Size-over-Lifetime.png" width="492" height="442"/></td>  
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_ParticleSystem_VFXKill_Renderer..png" width="490" height="440"/></td>
    </tr>
</table>
