<style>
#ca-important.clear-user-agent-styles table,
#ca-important.clear-user-agent-styles thead,
#ca-important.clear-user-agent-styles tbody,
#ca-important.clear-user-agent-styles tfoot,
#ca-important.clear-user-agent-styles tr,
#ca-important.clear-user-agent-styles th,
#ca-important.clear-user-agent-styles td {
    width: auto;
    height: auto;
    margin: 10px;
    padding: 6px;
    border: none !important;
    border-collapse: inherit !important;
    border-spacing: 0 !important;
    border-color: inherit !important;
    vertical-align: inherit;
    text-align: left;
    font-color: #1b1b1b;;
    font-weight: inherit;
    -webkit-border-horizontal-spacing: 0;
    -webkit-border-vertical-spacing: 0;
    background-color: initial;	
}
	
/**** SWATCH STYLES (individual) ****/
  body {
    --swatch-gap: 12px;
    --swatch-padding: 12px;
    --swatch-font-size: 12px;
    /* width only if flex-grow disabled for swatch layout*/
    --swatch-width: 1000px;
    --swatch-info-area-spacing: 10px;
    --swatch-hex-code-font-size: 18px;
    --swatch-name-font-size: 14px;
    --swatch-hex-code-color: #F5F5F0;
    --swatch-color-area-height: 140px;
    --swatch-info-area-height: auto;
    
    --swatch--gray-warm-4: #F5F5F0;
  }
  .swatch--red-50 {
    --swatch-background-color: #d83933;
  }
  .swatch--red-60 {
    --swatch-background-color: #a23737;
     --swatch-hex-code-color: #f5f5f0;
  }
  .swatch--mint-cool-40v {
    --swatch-background-color: #00a398;
  }
  .swatch--mint-cool-60v {
    --swatch-background-color: #0f6460;
  }
 .swatch--gray-warm-4 {
    --swatch-background-color: #F5F5F0;
	  --swatch-hex-code-color: #1b1b1b;
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
  .swatch__name {
    position: absolute;
    left: 20px;
    top: 10px;
    font-size: var(--swatch-hex-code-font-size, var(--swatch-font-size));
    color: var(--swatch-hex-code-color, var(--swatch-color-alt));
    font-weight: 700;
  }
.swatch__hex-code {
    position: absolute;
    left: 20px;
    top: 35px;
    font-size: var(--swatch-name-font-size, var(--swatch-font-size));
    color: var(--swatch-hex-code-color, var(--swatch-color-alt));
    font-weight: 400;
    text-transform: uppercase;
  }
  .swatch__color-area {
    position: relative;
  }
  .swatch__color-area--inverted {
    color: var(--swatch--gray-warm-4);
  }
  .swatch__info-area {
    background-color: white;
    padding: var(--swatch-padding, 12px) var(--swatch-padding, 12px) calc(var(--swatch-padding, 12px) - var(--swatch-info-area-spacing, 6px)) var(--swatch-padding, 12px);

  }
  .swatch__info-area > * {
    margin-bottom: var(--swatch-info-area-spacing, 6px);
  }
  .swatch__common-name {
    color: #757575;
  }
.contrast-table {
  position: absolute;
  right: calc(var(--swatch-gap, 12px) * 2);
  top: 48px;
  min-width: 300px;
}
#ca-important .contrast-table__row td {
  border-bottom: 1px solid #1b1b1b !important;
}
#ca-important .contrast-table__row--last td {
  border-bottom: 0px solid !important;
}
.swatch__color-area--inverted .contrast-table__row td {
  border-color: var(--swatch--gray-warm-4) !important;
}
.u-hide {
  visibility: hidden;
}

.text-color-1 {
  color: #F5F5F0; /*gray-warm-4 off-white*/
}
.text-color-2 {
  color: #1b1b1b; /*gray-90 warm black*/
}
.text-color-3 {
  color: #757575; /*gray-50 medium gray*/
}

  /**** PAGE STYLES ****/

  body {
    background: #fbfbfb;
    color: #333;
  }

  .main {
    margin: 4em auto 0;
    /* max-width: 800px; */
  }

  .headers {
    margin: 60px 0 20px;
  }
  .headers h1 {
    margin: 10px 0;
    color: #333;
  }
  .headers h2 {
    line-height: 1.5;
    padding-bottom: 0.5em;
  }
</style>

<article id="ca-important" class="main clear-user-agent-styles">
  <section class="color-topic-1">
    <div class="headers">
      <h1>Colors</h1>
      <h2>Color palette</h2>
    </div>
    <ul class="swatch-grid" aria-label="color swatches">

      <li class="swatch swatch--red-50" aria-label="red-50 swatch">
        <div class="swatch__color-area">
          <p class="swatch__name" aria-label="color name">Red-50</p>
          <p class="swatch__hex-code" aria-label="red-50 hex code">#d83933</p>
          <table class="contrast-table" cellspacing=0>
            <thead>
              <tr class="contrast-table__row">
                <td><span class="u-hide">Label</span></td>
                <td>16pt</td>
                <td>24pt</td>
                <td>Graphics</td>
              </tr>
            </thead>
            <tbody>
              <tr class="contrast-table__row">
                <td class="text-color-1">Gray-warm-4</td>
                <td>Pass</td>
                <td>Pass</td>
                <td>Pass</td>
              </tr>
              <tr class="contrast-table__row">
                <td class="text-color-2">Gray-90</td>
                <td>Not legible</td>
                <td>Pass</td>
                <td>Pass</td>
              </tr>
              <tr class="contrast-table__row contrast-table__row--last">
                <td class="text-color-3">Gray-50</td>
                <td>Not legible</td>
                <td>Not legible</td>
                <td>Not legible</td>
              </tr>
            </tbody>
          </table>
        </div>
        <div class="swatch__info-area">
          <p class="swatch__common-name" aria-label="color common name">Primary Red</p>
          <p class="swatch__rgb" aria-label="color rgb"><strong>RGB</strong> (216, 57, 51)</p><p><strong>CMYK</strong> (0, 62, 65, 15)</p>
        </div>
      </li>
      
      <li class="swatch swatch--red-60" aria-label="red-60 swatch">
        <div class="swatch__color-area swatch__color-area--inverted">
          <p class="swatch__name" aria-label="color name">Red-60</p>
          <p class="swatch__hex-code" aria-label="red-60 hex code">#a23737</p>
          <table class="contrast-table" cellspacing=0>
            <thead>
              <tr class="contrast-table__row">
                <td><span class="u-hide">Label</span></td>
                <td>16pt</td>
                <td>24pt</td>
                <td>Graphics</td>
              </tr>
            </thead>
            <tbody>
              <tr class="contrast-table__row">
                <td class="text-color-1">Gray-warm-4</td>
                <td>Pass</td>
                <td>Pass</td>
                <td>Pass</td>
              </tr>
              <tr class="contrast-table__row">
                <td class="text-color-2">Gray-90</td>
                <td>Not legible</td>
                <td>Not legible</td>
                <td>Not legible</td>
              </tr>
              <tr class="contrast-table__row contrast-table__row--last">
                <td class="text-color-3">Gray-50</td>
                <td>Not legible</td>
                <td>Not legible</td>
                <td>Not legible</td>
              </tr>
            </tbody>
          </table>
        </div>
        <div class="swatch__info-area">
          <p class="swatch__common-name" aria-label="color common name">Dark Red</p>
          <p class="swatch__rgb" aria-label="color rgb"><strong>RGB</strong> (162, 55, 55)</p><p><strong>CMYK</strong> (0, 42, 42, 36)</p>
        </div>
      </li>
      
            <li class="swatch swatch--mint-cool-40v" aria-label="mint-cool-40v swatch">
        <div class="swatch__color-area">
          <p class="swatch__name" aria-label="color name">Mint-cool-40v</p>
          <p class="swatch__hex-code" aria-label="mint-cool-40v hex code">#00a398</p>
          <table class="contrast-table" cellspacing=0>
            <thead>
              <tr class="contrast-table__row">
                <td><span class="u-hide">Label</span></td>
                <td>16pt</td>
                <td>24pt</td>
                <td>Graphics</td>
              </tr>
            </thead>
            <tbody>
              <tr class="contrast-table__row">
                <td class="text-color-1">Gray-warm-4</td>
                <td>Pass</td>
                <td>Pass</td>
                <td>Pass</td>
              </tr>
              <tr class="contrast-table__row">
                <td class="text-color-2">Gray-90</td>
                <td>Not legible</td>
                <td>Pass</td>
                <td>Pass</td>
              </tr>
              <tr class="contrast-table__row contrast-table__row--last">
                <td class="text-color-3">Gray-50</td>
                <td>Not legible</td>
                <td>Not legible</td>
                <td>Not legible</td>
              </tr>
            </tbody>
          </table>
        </div>
        <div class="swatch__info-area">
          <p class="swatch__common-name" aria-label="color common name">Primary Green</p>
          <p class="swatch__rgb" aria-label="color rgb"><strong>RGB</strong> (216, 57, 51)</p><p><strong>CMYK</strong> (0, 62, 65, 15)</p>
        </div>
      </li>
      
      <li class="swatch swatch--mint-cool-60v" aria-label="mint-cool-60v">
        <div class="swatch__color-area swatch__color-area--inverted">
          <p class="swatch__name" aria-label="color name">Mint-cool-60v</p>
          <p class="swatch__hex-code" aria-label="mint-cool-60v hex code">#0f6460</p>
          <table class="contrast-table" cellspacing=0>
            <thead>
              <tr class="contrast-table__row">
                <td><span class="u-hide">Label</span></td>
                <td>16pt</td>
                <td>24pt</td>
                <td>Graphics</td>
              </tr>
            </thead>
            <tbody>
              <tr class="contrast-table__row">
                <td class="text-color-1">Gray-warm-4</td>
                <td>Pass</td>
                <td>Pass</td>
                <td>Pass</td>
              </tr>
              <tr class="contrast-table__row">
                <td class="text-color-2">Gray-90</td>
                <td>Not legible</td>
                <td>Not legible</td>
                <td>Not legible</td>
              </tr>
              <tr class="contrast-table__row contrast-table__row--last">
                <td class="text-color-3">Gray-50</td>
                <td>Not legible</td>
                <td>Not legible</td>
                <td>Not legible</td>
              </tr>
            </tbody>
          </table>
        </div>
        <div class="swatch__info-area">
          <p class="swatch__common-name" aria-label="color common name">Dark Green</p>
          <p class="swatch__rgb" aria-label="color rgb"><strong>RGB</strong> (162, 55, 55)</p><p><strong>CMYK</strong> (0, 42, 42, 36)</p>
        </div>
      </li>
      
      <li class="swatch swatch--gray-warm-4" aria-label="gray-warm-4 swatch">
        <div class="swatch__color-area">
          <p class="swatch__name" aria-label="color name">Gray-warm-4</p>
          <p class="swatch__hex-code" aria-label="gray-warm-4 hex code">#F5F5F0</p>
          <table class="contrast-table" cellspacing=0>
            <thead>
              <tr class="contrast-table__row">
                <td><span class="u-hide">Label</span></td>
                <td>16pt</td>
                <td>24pt</td>
                <td>Graphics</td>
              </tr>
            </thead>
            <tbody>
              <tr class="contrast-table__row">
                <td class="text-color-1">Gray-warm-4</td>
                <td>Not legible</td>
                <td>Not legible</td>
                <td>Not legible</td>
              </tr>
              <tr class="contrast-table__row">
                <td class="text-color-2">Gray-90</td>
                <td>Pass</td>
                <td>Pass</td>
                <td>Pass</td>
              </tr>
              <tr class="contrast-table__row contrast-table__row--last">
                <td class="text-color-3">Gray-50</td>
                <td>Not legible</td>
                <td>Pass</td>
                <td>Pass</td>
              </tr>
            </tbody>
          </table>
        </div>
        <div class="swatch__info-area">
          <p class="swatch__common-name" aria-label="color common name">Off-White</p>
          <p class="swatch__rgb" aria-label="color rgb"><strong>RGB</strong> (245, 245, 240)</p><p><strong>CMYK</strong> (0, 0, 2, 4)</p>
        </div>
      </li>
      
      <li class="swatch swatch--gray-50" aria-label="gray-50">
        <div class="swatch__color-area swatch__color-area--inverted">
          <p class="swatch__name" aria-label="color name">Gray-50</p>
          <p class="swatch__hex-code" aria-label="gray-50 hex code">#757575</p>
          <table class="contrast-table" cellspacing=0>
            <thead>
              <tr class="contrast-table__row">
                <td><span class="u-hide">Label</span></td>
                <td>16pt</td>
                <td>24pt</td>
                <td>Graphics</td>
              </tr>
            </thead>
            <tbody>
              <tr class="contrast-table__row">
                <td class="text-color-1">Gray-warm-4</td>
                <td>Not legible</td>
                <td>Pass</td>
                <td>Pass</td>
              </tr>
              <tr class="contrast-table__row">
                <td class="text-color-2">Gray-90</td>
                <td>Not legible</td>
                <td>Pass</td>
                <td>Pass</td>
              </tr>
              <tr class="contrast-table__row contrast-table__row--last">
                <td class="text-color-3">Gray-50</td>
                <td>Not legible</td>
                <td>Not legible</td>
                <td>Not legible</td>
              </tr>
            </tbody>
          </table>
        </div>
        <div class="swatch__info-area">
          <p class="swatch__common-name" aria-label="color common name">Medium Gray</p>
          <p class="swatch__rgb" aria-label="color rgb"><strong>RGB</strong> (117, 117, 117)</p><p><strong>CMYK</strong> (0, 0, 0, 54)</p>
        </div>
      </li>
      
      <li class="swatch swatch--gray-90" aria-label="gray-90">
        <div class="swatch__color-area swatch__color-area--inverted">
          <p class="swatch__name" aria-label="color name">Gray-90</p>
          <p class="swatch__hex-code" aria-label="gray-90 hex code">#1b1b1b</p>
          <table class="contrast-table" cellspacing=0>
            <thead>
              <tr class="contrast-table__row">
                <td><span class="u-hide">Label</span></td>
                <td>16pt</td>
                <td>24pt</td>
                <td>Graphics</td>
              </tr>
            </thead>
            <tbody>
              <tr class="contrast-table__row">
                <td class="text-color-1">Gray-warm-4</td>
                <td>Pass</td>
                <td>Pass</td>
                <td>Pass</td>
              </tr>
              <tr class="contrast-table__row">
                <td class="text-color-2">Gray-90</td>
                <td>Not legible</td>
                <td>Not legible</td>
                <td>Not legible</td>
              </tr>
              <tr class="contrast-table__row contrast-table__row--last">
                <td class="text-color-3">Gray-50</td>
                <td>Not legible</td>
                <td>Pass</td>
                <td>Pass</td>
              </tr>
            </tbody>
          </table>
        </div>
        <div class="swatch__info-area">
          <p class="swatch__common-name" aria-label="color common name">Off-Black</p>
          <p class="swatch__rgb" aria-label="color rgb"><strong>RGB</strong> (27, 27, 27)</p><p><strong>CMYK</strong> (0, 0, 0, 89)</p>
        </div>
      </li>

    </ul>
  </section>
</article>
