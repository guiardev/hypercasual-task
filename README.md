# Menu Game

O menu do jogo vai ter só botão play quando o jogador clicar nesse o jogo começa.

No canvas do menu vai estar com StarScream que vai esta como BG tem imagem que escurece tela e botão play.

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

O script playerController vai cuidar toda configurações do player como animação e lerp e limites e também VFX, e o script bounceHelper fazer animação do player utilizando biblioteca DG.Tweening.

O TouchController vai ser responsável pela movimentação segurando o clique do mouse no smartphone com toque do dedo do jogador, o player vai seguir game objeto positionController.

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_playerController_bounceHelper_SphereCollider.png" width="490" height="700"/></td>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_TouchController.png" width="495" height="90"/></td>
    </tr>
</table>

# moedas

As moedas do jogo vão ser criadas redondamente no cenário e quando a personagem encostar nela vai ela vai ser destruída e vai aparecer um efeito em VFX com várias moedas caindo no chão.

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_coins.gif" width="450" height="650"/></td>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_SphereCollider_ItemCollectableCoin.png" width="495" height="430"/></td>
    </tr>
</table>

No player vai ter um gameobject chamado CoinCollector que vai Sphere collider vai ser responsável pelas coleta das moedas e script itemCollectableCoin administrar os comportamento das moedas.

<img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_CoinCollector.png" width="495" height="350"/>

# obstáculos

O jogo vai ter obstáculos que vão se movimentar de um lado para outro seguindo objectos A e B, se o jogador encostar nos obstáculos da gameover.

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_Death.gif" width="450" height="650"/></td>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_Enemy_MovimentHelper.png" width="480" height="300"/></td>
    </tr>
</table>

# gameover

A tela gameover vai estar com as mesmas objectos como BG tem imagem que escurece tela e botão restart.

<table border="0">
    <tr>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_Death.gif" width="450" height="650"/></td>
      <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_BtnRestart.png" width="480" height="500"/></td>
    </tr>
</table>

# PowerUps

<ol>
    
<li><h3>PowerUp Coins</h3></li>
    
Quando o powerUp coins for ativado as moedas do jogo seguir personagem em um distância por uns segundos. O script do PowerUpCoin herda todas variáveis e classe PowerBase e BoxCollider ativado Trigger.
        
<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/Records/Movie_PowerUpCoins.gif" width="450" height="650"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_BoxCollider_PowerUpCoin.png" width="480" height="380"/></td>
    </tr>
</table>
    
Quando o player pegar power up coins objecto que está no personagem é chamado CoinCollector vai aumentar o SpheneCollider que está com Trigger ativado.
    
<table border="0">
    <tr>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_CoinCollector_active.png" width="600" height="550"/></td>
        <td><img src="https://github.com/guiardev/hypercasual-task/blob/develop/Assets/imgs/img_CoinCollector.png" width="480" height="350"/></td>
    </tr>
</table>
    
<li><h3>PowerUp Speed</h3></li>

<li><h3>PowerUp Invencivel</h3></li>
    
<li><h3>PowerUp Fly</h3></li>

</ol>



    
# Animation

Animator manager

# Level Manager

level base

level manager

Rondom cores

# poling game

corotinas

tweens

# VFX and Particulas.
