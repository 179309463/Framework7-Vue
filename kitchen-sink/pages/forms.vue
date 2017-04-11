<template>
  <f7-page>
    <f7-navbar back-link="Back" title="Forms" sliding></f7-navbar>

    <f7-block-title>FULL LAYOUT</f7-block-title>
    <f7-list form>
      <f7-list-item media='<i class="icon f7-icons">person</i>'>
        <f7-label>Name</f7-label>
        <f7-input name="name" type="text" placeholder="Name"></f7-input>
      </f7-list-item>
      <f7-list-item media='<i class="icon f7-icons">email</i>'>
        <f7-label>E-mail</f7-label>
        <f7-input name="email" type="email" placeholder="E-mail"></f7-input>
      </f7-list-item>
      <f7-list-item media='<i class="icon f7-icons">world</i>'>
        <f7-label>URL</f7-label>
        <f7-input name="url" type="url" placeholder="URL"></f7-input>
      </f7-list-item>
      <f7-list-item media='<i class="icon f7-icons">lock</i>'>
        <f7-label>Password</f7-label>
        <f7-input name="password" type="password" placeholder="Password"></f7-input>
      </f7-list-item>
      <f7-list-item media='<i class="icon f7-icons">phone</i>'>
        <f7-label>Phone</f7-label>
        <f7-input name="tel" type="tel" placeholder="Phone"></f7-input>
      </f7-list-item>
      <f7-list-item media='<i class="icon f7-icons">persons</i>'>
        <f7-label>Gender</f7-label>
        <f7-input name="gender" type="select">
          <option value="1">Male</option>
          <option value="2">Female</option>
        </f7-input>
      </f7-list-item>      
      <f7-list-item media='<i class="icon f7-icons">calendar</i>'>
        <f7-label>Birth date</f7-label>
        <f7-input name="date" type="date" placeholder="Birth date" value="2014-04-30"></f7-input>
      </f7-list-item>
      <f7-list-item media='<i class="icon f7-icons">calendar</i>'>
        <f7-label>Date time</f7-label>
        <f7-input name="datetime" type="datetime-local"></f7-input>
      </f7-list-item>
      <f7-list-item media='<i class="icon f7-icons">check</i>'>
        <f7-label>Switch</f7-label>
        <f7-input name="switch" type="switch" @change="onChange"></f7-input>
      </f7-list-item>
      <f7-list-item media='<i class="icon f7-icons">filter</i>'>
        <f7-label>Slider</f7-label>
        <f7-input type="range" min="0" max="100" step="1" value="90"></f7-input>
      </f7-list-item>
      <f7-list-item media='<i class="icon f7-icons">chat</i>'>
        <f7-label>Textarea</f7-label>
        <f7-input name="textarea" type="textarea" placeholder="Textarea"></f7-input>
      </f7-list-item>
      <f7-list-item media='<i class="icon f7-icons">chat</i>'>
        <f7-label>Resizable</f7-label>
        <f7-input name="textarea" type="textarea" resizable placeholder="Textarea"></f7-input>
      </f7-list-item>
      <f7-list-item media='<i class="icon f7-icons">calendar</i>'>
        <f7-label>Datepicker</f7-label>
        <f7-datepicker date-format="DD, dd MM yyyy" :value="new Date().getTime()"/>
      </f7-list-item>
      <f7-list-item media='<i class="icon f7-icons">calendar</i>'>
        <f7-label>Range Datepicker</f7-label>
        <f7-datepicker date-format="dd MM yyyy" :range-picker="true"/>
      </f7-list-item>
      <f7-list-item media='<i class="icon f7-icons">folder</i>'>
        <f7-label>File</f7-label>
        <f7-input type="file"></f7-input>
      </f7-list-item>
    </f7-list>

    <f7-block-title>ICONS AND INPUTS</f7-block-title>
    <f7-list form>
      <f7-list-item media='<i class="icon f7-icons">person</i>'>
        <f7-input name="name" type="text" placeholder="Name"></f7-input>
      </f7-list-item>
      <f7-list-item media='<i class="icon f7-icons">email</i>'>
        <f7-input name="email" type="email" placeholder="E-mail"></f7-input>
      </f7-list-item>
      <f7-list-item media='<i class="icon f7-icons">persons</i>'>
        <f7-input name="gender" type="select">
          <option value="1">Male</option>
          <option value="2">Female</option>
        </f7-input>
      </f7-list-item>      
      <f7-list-item media='<i class="icon f7-icons">calendar</i>'>
        <f7-input name="date" type="date" placeholder="Birth date" value="2014-04-30"></f7-input>
      </f7-list-item>
      <f7-list-item media='<i class="icon f7-icons">check</i>'>
        <f7-input name="switch" type="switch" @change="onChange"></f7-input>
      </f7-list-item>
    </f7-list>

    <f7-block-title>Form With Floating Labels</f7-block-title>
    <f7-list form>
      <f7-list-item>
        <f7-label floating>Name</f7-label>
        <f7-input name="name" type="text" placeholder="Name"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label floating>Password</f7-label>
        <f7-input name="password" type="password" placeholder="Password"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label floating>E-mail</f7-label>
        <f7-input name="email" type="email" placeholder="E-mail"></f7-input>
      </f7-list-item>
    </f7-list>

    <f7-block-title>JUST INPUTS</f7-block-title>
    <f7-list form>
      <f7-list-item>
        <f7-input name="name" type="text" placeholder="Name"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-input name="email" type="email" placeholder="E-mail"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-input name="gender" type="select">
          <option value="1">Male</option>
          <option value="2">Female</option>
        </f7-input>
      </f7-list-item>      
      <f7-list-item>
        <f7-input name="date" type="date" placeholder="Birth date" value="2014-04-30"></f7-input>
      </f7-list-item>
    </f7-list>

    <f7-block-title>INSET, JUST INPUTS</f7-block-title>
    <f7-list form inset>
      <f7-list-item>
        <f7-input name="name" type="text" placeholder="Name"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-input name="email" type="email" placeholder="E-mail"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-input name="gender" type="select">
          <option value="1">Male</option>
          <option value="2">Female</option>
        </f7-input>
      </f7-list-item>      
      <f7-list-item>
        <f7-input name="date" type="date" placeholder="Birth date" value="2014-04-30"></f7-input>
      </f7-list-item>
    </f7-list>    

    <f7-block-title>Form Storage</f7-block-title>
    <f7-list form id="form" store-data>
      <f7-list-item>
        <f7-label>Name</f7-label>
        <f7-input name="name" type="text" placeholder="Name"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Password</f7-label>
        <f7-input name="password" type="password" placeholder="Password"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>E-mail</f7-label>
        <f7-input name="email" type="email" placeholder="E-mail"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Birth date</f7-label>
        <f7-input name="date" type="date" placeholder="Birth date" value="2014-04-30"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Date time</f7-label>
        <f7-input name="datetime" type="datetime-local"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Gender</f7-label>
        <f7-input name="gender" type="select">
          <option value="1">Male</option>
          <option value="2">Female</option>
        </f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Switch</f7-label>
        <f7-input name="switch" type="switch" @change="onChange"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Range</f7-label>
        <f7-input type="range" min="0" max="100" step="1" value="90"></f7-input>
      </f7-list-item>
      <f7-list-item>
        <f7-label>Textarea</f7-label>
        <f7-input name="textarea" type="textarea" placeholder="Textarea"></f7-input>
      </f7-list-item>
    </f7-list>

    <f7-block-title>Checkboxes</f7-block-title>
    <f7-list form>
      <f7-list-item v-for="n in 3" :key="n" checkbox name="my-checkbox" :value="n" :title="'Checkbox ' + n"></f7-list-item>
    </f7-list>

    <f7-block-title>Radios</f7-block-title>
    <f7-list form>
      <f7-list-item v-for="n in 3" :key="n" radio name="my-radio" :checked="n === 1" :value="n" :title="'Radio ' + n"></f7-list-item>
    </f7-list>

    <div class="content-block-title">With Media Lists</div>
    <div class="list-block media-list">
      <ul>
        <li>
          <label class="label-checkbox item-content">
            <input type="checkbox" name="ks-media-checkbox" value="1"/>
            <div class="item-media"><i class="icon icon-form-checkbox"></i></div>
            <div class="item-inner">
              <div class="item-title-row">
                <div class="item-title">Facebook</div>
                <div class="item-after">17:14</div>
              </div>
              <div class="item-subtitle">New messages from John Doe</div>
              <div class="item-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sagittis tellus ut turpis condimentum, ut dignissim lacus tincidunt. Cras dolor metus, ultrices condimentum sodales sit amet, pharetra sodales eros. Phasellus vel felis tellus. Mauris rutrum ligula nec dapibus feugiat. In vel dui laoreet, commodo augue id, pulvinar lacus.</div>
            </div>
          </label>
        </li>
        <li>
          <label class="label-checkbox item-content">
            <input type="checkbox" name="ks-media-checkbox" value="2"/>
            <div class="item-media"><i class="icon icon-form-checkbox"></i></div>
            <div class="item-inner">
              <div class="item-title-row">
                <div class="item-title">John Doe (via Twitter)</div>
                <div class="item-after">17:11</div>
              </div>
              <div class="item-subtitle">John Doe (@_johndoe) mentioned you on Twitter!</div>
              <div class="item-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sagittis tellus ut turpis condimentum, ut dignissim lacus tincidunt. Cras dolor metus, ultrices condimentum sodales sit amet, pharetra sodales eros. Phasellus vel felis tellus. Mauris rutrum ligula nec dapibus feugiat. In vel dui laoreet, commodo augue id, pulvinar lacus.</div>
            </div>
          </label>
        </li>
        <li>
          <label class="label-checkbox item-content">
            <input type="checkbox" name="ks-media-checkbox" value="3"/>
            <div class="item-media"><i class="icon icon-form-checkbox"></i></div>
            <div class="item-inner">
              <div class="item-title-row">
                <div class="item-title">Facebook</div>
                <div class="item-after">16:48</div>
              </div>
              <div class="item-subtitle">New messages from John Doe</div>
              <div class="item-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sagittis tellus ut turpis condimentum, ut dignissim lacus tincidunt. Cras dolor metus, ultrices condimentum sodales sit amet, pharetra sodales eros. Phasellus vel felis tellus. Mauris rutrum ligula nec dapibus feugiat. In vel dui laoreet, commodo augue id, pulvinar lacus.</div>
            </div>
          </label>
        </li>
        <li>
          <label class="label-checkbox item-content">
            <input type="checkbox" name="ks-media-checkbox" value="4"/>
            <div class="item-media"><i class="icon icon-form-checkbox"></i></div>
            <div class="item-inner">
              <div class="item-title-row">
                <div class="item-title">John Doe (via Twitter)</div>
                <div class="item-after">15:32</div>
              </div>
              <div class="item-subtitle">John Doe (@_johndoe) mentioned you on Twitter!</div>
              <div class="item-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sagittis tellus ut turpis condimentum, ut dignissim lacus tincidunt. Cras dolor metus, ultrices condimentum sodales sit amet, pharetra sodales eros. Phasellus vel felis tellus. Mauris rutrum ligula nec dapibus feugiat. In vel dui laoreet, commodo augue id, pulvinar lacus.</div>
            </div>
          </label>
        </li>
      </ul>
    </div>
    <div class="content-block-title">What is your favourite song?</div>
    <div class="list-block media-list">
      <ul>
        <li>
          <label class="label-radio item-content">
            <input type="radio" name="ks-media-radio" value="1" checked="checked"/>
            <div class="item-media"><img src="http://lorempixel.com/160/160/fashion/1" width="80"/></div>
            <div class="item-inner">
              <div class="item-title-row">
                <div class="item-title">Yellow Submarine</div>
                <div class="item-after">$15</div>
              </div>
              <div class="item-subtitle">Beatles</div>
              <div class="item-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sagittis tellus ut turpis condimentum, ut dignissim lacus tincidunt. Cras dolor metus, ultrices condimentum sodales sit amet, pharetra sodales eros. Phasellus vel felis tellus. Mauris rutrum ligula nec dapibus feugiat. In vel dui laoreet, commodo augue id, pulvinar lacus.</div>
            </div>
          </label>
        </li>
        <li>
          <label class="label-radio item-content">
            <input type="radio" name="ks-media-radio" value="2"/>
            <div class="item-media"><img src="http://lorempixel.com/160/160/fashion/2" width="80"/></div>
            <div class="item-inner">
              <div class="item-title-row">
                <div class="item-title">Don't Stop Me Now</div>
                <div class="item-after">$22</div>
              </div>
              <div class="item-subtitle">Queen</div>
              <div class="item-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sagittis tellus ut turpis condimentum, ut dignissim lacus tincidunt. Cras dolor metus, ultrices condimentum sodales sit amet, pharetra sodales eros. Phasellus vel felis tellus. Mauris rutrum ligula nec dapibus feugiat. In vel dui laoreet, commodo augue id, pulvinar lacus.</div>
            </div>
          </label>
        </li>
        <li>
          <label class="label-radio item-content">
            <input type="radio" name="ks-media-radio" value="3"/>
            <div class="item-media"><img src="http://lorempixel.com/160/160/fashion/3" width="80"/></div>
            <div class="item-inner">
              <div class="item-title-row">
                <div class="item-title">Billie Jean</div>
                <div class="item-after">$16</div>
              </div>
              <div class="item-subtitle">Michael Jackson</div>
              <div class="item-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sagittis tellus ut turpis condimentum, ut dignissim lacus tincidunt. Cras dolor metus, ultrices condimentum sodales sit amet, pharetra sodales eros. Phasellus vel felis tellus. Mauris rutrum ligula nec dapibus feugiat. In vel dui laoreet, commodo augue id, pulvinar lacus.</div>
            </div>
          </label>
        </li>
      </ul>
    </div>

    <f7-block-title>Buttons</f7-block-title>
    <f7-block inner>
      <p><f7-button>Button</f7-button></p>
      <p><f7-button round>Button Round</f7-button></p>
      <p><f7-button fill>Button Fill</f7-button></p>
      <p>
        <f7-buttons>
          <f7-button round active>Button 1</f7-button>
          <f7-button round>Button 2</f7-button>
          <f7-button round>Button 3</f7-button>
        </f7-buttons>
      </p>
      <p>
        <f7-buttons color="orange">
          <f7-button round big>Button 1</f7-button>
          <f7-button round big active>Button 2</f7-button>
          <f7-button round big>Button 3</f7-button>
        </f7-buttons>
      </p>
      <p>
        <f7-grid>
          <f7-col><f7-button big fill color="green">Send</f7-button></f7-col>
          <f7-col><f7-button big fill color="red">Delete</f7-button></f7-col>
        </f7-grid>
      </p>
      <p>
        <f7-grid>
          <f7-col><f7-button fill raised color="green">Raised</f7-button></f7-col>
          <f7-col><f7-button raised color="red">Raised</f7-button></f7-col>
          <f7-col><f7-button fill raised color="pink">Raised</f7-button></f7-col>
        </f7-grid>
      </p>
    </f7-block>

    <div class="content-block-title">Usual Buttons</div>
    <div class="content-block">
      <div class="row">
        <div class="col-33"><a href="#" class="button active">Active</a></div>
        <div class="col-33"><a href="#" class="button">Button</a></div>
        <div class="col-33"><a href="#" class="button button-round">Round</a></div>
      </div>
    </div>
    <div class="content-block">
      <div class="row">
        <div class="col-50"><a href="#" class="button active">Active</a></div>
        <div class="col-50"><a href="#" class="button">Button</a></div>
      </div>
    </div>
    <div class="content-block">
      <div class="buttons-row"><a href="#" class="button">Button</a><a href="#" class="button">Button</a></div>
    </div>
    <div class="content-block">
      <div class="buttons-row"><a href="#" class="button button-round">Button</a><a href="#" class="button button-round">Button</a><a href="#" class="button button-round">Button</a></div>
    </div>
    <div class="content-block">
      <div class="buttons-row"><a href="#" class="button">Button</a><a href="#" class="button active">Button</a><a href="#" class="button">Button</a><a href="#" class="button">Button</a></div>
    </div>
    <div class="content-block-title">Big Buttons</div>
    <div class="content-block">
      <div class="row">
        <div class="col-50"><a href="#" class="button button-big active">Active</a></div>
        <div class="col-50"><a href="#" class="button button-big">Button</a></div>
      </div>
    </div>
    <div class="content-block-title">Themed Fill Buttons</div>
    <div class="content-block">
      <div class="row">
        <div class="col-50"><a href="#" class="button button-big button-fill color-green">Submit</a></div>
        <div class="col-50"><a href="#" class="button button-big button-fill color-red">Cancel</a></div>
      </div>
    </div>
    <div class="content-block-title">List-Block Buttons</div>
    <div class="list-block inset">
      <ul>
        <li><a href="#" class="list-button item-link">List Button 1</a></li>
        <li><a href="#" class="list-button item-link">List Button 2</a></li>
        <li><a href="#" class="list-button item-link">List Button 2</a></li>
      </ul>
    </div>
    <div class="list-block inset">
      <ul>
        <li><a href="#" class="list-button item-link color-red">Big Red Button</a></li>
      </ul>
    </div>

    
  </f7-page>
</template>
<script>
  export default {
    data: function () {
      return {
        columnStyle: 'border: 1px solid #e5e5e5; padding:5px; text-align: center'
      }
    },
    methods: {
      onChange: function (event){
        console.log('change');
      }
    }
  }
</script>
<style>
form .f7-icons {
  width: 29px;
  font-size: 29px;
  height: 29px;
  text-align: center;
  opacity: 0.5;
}
</style>