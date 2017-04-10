<template>
  <f7-page>
    <f7-navbar back-link="Back" title="Cards" sliding></f7-navbar>

    <f7-block>
      <p>Cards, along with List View, is a one more great way to contain and orginize your information. Cards contains unique related data, for example, a photo, text, and link all about a single subject. Cards are typically an entry point to more complex and detailed information.</p>
    </f7-block>
    
    <f7-block-title>Simple Cards</f7-block-title>
    <f7-card>
      <f7-card-content inner>
        This is simple card with plain text. But card could contain its own header, footer, list view, image, and any elements inside.
      </f7-card-content>
    </f7-card>


    <f7-card>
      <f7-card-header>Card header</f7-card-header>
      <f7-card-content inner> 
        Card with header and footer. Card header is used to display card title and footer for some additional information or for custom actions.
      </f7-card-content>
      <f7-card-footer>Card Footer</f7-card-footer>
    </f7-card>

    <f7-card>
      <f7-card-content inner>
        Another card. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse feugiat sem est, non tincidunt ligula volutpat sit amet. Mauris aliquet magna justo. 
      </f7-card-content>
    </f7-card>

    <f7-block-title>Styled Cards</f7-block-title>

    <f7-card class="ks-card-header-pic">
      <f7-card-header style="background-image:url(http://lorempixel.com/1000/600/nature/3/)" valign="bottom" class="color-white no-border">Journey To Mountains</f7-card-header>
      <f7-card-content inner> 
        <p class="color-gray">Posted on January 21, 2015</p>
        <p>Quisque eget vestibulum nulla. Quisque quis dui quis ex ultricies efficitur vitae non felis. Phasellus quis nibh hendrerit...</p>
      </f7-card-content>
      <f7-card-footer><a href="#" class="link">Like</a><a href="#" class="link">Read more</a></f7-card-footer>
    </f7-card>

    <div class="content-block-title">Facebook Cards</div>

    <f7-card class="ks-facebook-card">
      <f7-card-header class="no-border">
        <div class="ks-facebook-avatar"><img src="http://lorempixel.com/68/68/people/1/" width="34" height="34"/></div>
        <div class="ks-facebook-name">John Doe</div>
        <div class="ks-facebook-date">Monday at 3:47 PM</div>
      </f7-card-header>
      <f7-card-content inner="false"><img src="http://lorempixel.com/1000/700/nature/8/" width="100%"/></f7-card-content>
      <f7-card-footer class="no-border">
        <a href="#" class="link">Like</a><a href="#" class="link">Comment</a><a href="#" class="link">Share</a>
      </f7-card-footer>
    </f7-card>

    <f7-card class="ks-facebook-card">
      <f7-card-header>
        <div class="ks-facebook-avatar"><img src="http://lorempixel.com/68/68/people/1/" width="34" height="34"/></div>
        <div class="ks-facebook-name">John Doe</div>
        <div class="ks-facebook-date">Monday at 2:15 PM</div>
      </f7-card-header>
      <f7-card-content inner> 
        <p>What a nice photo i took yesterday!</p><img src="http://lorempixel.com/1000/700/nature/8/" width="100%"/>
        <p class="color-gray">Likes: 112 &nbsp;&nbsp; Comments: 43</p>
      </f7-card-content>
      <f7-card-footer>
        <a href="#" class="link">Like</a>
        <a href="#" class="link">Comment</a>
        <a href="#" class="link">Share</a>
      </f7-card-footer>
    </f7-card>

    <f7-block-title>Cards With List View</f7-block-title>

    <f7-card>
      <f7-card-content> 
        <div class="list-block">
          <ul>
            <li
              v-for="n in 5"
              :key="n">
              <a href="#" class="item-link item-content">
                <div class="item-media"><i class="icon icon-f7"></i></div>
                <div class="item-inner">
                  <div class="item-title">Link {{n}}</div>
                </div>
              </a>
            </li>
          </ul>
        </div>
      </f7-card-content>
    </f7-card>

    <f7-card>
      <f7-card-header>New Releases:</f7-card-header>
      <f7-card-content> 
        <div class="list-block media-list">
          <ul>
            <li class="item-content"
              v-for="n in 5"
              :key="n"
              >
              <div class="item-media"><img src="http://lorempixel.com/88/88/fashion/5" width="44"/></div>
              <div class="item-inner">
                <div class="item-title-row">
                  <div class="item-title">Yellow Submarine</div>
                </div>
                <div class="item-subtitle">Beatles</div>
              </div>
            </li>
          </ul>
        </div>
      </f7-card-content>
      <f7-card-footer>
        <span>January 20, 2015</span><span>5 comments</span>
      </f7-card-footer>
    </f7-card>
      
  </f7-page>
</template>
<script>
  export default {}
</script>
<style>
.ks-card-header-pic .card-header {
  height: 40vw;
  background-size: cover;
  background-position: center;
}
.ks-facebook-card .card-header {
  display: block;
  padding: 10px;
}
.ks-facebook-card .ks-facebook-avatar {
  float: left;
}
.ks-facebook-card .ks-facebook-name {
  margin-left: 44px;
  font-size: 14px;
  font-weight: 500;
}
.ks-facebook-card .ks-facebook-date {
  margin-left: 44px;
  font-size: 13px;
  color: #8e8e93;
}
.ks-facebook-card .card-footer {
  background: #fafafa;
}
.ks-facebook-card .card-footer a {
  color: #81848b;
  font-weight: 500;
}
.ks-facebook-card .card-content img {
  display: block;
}
.ks-facebook-card .card-content-inner {
  padding: 15px 10px;
}
</style>