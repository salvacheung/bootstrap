---
layout: docs
title: Accordion
description: Build vertically collapsing accordions in combination with our Collapse JavaScript plugin.
group: components
aliases:
  - "/components/"
  - "/docs/5.2/components/"
toc: true
---

## How it works

The accordion uses [collapse]({{< docsref "/components/collapse" >}}) internally to make it collapsible. To render an accordion that's expanded, add the `.open` class on the `.accordion`.

{{< callout info >}}
{{< partial "callout-info-prefersreducedmotion.md" >}}
{{< /callout >}}

## Example

Click the accordions below to expand/collapse the accordion content.

{{< example >}}
<div class="accordion" id="accordionExample">
  <div class="card mb-0">
      <div class="card-header" id="headingOne">
          <h5 class="m-0">
              <a class="accordion-title d-block pt-2 pb-2 collapsed" data-bs-toggle="collapse" href="#collapseOne" aria-expanded="false" aria-controls="collapseOne">
                  Collapsible Group Item #1
              </a>
          </h5>
      </div>
      <div id="collapseOne" class="collapse" aria-labelledby="headingOne" data-bs-parent="#accordionExample" style="">
          <div class="card-body">
              Anim pariatur cliche reprehenderit, enim eiusmod high life
              accusamus terry richardson ad squid. 3 wolf moon officia
              aute, non cupidatat skateboard dolor brunch. Food truck
              quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor,
              sunt aliqua put a bird on it squid single-origin coffee
              nulla assumenda shoreditch et. Nihil anim keffiyeh
              helvetica, craft beer labore wes anderson cred nesciunt
              sapiente ea proident. Ad vegan excepteur butcher vice lomo.
              Leggings occaecat craft beer farm-to-table, raw denim
              aesthetic synth nesciunt you probably haven't heard of them
              accusamus labore sustainable VHS.
          </div>
      </div>
  </div>
  <div class="card mb-0">
      <div class="card-header" id="heading2">
          <h5 class="m-0">
              <a class="accordion-title d-block pt-2 pb-2 collapsed" data-bs-toggle="collapse" href="#collapse2" aria-expanded="false" aria-controls="collapse2">
                  Collapsible Group Item #1
              </a>
          </h5>
      </div>
      <div id="collapse2" class="collapse" aria-labelledby="heading2" data-bs-parent="#accordionExample" style="">
          <div class="card-body">
              Anim pariatur cliche reprehenderit, enim eiusmod high life
              accusamus terry richardson ad squid. 3 wolf moon officia
              aute, non cupidatat skateboard dolor brunch. Food truck
              quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor,
              sunt aliqua put a bird on it squid single-origin coffee
              nulla assumenda shoreditch et. Nihil anim keffiyeh
              helvetica, craft beer labore wes anderson cred nesciunt
              sapiente ea proident. Ad vegan excepteur butcher vice lomo.
              Leggings occaecat craft beer farm-to-table, raw denim
              aesthetic synth nesciunt you probably haven't heard of them
              accusamus labore sustainable VHS.
          </div>
      </div>
  </div>
  <div class="card mb-0">
      <div class="card-header" id="heading3">
          <h5 class="m-0">
              <a class="accordion-title d-block pt-2 pb-2 collapsed" data-bs-toggle="collapse" href="#collapse3" aria-expanded="false" aria-controls="collapse3">
                  Collapsible Group Item #1
              </a>
          </h5>
      </div>
      <div id="collapse3" class="collapse" aria-labelledby="heading3" data-bs-parent="#accordionExample" style="">
          <div class="card-body">
              Anim pariatur cliche reprehenderit, enim eiusmod high life
              accusamus terry richardson ad squid. 3 wolf moon officia
              aute, non cupidatat skateboard dolor brunch. Food truck
              quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor,
              sunt aliqua put a bird on it squid single-origin coffee
              nulla assumenda shoreditch et. Nihil anim keffiyeh
              helvetica, craft beer labore wes anderson cred nesciunt
              sapiente ea proident. Ad vegan excepteur butcher vice lomo.
              Leggings occaecat craft beer farm-to-table, raw denim
              aesthetic synth nesciunt you probably haven't heard of them
              accusamus labore sustainable VHS.
          </div>
      </div>
  </div>
</div>
{{< /example >}}

### Flush

Add `.accordion-flush` to remove the default `background-color`, some borders, and some rounded corners to render accordions edge-to-edge with their parent container.

{{< example class="bg-light" >}}
<div class="accordion accordion-flush" id="accordionFlushExample">
  <div class="accordion-item">
    <h2 class="accordion-header" id="flush-headingOne">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#flush-collapseOne" aria-expanded="false" aria-controls="flush-collapseOne">
        Accordion Item #1
      </button>
    </h2>
    <div id="flush-collapseOne" class="accordion-collapse collapse" aria-labelledby="flush-headingOne" data-bs-parent="#accordionFlushExample">
      <div class="accordion-body">Placeholder content for this accordion, which is intended to demonstrate the <code>.accordion-flush</code> class. This is the first item's accordion body.</div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="flush-headingTwo">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#flush-collapseTwo" aria-expanded="false" aria-controls="flush-collapseTwo">
        Accordion Item #2
      </button>
    </h2>
    <div id="flush-collapseTwo" class="accordion-collapse collapse" aria-labelledby="flush-headingTwo" data-bs-parent="#accordionFlushExample">
      <div class="accordion-body">Placeholder content for this accordion, which is intended to demonstrate the <code>.accordion-flush</code> class. This is the second item's accordion body. Let's imagine this being filled with some actual content.</div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="flush-headingThree">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#flush-collapseThree" aria-expanded="false" aria-controls="flush-collapseThree">
        Accordion Item #3
      </button>
    </h2>
    <div id="flush-collapseThree" class="accordion-collapse collapse" aria-labelledby="flush-headingThree" data-bs-parent="#accordionFlushExample">
      <div class="accordion-body">Placeholder content for this accordion, which is intended to demonstrate the <code>.accordion-flush</code> class. This is the third item's accordion body. Nothing more exciting happening here in terms of content, but just filling up the space to make it look, at least at first glance, a bit more representative of how this would look in a real-world application.</div>
    </div>
  </div>
</div>
{{< /example >}}

### Always open

Omit the `data-bs-parent` attribute on each `.accordion-collapse` to make accordion items stay open when another item is opened.

{{< example >}}
<div class="accordion" id="accordionPanelsStayOpenExample">
  <div class="accordion-item">
    <h2 class="accordion-header" id="panelsStayOpen-headingOne">
      <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#panelsStayOpen-collapseOne" aria-expanded="true" aria-controls="panelsStayOpen-collapseOne">
        Accordion Item #1
      </button>
    </h2>
    <div id="panelsStayOpen-collapseOne" class="accordion-collapse collapse show" aria-labelledby="panelsStayOpen-headingOne">
      <div class="accordion-body">
        <strong>This is the first item's accordion body.</strong> It is shown by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables. It's also worth noting that just about any HTML can go within the <code>.accordion-body</code>, though the transition does limit overflow.
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="panelsStayOpen-headingTwo">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#panelsStayOpen-collapseTwo" aria-expanded="false" aria-controls="panelsStayOpen-collapseTwo">
        Accordion Item #2
      </button>
    </h2>
    <div id="panelsStayOpen-collapseTwo" class="accordion-collapse collapse" aria-labelledby="panelsStayOpen-headingTwo">
      <div class="accordion-body">
        <strong>This is the second item's accordion body.</strong> It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables. It's also worth noting that just about any HTML can go within the <code>.accordion-body</code>, though the transition does limit overflow.
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="panelsStayOpen-headingThree">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#panelsStayOpen-collapseThree" aria-expanded="false" aria-controls="panelsStayOpen-collapseThree">
        Accordion Item #3
      </button>
    </h2>
    <div id="panelsStayOpen-collapseThree" class="accordion-collapse collapse" aria-labelledby="panelsStayOpen-headingThree">
      <div class="accordion-body">
        <strong>This is the third item's accordion body.</strong> It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables. It's also worth noting that just about any HTML can go within the <code>.accordion-body</code>, though the transition does limit overflow.
      </div>
    </div>
  </div>
</div>
{{< /example >}}

## Accessibility

Please read the [collapse accessibility section]({{< docsref "/components/collapse#accessibility" >}}) for more information.

## CSS

### Variables

{{< added-in "5.2.0" >}}

As part of Bootstrap's evolving CSS variables approach, accordions now use local CSS variables on `.accordion` for enhanced real-time customization. Values for the CSS variables are set via Sass, so Sass customization is still supported, too.

{{< scss-docs name="accordion-css-vars" file="scss/_accordion.scss" >}}

### Sass variables

{{< scss-docs name="accordion-variables" file="scss/_variables.scss" >}}
