<script>
  import svelteLogo from "../public/logo.png";
  import toyota from "../public/Toyota.jpg";
  import wasserstoff from "../public/wasserstoff.jpg"
  import hydrogene from "../public/hydrogene.jpg"
  import hydroVert from "../public/Hydrogene-vert.jpg"
    import Counter from "./lib/Header.svelte";
  import LocomotiveScroll from "locomotive-scroll";
</script>

<main>
  <div class="headerTitle">
    <a href="#" target="_blank" rel="noreferrer">
      <img src={svelteLogo} class="logo svelte" alt="Svelte Logo" />
      <h1 class="title">Hydrogène</h1>
    </a>
  </div>
  <div>
    <h2 class="subtitle">Qu'est-ce que l’hydrogène</h2>
    <p class="subtitle">
      L'hydrogène est la plus petite molécule qui existe dans la nature. Elle se compose de deux atomes identiques combinant simplement un proton et un électron. L'atome d'hydrogène est si petit qu'il se faufile partout. La combustion d'hydrogène produit 3 fois plus d'énergie que l'essence. Il est présent dans l'eau et dans beaucoup de gaz.
    </p>
    <h2 class="subtitle">Comment produire de l’hydrogène</h2>
    <p class="subtitle">
      Pour produire de l'hydrogène, on utilise principalement le gaz naturel CH<sub>4</sub>. À la fin de ce processus, on obtient du CO<sub>2</sub> qui contribue à l'effet de serre. Une autre solution est d'utiliser une électrolyse de l'eau. Le principe est que, à l'aide de deux électrodes, l'anode et la cathode, on fait passer du courant électrique dans l'eau, séparant ainsi l'hydrogène de l'oxygène.
    </p>
  </div>

  <div class="grid">
    <div class="card">
      <img src="{toyota}" alt="Image 1">
      <div class="card-overlay">
        <h3>Premièrement</h3>
        <p>Les moteurs à hydrogène peuvent être une solution intéressante pour de
          nombreuses raisons. Tout d'abord, l'hydrogène est une source d'énergie
          propre et renouvelable qui ne produit pas de gaz à effet de serre
          lorsqu'elle est utilisée dans un moteur. Cela peut contribuer à
          réduire l'impact de l'utilisation de véhicules sur l'environnement et
          à lutter contre le changement climatique.</p>
      </div>
    </div>
    <div class="card">
      <img src="{hydroVert}" alt="Image 2">
      <div class="card-overlay">
        <h3>Deuxièmement</h3>
        <p>l'hydrogène peut être produit à partir de différentes
          sources d'énergie renouvelables, telles que l'énergie solaire ou
          éolienne. Cela signifie que les moteurs à hydrogène peuvent
          fonctionner sans dépendre des combustibles fossiles, qui sont limités
          et non durables.</p>
      </div>
    </div>
    <div class="card">
      <img src="{wasserstoff}" alt="Image 3">
      <div class="card-overlay">
        <h3>Troisièmement</h3>
        <p>Les moteurs à hydrogène peuvent être plus efficaces et plus
          performants que les moteurs à essence ou diesel. Ils peuvent offrir
          des performances supérieures en termes de puissance, de vitesse et
          d'autonomie, ce qui peut être attrayant pour les conducteurs.</p>
      </div>
    </div>
    <div class="card">
    <img src="{hydrogene}" alt="Image 4">
    <div class="card-overlay">
      <h3>En resumé</h3>
      <p>les moteurs à hydrogène sont une solution intéressante car
        ils peuvent contribuer à la protection de l'environnement, être
        alimentés par des sources d'énergie renouvelables et offrir des
        performances supérieures à celles des moteurs à essence ou diesel.</p>
    </div>
  </div>
  </div>
<!--
  <div class="figuresContainer">
    <div class="image-block" id="block_1">
      <div>
        <h3>Premièrement</h3>
        <p>
          Les moteurs à hydrogène peuvent être une solution intéressante pour de
          nombreuses raisons. Tout d'abord, l'hydrogène est une source d'énergie
          propre et renouvelable qui ne produit pas de gaz à effet de serre
          lorsqu'elle est utilisée dans un moteur. Cela peut contribuer à
          réduire l'impact de l'utilisation de véhicules sur l'environnement et
          à lutter contre le changement climatique.
        </p>
      </div>
    </div>

    <figure class="image-block" id="block_2">
      <figcaption>
        <h3>Deuxièmement</h3>
        <p>
          Deuxièmement, l'hydrogène peut être produit à partir de différentes
          sources d'énergie renouvelables, telles que l'énergie solaire ou
          éolienne. Cela signifie que les moteurs à hydrogène peuvent
          fonctionner sans dépendre des combustibles fossiles, qui sont limités
          et non durables.
        </p>
      </figcaption>
    </figure>

    <figure class="image-block" id="block_3">
      <figcaption>
        <h3>Troisièmement</h3>
        <p>
          Les moteurs à hydrogène peuvent être plus efficaces et plus
          performants que les moteurs à essence ou diesel. Ils peuvent offrir
          des performances supérieures en termes de puissance, de vitesse et
          d'autonomie, ce qui peut être attrayant pour les conducteurs.
        </p>
      </figcaption>
    </figure>

    <figure class="image-block" id="block_4">
      <figcaption>
        <h3>En resumé</h3>
        <p>
          En résumé, les moteurs à hydrogène sont une solution intéressante car
          ils peuvent contribuer à la protection de l'environnement, être
          alimentés par des sources d'énergie renouvelables et offrir des
          performances supérieures à celles des moteurs à essence ou diesel.
        </p>
      </figcaption>
    </figure>
  </div>
  -->
</main>

<style>
  .subtitle {
    color: #1a1a1a;
  }
  .logo {
    height: 6em;
    padding: 1.5em;

    float: left;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  @keyframes scale {
    from {
      transform: scale(0) rotate(180deg);
    }
    to {
      transform: scale(1) rotate(0deg);
    }
  }

  .headerTitle {
    display: inline-block;
    animatiomn: scale 400s linear alternate;
    transition: all 500ms;
  }

  .title {
    float: right;
    color: #2a2a2a;
  }
  .headerTitle:hover{
    transition: all 500ms;
    filter: drop-shadow(0 0 2em #646cffaa);
  }
</style>
