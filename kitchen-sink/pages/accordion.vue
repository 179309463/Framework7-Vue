<template>
  <f7-page>
    <f7-navbar back-link="Back" title="Accordion" sliding></f7-navbar>

    <f7-block-title>List View Accordion</f7-block-title>
    <f7-list accordion>
      <f7-list-item accordion-item
        v-for="n in 3"
        :key="n"
        :title="'Item ' + n"
        @accordion:open="onOpen"
        @accordion:opened="onOpened"
        @accordion:close="onClose"
        @accordion:closed="onClosed"
      >
        <f7-accordion-content>
          <f7-block>
            <p>Accordion content {{n}}</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean eu felis volutpat, rutrum ex quis, lobortis ex. Curabitur quis mattis lorem. Nullam magna lacus, interdum vel maximus nec, vestibulum non quam. Phasellus ornare efficitur porttitor. Quisque neque diam, imperdiet in fermentum nec, congue vitae ante. Nullam imperdiet maximus commodo. Morbi pharetra id purus ac ultrices. Duis non posuere libero.</p>
          </f7-block>
        </f7-accordion-content>
      </f7-list-item>
    </f7-list>

    <f7-block-title>List View Accordion Seperate</f7-block-title>
    <f7-list>
      <f7-list-item accordion-item
        v-for="n in 3"
        :key="n"
        :title="'Item ' + n"
        @accordion:open="onOpen"
        @accordion:opened="onOpened"
        @accordion:close="onClose"
        @accordion:closed="onClosed"
      >
        <f7-accordion-content>
          <f7-block>
            <p>Accordion content {{n}}</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean eu felis volutpat, rutrum ex quis, lobortis ex. Curabitur quis mattis lorem. Nullam magna lacus, interdum vel maximus nec, vestibulum non quam. Phasellus ornare efficitur porttitor. Quisque neque diam, imperdiet in fermentum nec, congue vitae ante. Nullam imperdiet maximus commodo. Morbi pharetra id purus ac ultrices. Duis non posuere libero.</p>
          </f7-block>
        </f7-accordion-content>
      </f7-list-item>
    </f7-list>


    <f7-block-title>Inset Accordion</f7-block-title>
    <f7-list accordion inset>
      <f7-list-item accordion-item
        v-for="n in 3"
        :key="n"
        :title="'Item ' + n"
        @accordion:open="onOpen"
        @accordion:opened="onOpened"
        @accordion:close="onClose"
        @accordion:closed="onClosed"
      >
        <f7-accordion-content>
          <f7-block>
            <p>Accordion content {{n}}</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean eu felis volutpat, rutrum ex quis, lobortis ex. Curabitur quis mattis lorem. Nullam magna lacus, interdum vel maximus nec, vestibulum non quam. Phasellus ornare efficitur porttitor. Quisque neque diam, imperdiet in fermentum nec, congue vitae ante. Nullam imperdiet maximus commodo. Morbi pharetra id purus ac ultrices. Duis non posuere libero.</p>
          </f7-block>
        </f7-accordion-content>
      </f7-list-item>
    </f7-list>

    <f7-block-title>Custom Collapsible</f7-block-title>
    <f7-block inner>
      <f7-accordion-item v-for="n in 3" :key="n">
        <f7-accordion-toggle><b>Item {{n}}</b></f7-accordion-toggle>
        <f7-accordion-content>Content {{n}}</f7-accordion-content>
      </f7-accordion-item>
    </f7-block>

    <f7-block-title>Custom Styled Accordion</f7-block-title>
    <f7-accordion class="content-block custom-accordion">
      <f7-accordion-item
        v-for="n in 3"
        :key="n"
        :title="'Item ' + n"
        @accordion:open="onOpen"
        @accordion:opened="onOpened"
        @accordion:close="onClose"
        @accordion:closed="onClosed">
        <f7-accordion-toggle><i class="icon icon-ks-plus">+</i><i class="icon icon-ks-minus">-</i><span>Item {{n}}</span></f7-accordion-toggle>
        <f7-accordion-content>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean elementum id neque nec commodo. Sed vel justo at turpis laoreet pellentesque quis sed lorem. Integer semper arcu nibh, non mollis arcu tempor vel. Sed pharetra tortor vitae est rhoncus, vel congue dui sollicitudin. Donec eu arcu dignissim felis viverra blandit suscipit eget ipsum.</p>
        </f7-accordion-content>
      </f7-accordion-item>
    </f7-accordion>

  </f7-page>
</template>
<script>
  export default {
    methods: {
      onOpen: function (event){
        console.log('open');
      },
      onOpened: function (event){
        console.log('opened');
      },
      onClose: function (event){
        console.log('close');
      },
      onClosed: function (event){
        console.log('closed');
      }
    }
  }
</script>
<style>
.custom-accordion {
  padding-left: 0;
  padding-right: 0;
}
.custom-accordion .accordion-item-toggle {
  padding: 0px 15px;
  height: 44px;
  line-height: 44px;
  font-size: 17px;
  color: #000;
  border-bottom: 1px solid rgba(0, 0, 0, 0.15);
  cursor: pointer;
}
.custom-accordion .accordion-item-toggle:active {
  background: rgba(0, 0, 0, 0.15);
}
.custom-accordion .accordion-item-toggle span {
  display: inline-block;
  margin-left: 15px;
}
html[dir="rtl"] .custom-accordion .accordion-item-toggle span {
  margin-left: 0;
  margin-right: 15px;
}
.custom-accordion .accordion-item:last-child .accordion-item-toggle {
  border-bottom: none;
}
.custom-accordion .icon-ks-plus,
.custom-accordion .icon-ks-minus {
  display: inline-block;
  width: 22px;
  height: 22px;
  border: 1px solid #000;
  border-radius: 100%;
  line-height: 20px;
  text-align: center;
}
.custom-accordion .icon-ks-minus {
  display: none;
}
.custom-accordion .accordion-item-expanded .icon-ks-minus {
  display: inline-block;
}
.custom-accordion .accordion-item-expanded .icon-ks-plus {
  display: none;
}
.custom-accordion .accordion-item-content {
  padding: 0px 15px;
}
</style>
