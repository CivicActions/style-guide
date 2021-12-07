<style>
 
  /**** SWATCH STYLES (individual) ****/
  
  body {
    --swatch-gap: 12px;
    --swatch-padding: 12px;
    --swatch-font-size: 12px;
    /* width only if flex-grow disabled for swatch layout*/
    --swatch-width: 300px;
    --swatch-color-alt: #fff;
    --swatch-info-area-spacing: 10px;
    --swatch-hex-code-font-size: 18px;
    --swatch-hex-code-color: #fff;
    --swatch-grid-alt-width: 100px;
    --swatch-color-area-height: 140px;
    --swatch-info-area-height: auto;
  }
  .swatch--red-50 {
    --swatch-background-color: #d83933;
  }
  .swatch--red-40 {
    --swatch-alt-background-color: #e9695f;
  }
  .swatch--red-60 {
    --swatch-alt-background-color: #a23737;
  }
  .swatch--red-60 {
    --swatch-background-color: #a23737;
  }
  .swatch--red-50 {
    --swatch-alt-background-color: #d83933;
  }
  .swatch--red-70 {
    --swatch-alt-background-color: #6f3331;
  }
  .swatch--mint-40v {
    --swatch-background-color: #00a398;
  }
  .swatch--mint-30v {
    --swatch-alt-background-color: #1dc2ae;
  }
  .swatch--mint-50v {
    --swatch-alt-background-color: #008480;
  }
  .swatch--mint-60v {
    --swatch-background-color: #0f6460;
  }
  .swatch--mint-50v {
    --swatch-alt-background-color: #008480;
  }
  .swatch--mint-70v {
    --swatch-alt-background-color: #0b4b3f;
  }
 .swatch--gray-warm-4 {
    --swatch-background-color: #F5F5F0;
	  --swatch-hex-code-color: #111111;
  }
 .swatch--gray-90 {
    --swatch-background-color: #1b1b1b;
  }
.swatch--gray-50 {
    --swatch-background-color: #757575;
  }

  /**** SWATCH STYLES (general) ****/
  
  .swatch-grid {
    display: flex;
    flex-wrap: wrap;
    gap: var(--swatch-gap, 12px);
  }
  .swatch {
    /* flex: 1 1 0;  remove this and the swatches will wrap onto the next line */
    position: relative;
    display: grid;
    grid-template-rows: var(--swatch-color-area-height, 100px) var(--swatch-info-area-height, auto);
    width: var(--swatch-width, 300px);
    box-shadow: 0px 5px 20px rgba(128, 128, 128, 0.1);
    transition: 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    font-size: var(--swatch-font-size);
    color: var(--swatch-color);
    background-color: var(--swatch-background-color);
    overflow: hidden;
  }
  .swatch:hover {
    box-shadow: 0 8px 20px rgba(128, 128, 128, 0.12);
  }
  .swatch__hex-code {
    position: absolute;
    left: 20px;
    top: 20px;
    font-size: var(--swatch-hex-code-font-size, var(--swatch-font-size));
    color: var(--swatch-hex-code-color, var(--swatch-color-alt));
    font-weight: 700;
    text-transform: uppercase;
  }
  .swatch__color-area {
    position: relative;
  }
  .swatch-grid--alt {
    position: absolute;
    right: calc(var(--swatch-grid-alt-width, 100px) * -1); /* to hide off canvas initially */
    width: var(--swatch-grid-alt-width, 100px);
    display: flex;
    flex-direction: column;
    height: 100%;
    transition: 0.2s ease; /* handles mouse-out */
  }
  .swatch:hover .swatch-grid--alt {
    right: 0;
    transition: 0.2s ease;
  }
  .swatch--alt {
    flex-grow: 1;
    display: flex;
    justify-content: center;
    align-items: center;
    color: var(--swatch-alt-color, var(--swatch-color-alt));
    background-color: var(--swatch-alt-background-color);
  }
  .swatch__info-area {
    background-color: white;
    padding: var(--swatch-padding, 12px) var(--swatch-padding, 12px) calc(var(--swatch-padding, 12px) - var(--swatch-info-area-spacing, 6px)) var(--swatch-padding, 12px);

  }
  .swatch__info-area > * {
    margin-bottom: var(--swatch-info-area-spacing, 6px);
  }
  .swatch__importance {
    color: gray;
  }

  /**** PAGE STYLES ****/

  body {
    background: #fbfbfb;
    color: #333;
  }

  .main {
    margin: 4em auto 0;
    max-width: 800px;
  }

  .headers {
    margin: 60px 0 20px;
  }
  .headers h1 {
    margin: 10px 0;
    color: #333;
  }
  .headers h2 {
    color: #999;
    line-height: 1.5;
    padding-bottom: 0.5em;
  }
</style>

<article class="main">
  <section class="color-topic-1">
    <div class="headers">
      <h1>Colors</h1>
	    <h2>Color palette</h2>
    </div>
    <ul class="swatch-grid" aria-label="color swatches">

      <li class="swatch swatch--red-50" aria-label="red-50 swatch">
        <div class="swatch__color-area">
          <p class="swatch__hex-code" aria-label="primary hex code">#d83933</p>
          <ul class="swatch-grid--alt">
            <li class="swatch--alt swatch--red-40" aria-label="red-40">
              <p class="swatch__hex-code--alt">#e9695f</p>
            </li>
            <li class="swatch--alt swatch--red-60" aria-label="red-60">
              <p class="swatch__hex-code--alt">#a23737</p>
            </li>
          </ul>
        </div>
        <div class="swatch__info-area">
          <p class="swatch__name" aria-label="color name">Red-50</p>
          <p class="swatch__importance" aria-label="color importance">Primary</p>
        </div>
      </li>
			
			<li class="swatch swatch--red-60" aria-label="red-60 swatch">
        <div class="swatch__color-area">
          <p class="swatch__hex-code" aria-label="primary hex code">#a23737</p>
          <ul class="swatch-grid--alt">
            <li class="swatch--alt swatch--red-50" aria-label="red-50">
              <p class="swatch__hex-code--alt">#d83933</p>
            </li>
            <li class="swatch--alt swatch--red-70" aria-label="red-70">
              <p class="swatch__hex-code--alt">#6f3331</p>
            </li>
          </ul>
        </div>
        <div class="swatch__info-area">
          <p class="swatch__name" aria-label="color name">Red-60</p>
          <p class="swatch__importance" aria-label="color importance">Secondary</p>
        </div>
      </li>

      <li class="swatch swatch--mint-40v" aria-label="mint-40 vivid swatch">
        <div class="swatch__color-area">
          <p class="swatch__hex-code" aria-label="primary hex code">#00a398</p>
          <ul class="swatch-grid--alt">
            <li class="swatch--alt swatch--mint-30v" aria-label="mint-30 vivid swatch">
              <p class="swatch__hex-code--alt">#1dc2ae</p>
            </li>
            <li class="swatch--alt swatch--mint-50v" aria-label="mint-50 vivid swatch">
              <p class="swatch__hex-code--alt">#008480</p>
            </li>
          </ul>
        </div>
        <div class="swatch__info-area">
          <p class="swatch__name" aria-label="color name">Mint Cool-40v</p>
          <p class="swatch__importance" aria-label="color importance">Primary</p>
        </div>
      </li>
			
			<li class="swatch swatch--mint-60v" aria-label="mint-60 vivid swatch">
        <div class="swatch__color-area">
          <p class="swatch__hex-code" aria-label="primary hex code">#0f6460</p>
          <ul class="swatch-grid--alt">
            <li class="swatch--alt swatch--mint-50v" aria-label="mint-50 vivid swatch">
              <p class="swatch__hex-code--alt">#008480</p>
            </li>
            <li class="swatch--alt swatch--mint-70v" aria-label="mint-70 vivid swatch">
              <p class="swatch__hex-code--alt">#0b4b3f</p>
            </li>
          </ul>
        </div>
        <div class="swatch__info-area">
          <p class="swatch__name" aria-label="color name">Mint Cool-60v</p>
          <p class="swatch__importance" aria-label="color importance">Secondary</p>
        </div>
      </li>
			
			<li class="swatch swatch--gray-warm-4" aria-label="gray-warm-4 swatch">
        <div class="swatch__color-area">
          <p class="swatch__hex-code" aria-label="primary hex code">#F5F5F0</p>
          <ul class="swatch-grid--alt">
     
          </ul>
        </div>
        <div class="swatch__info-area">
          <p class="swatch__name" aria-label="color name">gray-warm-4</p>
          <p class="swatch__importance" aria-label="color importance">Neutral</p>
        </div>
      </li>
			
						<li class="swatch swatch--gray-90" aria-label="gray-90 swatch">
        <div class="swatch__color-area">
          <p class="swatch__hex-code" aria-label="primary hex code">#1b1b1b</p>
          <ul class="swatch-grid--alt">
     
          </ul>
        </div>
        <div class="swatch__info-area">
          <p class="swatch__name" aria-label="color name">gray-90</p>
          <p class="swatch__importance" aria-label="color importance">Neutral</p>
        </div>
      </li>
			
			<li class="swatch swatch--gray-50" aria-label="gray-50 swatch">
        <div class="swatch__color-area">
          <p class="swatch__hex-code" aria-label="primary hex code">#757575</p>
          <ul class="swatch-grid--alt">
     
          </ul>
        </div>
        <div class="swatch__info-area">
          <p class="swatch__name" aria-label="color name">gray-50</p>
          <p class="swatch__importance" aria-label="color importance">Neutral</p>
        </div>
      </li>
      
    </ul>
  </section>
<section class="color-topic-2">
	<h2>Color accessibility</h2>
</section>
</article>
