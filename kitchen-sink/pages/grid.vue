<template>
  <f7-page>
    <f7-navbar back-link="Back" title="Grid" sliding></f7-navbar>

    <f7-block-title>Grid</f7-block-title>
    <f7-block inner>
      <p>
        <f7-grid>
          <f7-col :style="columnStyle">50%</f7-col>
          <f7-col :style="columnStyle">50%</f7-col>
        </f7-grid>
      </p>
      <p>
        <f7-grid>
          <f7-col :style="columnStyle">33%</f7-col>
          <f7-col :style="columnStyle">33%</f7-col>
          <f7-col :style="columnStyle">33%</f7-col>
        </f7-grid>
      </p>
      <p>
        <f7-grid>
          <f7-col width="50" tablet-width="80" :style="columnStyle">50%</f7-col>
          <f7-col width="25" tablet-width="10" :style="columnStyle">25%</f7-col>
          <f7-col width="25" tablet-width="10" :style="columnStyle">25%</f7-col>
        </f7-grid>
      </p>
      <p>
        <f7-grid no-gutter>
          <f7-col width="66" :style="columnStyle">66%</f7-col>
          <f7-col width="33" :style="columnStyle">33%</f7-col>
        </f7-grid>
      </p>
    </f7-block>

    <div class="content-block">
      <p>Framework7 comes with flexible layout grid:</p>
    </div>
    <div class="ks-grid">
      <div class="content-block-title">Columns with gutter</div>
      <div class="content-block">
        <div class="row">
          <div class="col-50">.col-50</div>
          <div class="col-50">.col-50</div>
        </div>
        <div class="row">
          <div class="col-25">.col-25</div>
          <div class="col-25">.col-25</div>
          <div class="col-25">.col-25</div>
          <div class="col-25">.col-25</div>
        </div>
        <div class="row">
          <div class="col-33">.col-33</div>
          <div class="col-33">.col-33</div>
          <div class="col-33">.col-33</div>
        </div>
        <div class="row">
          <div class="col-20">.col-20</div>
          <div class="col-20">.col-20</div>
          <div class="col-20">.col-20</div>
          <div class="col-20">.col-20</div>
          <div class="col-20">.col-20</div>
        </div>
        <div class="row">
          <div class="col-33">.col-33</div>
          <div class="col-66">.col-66</div>
        </div>
        <div class="row">
          <div class="col-25">.col-25</div>
          <div class="col-25">.col-25</div>
          <div class="col-50">.col-50</div>
        </div>
        <div class="row">
          <div class="col-75">.col-75</div>
          <div class="col-25">.col-25</div>
        </div>
        <div class="row">
          <div class="col-80">.col-80</div>
          <div class="col-20">.col-20</div>
        </div>
      </div>
      <div class="content-block-title">No gutter between columns</div>
      <div class="content-block">
        <div class="row no-gutter">
          <div class="col-50">.col-50</div>
          <div class="col-50">.col-50</div>
        </div>
        <div class="row no-gutter">
          <div class="col-25">.col-25</div>
          <div class="col-25">.col-25</div>
          <div class="col-25">.col-25</div>
          <div class="col-25">.col-25</div>
        </div>
        <div class="row no-gutter">
          <div class="col-33">.col-33</div>
          <div class="col-33">.col-33</div>
          <div class="col-33">.col-33</div>
        </div>
        <div class="row no-gutter">
          <div class="col-20">.col-20</div>
          <div class="col-20">.col-20</div>
          <div class="col-20">.col-20</div>
          <div class="col-20">.col-20</div>
          <div class="col-20">.col-20</div>
        </div>
        <div class="row no-gutter">
          <div class="col-33">.col-33</div>
          <div class="col-66">.col-66</div>
        </div>
        <div class="row no-gutter">
          <div class="col-25">.col-25</div>
          <div class="col-25">.col-25</div>
          <div class="col-50">.col-50</div>
        </div>
        <div class="row no-gutter">
          <div class="col-75">.col-75</div>
          <div class="col-25">.col-25</div>
        </div>
        <div class="row no-gutter">
          <div class="col-80">.col-80</div>
          <div class="col-20">.col-20</div>
        </div>
      </div>
      <div class="content-block-title">Nested</div>
      <div class="content-block">
        <div class="row">
          <div class="col-50">.col-50
            <div class="row">
              <div class="col-50">.col-50</div>
              <div class="col-50">.col-50</div>
            </div>
          </div>
          <div class="col-50">.col-50
            <div class="row">
              <div class="col-33">.col-33</div>
              <div class="col-66">.col-66</div>
            </div>
          </div>
        </div>
      </div>
      <div class="content-block-title">Responsive Grid</div>
      <div class="content-block">
        <p>Grid cells have different size on Phone/Tablet</p>
        <div class="row">
          <div class="col-100 tablet-50">.col-100.tablet-50</div>
          <div class="col-100 tablet-50">.col-100.tablet-50</div>
        </div>
        <div class="row">
          <div class="col-50 tablet-25">.col-50.tablet-25</div>
          <div class="col-50 tablet-25">.col-50.tablet-25</div>
          <div class="col-50 tablet-25">.col-50.tablet-25</div>
          <div class="col-50 tablet-25">.col-50.tablet-25</div>
        </div>
        <div class="row">
          <div class="col-100 tablet-40">.col-100.tablet-40</div>
          <div class="col-50 tablet-60">.col-50.tablet-60</div>
          <div class="col-50 tablet-66">.col-50.tablet-66</div>
          <div class="col-100 tablet-33">.col-100.tablet-33</div>
        </div>
      </div>
    </div>

  </f7-page>
</template>
<script>
  export default {
    data: function () {
      return {
        columnStyle: 'border: 1px solid #e5e5e5; padding:5px; text-align: center'
      }
    }
  }
</script>
<style>
.ks-grid div[class*="col-"] {
  background: #fff;
  text-align: center;
  color: #000;
  border: 1px solid #ddd;
  padding: 5px;
  margin-bottom: 15px;
}
</style>