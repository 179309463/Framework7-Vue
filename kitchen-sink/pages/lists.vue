<template>
  <f7-page>
    <f7-navbar back-link="Back" title="Lists" sliding></f7-navbar>

    <f7-block-title>List</f7-block-title>
    <f7-list>
      <f7-list-item
        v-for="n in 5"
        :key="n"
        :title="n === 3 ? 'Divider' : 'Item ' + n"
        badge="3"
        badge-color="red"
        :divider="n === 3"
      ></f7-list-item>
      <f7-list-label>Hello I'm List Label</f7-list-label>
    </f7-list>

    <f7-block-title>Grouped List</f7-block-title>
    <f7-list>
      <f7-list-group v-for="n in 2" :key="n">
        <f7-list-item
          v-for="n in 3"
          :key="n"
          :title="n === 1 ? 'Group Title' : 'Group Item ' + (n - 1)"
          :group-title="n === 1"
        ></f7-list-item>
      </f7-list-group>
      <f7-list-label>Hello I'm List Label</f7-list-label>
    </f7-list>

    <f7-block-title>Buttons List</f7-block-title>
    <f7-list inset>
      <f7-list-button v-for="n in 3" :key="n" :title="'List Button ' + n" link="http://google.com"></f7-list-button>
    </f7-list>

    <div class="content-block">
      <p>Framework7 allows you to be flexible with list views (table views). You can make them as navigation menus, you can use there icons, inputs, and any elements inside of the list, and even make them nested:</p>
    </div>
    <div class="content-block-title">Data list, with icons</div>
    <div class="list-block">
      <ul>
        <li>
          <div class="item-content">
            <div class="item-media"><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">Ivan Petrov</div>
              <div class="item-after">CEO</div>
            </div>
          </div>
        </li>
        <li>
          <div class="item-content">
            <div class="item-media"><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">John Doe</div>
              <div class="item-after"> <span class="badge">5</span></div>
            </div>
          </div>
        </li>
        <li>
          <div class="item-content">
            <div class="item-media"><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">Jenna Smith</div>
            </div>
          </div>
        </li>
      </ul>
    </div>
    <div class="content-block-title">Links</div>
    <div class="list-block">
      <ul>
        <li><a href="#" class="item-link item-content">
            <div class="item-media"><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">Ivan Petrov</div>
              <div class="item-after">CEO</div>
            </div></a></li>
        <li><a href="#" class="item-link item-content">
            <div class="item-media"><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">John Doe</div>
              <div class="item-after">Cleaner</div>
            </div></a></li>
        <li><a href="#" class="item-link item-content">
            <div class="item-media"><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">Jenna Smith</div>
            </div></a></li>
      </ul>
    </div>
    <div class="content-block-title">Links, no icons</div>
    <div class="list-block">
      <ul>
        <li><a href="#" class="item-link item-content">
            <div class="item-inner"> 
              <div class="item-title">Ivan Petrov</div>
            </div></a></li>
        <li><a href="#" class="item-link item-content">
            <div class="item-inner"> 
              <div class="item-title">John Doe</div>
            </div></a></li>
        <li>
          <div class="item-divider">Divider Here</div>
        </li>
        <li><a href="#" class="item-link item-content">
            <div class="item-inner"> 
              <div class="item-title">Ivan Petrov</div>
            </div></a></li>
        <li><a href="#" class="item-link item-content">
            <div class="item-inner"> 
              <div class="item-title">Jenna Smith</div>
            </div></a></li>
      </ul>
    </div>
    <div class="content-block-title">Grouped with sticky titles</div>
    <div class="list-block">
      <div class="list-group">
        <ul>
          <li class="list-group-title">A</li>
          <li>
            <div class="item-content">
              <div class="item-inner">
                <div class="item-title">Aaron </div>
              </div>
            </div>
          </li>
          <li>
            <div class="item-content">
              <div class="item-inner">
                <div class="item-title">Abbie</div>
              </div>
            </div>
          </li>
          <li>
            <div class="item-content">
              <div class="item-inner">
                <div class="item-title">Adam</div>
              </div>
            </div>
          </li>
        </ul>
      </div>
      <div class="list-group">
        <ul>
          <li class="list-group-title">B</li>
          <li>
            <div class="item-content">
              <div class="item-inner">
                <div class="item-title">Bailey</div>
              </div>
            </div>
          </li>
          <li>
            <div class="item-content">
              <div class="item-inner">
                <div class="item-title">Barclay</div>
              </div>
            </div>
          </li>
          <li>
            <div class="item-content">
              <div class="item-inner">
                <div class="item-title">Bartolo</div>
              </div>
            </div>
          </li>
        </ul>
      </div>
      <div class="list-group">
        <ul>
          <li class="list-group-title">C</li>
          <li>
            <div class="item-content">
              <div class="item-inner">
                <div class="item-title">Caiden</div>
              </div>
            </div>
          </li>
          <li>
            <div class="item-content">
              <div class="item-inner">
                <div class="item-title">Calvin</div>
              </div>
            </div>
          </li>
          <li>
            <div class="item-content">
              <div class="item-inner">
                <div class="item-title">Candy</div>
              </div>
            </div>
          </li>
        </ul>
      </div>
    </div>
    <div class="content-block-title">Mixed and nested</div>
    <div class="list-block">
      <ul>
        <li><a href="#" class="item-link item-content">
            <div class="item-media"><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">Ivan Petrov</div>
              <div class="item-after">CEO</div>
            </div></a></li>
        <li><a href="#" class="item-link item-content">
            <div class="item-media"><i class="icon icon-f7"></i><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">Two icons here</div>
            </div></a></li>
        <li>
          <div class="item-content">
            <div class="item-inner"> 
              <div class="item-title">No icons here</div>
            </div>
          </div>
          <ul>
            <li><a href="#" class="item-link item-content">
                <div class="item-media"><i class="icon icon-f7"></i></div>
                <div class="item-inner"> 
                  <div class="item-title">Ivan Petrov</div>
                  <div class="item-after">CEO</div>
                </div></a></li>
            <li><a href="#" class="item-link item-content">
                <div class="item-media"><i class="icon icon-f7"></i><i class="icon icon-f7"></i></div>
                <div class="item-inner"> 
                  <div class="item-title">Two icons here</div>
                </div></a></li>
            <li>
              <div class="item-content">
                <div class="item-inner"> 
                  <div class="item-title">No icons here</div>
                </div>
              </div>
            </li>
            <li><a href="#" class="item-link item-content">
                <div class="item-media"><i class="icon icon-f7"></i></div>
                <div class="item-inner"> 
                  <div class="item-title">Ultra long text goes here, no, it is really really long</div>
                </div></a></li>
            <li>
              <div class="item-content">
                <div class="item-media"><i class="icon icon-f7"></i></div>
                <div class="item-inner"> 
                  <div class="item-title">With switch</div>
                  <div class="item-after">
                    <label class="label-switch">
                      <input type="checkbox"/>
                      <div class="checkbox"></div>
                    </label>
                  </div>
                </div>
              </div>
            </li>
          </ul>
        </li>
        <li><a href="#" class="item-link item-content">
            <div class="item-media"><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">Ultra long text goes here, no, it is really really long</div>
            </div></a></li>
        <li>
          <div class="item-content">
            <div class="item-media"><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">With switch</div>
              <div class="item-after">
                <label class="label-switch">
                  <input type="checkbox"/>
                  <div class="checkbox"></div>
                </label>
              </div>
            </div>
          </div>
        </li>
      </ul>
    </div>
    <div class="content-block-title">Mixed, inset</div>
    <div class="list-block inset">
      <ul>
        <li><a href="#" class="item-link item-content">
            <div class="item-media"><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">Ivan Petrov</div>
              <div class="item-after">CEO</div>
            </div></a></li>
        <li><a href="#" class="item-link item-content">
            <div class="item-media"><i class="icon icon-f7"></i><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">Two icons here</div>
            </div></a></li>
        <li><a href="#" class="item-link item-content">
            <div class="item-media"><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">Ultra long text goes here, no, it is really really long</div>
            </div></a></li>
        <li>
          <div class="item-content">
            <div class="item-media"><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">With switch</div>
              <div class="item-after">
                <label class="label-switch">
                  <input type="checkbox"/>
                  <div class="checkbox"></div>
                </label>
              </div>
            </div>
          </div>
        </li>
      </ul>
      <div class="list-block-label">
        <p>Here comes some useful information about list above</p>
      </div>
    </div>
    <div class="content-block-title">Tablet inset</div>
    <div class="list-block tablet-inset">
      <ul>
        <li><a href="#" class="item-link item-content">
            <div class="item-media"><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">Ivan Petrov</div>
              <div class="item-after">CEO</div>
            </div></a></li>
        <li><a href="#" class="item-link item-content">
            <div class="item-media"><i class="icon icon-f7"></i><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">Two icons here</div>
            </div></a></li>
        <li><a href="#" class="item-link item-content">
            <div class="item-media"><i class="icon icon-f7"></i></div>
            <div class="item-inner"> 
              <div class="item-title">Ultra long text goes here, no, it is really really long</div>
            </div></a></li>
      </ul>
      <div class="list-block-label">
        <p>This list block will look like "inset" only on tablets (iPad)</p>
      </div>
    </div>

  </f7-page>
</template>
<script>
  export default {}
</script>
