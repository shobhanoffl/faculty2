<template>
<body>
<div class="container">
      <h2>FAQ</h2>
      <div class="accordion">
        <div class="accordion-item">
          <button id="accordion-button-1" aria-expanded="false">
            <span class="accordion-title">What is this website about?</span>
            <span class="icon" aria-hidden="true"></span>
          </button>
          <div class="accordion-content">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
              incididunt ut labore et dolore magna aliqua. Elementum sagittis vitae et leo duis ut.
              Ut tortor pretium viverra suspendisse potenti.
            </p>
          </div>
        </div>
        <div class="accordion-item">
          <button id="accordion-button-2" aria-expanded="false">
            <span class="accordion-title">How to post a photo?</span>
            <span class="icon" aria-hidden="true"></span>
          </button>
          <div class="accordion-content">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
              incididunt ut labore et dolore magna aliqua. Elementum sagittis vitae et leo duis ut.
              Ut tortor pretium viverra suspendisse potenti.
            </p>
          </div>
        </div>
        <div class="accordion-item">
          <button id="accordion-button-3" aria-expanded="false">
            <span class="accordion-title">How to upload a video?</span>
            <span class="icon" aria-hidden="true"></span>
          </button>
          <div class="accordion-content">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
              incididunt ut labore et dolore magna aliqua. Elementum sagittis vitae et leo duis ut.
              Ut tortor pretium viverra suspendisse potenti.
            </p>
          </div>
        </div>
        <div class="accordion-item">
          <button id="accordion-button-4" aria-expanded="false">
            <span class="accordion-title">How much does the Earth weigh?</span>
            <span class="icon" aria-hidden="true"></span>
          </button>
          <div class="accordion-content">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
              incididunt ut labore et dolore magna aliqua. Elementum sagittis vitae et leo duis ut.
              Ut tortor pretium viverra suspendisse potenti.
            </p>
          </div>
        </div>
        <div class="accordion-item">
          <button id="accordion-button-5" aria-expanded="false">
            <span class="accordion-title">How do airplanes stay up?</span>
            <span class="icon" aria-hidden="true"></span>
          </button>
          <div class="accordion-content">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
              incididunt ut labore et dolore magna aliqua. Elementum sagittis vitae et leo duis ut.
              Ut tortor pretium viverra suspendisse potenti.
            </p>
          </div>
          <div class="accordion-item">
            <button id="accordion-button-5" aria-expanded="false">
              <span class="accordion-title">How do airplanes stay up?</span>
              <span class="icon" aria-hidden="true"></span>
            </button>
            <div class="accordion-content">
              <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                incididunt ut labore et dolore magna aliqua. Elementum sagittis vitae et leo duis ut.
                Ut tortor pretium viverra suspendisse potenti.
              </p>
        </div>
    </div>
        <div class="accordion-item">
          <button id="accordion-button-5" aria-expanded="false">
            <span class="accordion-title">How do airplanes stay up?</span>
            <span class="icon" aria-hidden="true"></span>
          </button>
          <div class="accordion-content">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
              incididunt ut labore et dolore magna aliqua. Elementum sagittis vitae et leo duis ut.
              Ut tortor pretium viverra suspendisse potenti.
            </p>

      </div>
    </div>
    <div class="accordion-item">
      <button id="accordion-button-5" aria-expanded="false">
        <span class="accordion-title">How do airplanes stay up?</span>
        <span class="icon" aria-hidden="true"></span>
      </button>
      <div class="accordion-content">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
          incididunt ut labore et dolore magna aliqua. Elementum sagittis vitae et leo duis ut.
          Ut tortor pretium viverra suspendisse potenti.
        </p>


    </div>
</div>
<div class="accordion-item">
  <button id="accordion-button-5" aria-expanded="false">
    <span class="accordion-title">How do airplanes stay up?</span>
    <span class="icon" aria-hidden="true"></span>
  </button>
  <div class="accordion-content">
    <p>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
      incididunt ut labore et dolore magna aliqua. Elementum sagittis vitae et leo duis ut.
      Ut tortor pretium viverra suspendisse potenti.
    </p>
</div>
    </div>
</div>
<div class="accordion-item">
  <button id="accordion-button-5" aria-expanded="false">
    <span class="accordion-title">How do airplanes stay up?</span>
    <span class="icon" aria-hidden="true"></span>
  </button>
  <div class="accordion-content">
    <p>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
      incididunt ut labore et dolore magna aliqua. Elementum sagittis vitae et leo duis ut.
      Ut tortor pretium viverra suspendisse potenti.
    </p>

  </div>
</div>
</div>
      </div>
</body>
</template>

<script>
export default {
    data(){
        //
    },
    mounted(){
        const items = document.querySelectorAll('.accordion button');

        function toggleAccordion() {
          const itemToggle = this.getAttribute('aria-expanded');
          var i=0;
          for (i = 0; i < items.length; i++) {
            items[i].setAttribute('aria-expanded', 'false');
          }
          if (itemToggle == 'false') {
            this.setAttribute('aria-expanded', 'true');
          }
        }

        items.forEach((item) => item.addEventListener('click', toggleAccordion));
    }
}
</script>

<style scoped src="../assets/styles/faq.css">

</style>