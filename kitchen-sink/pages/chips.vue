<template>
  <f7-page>
    <f7-navbar back-link="Back" title="Chips" sliding></f7-navbar>

    <f7-block>
      <p>Chips/Tags represent complex entities in small blocks, such as a contact. They can contain a photo, short title string, and brief information.</p>
    </f7-block>

    <f7-block-title>Chips With Text</f7-block-title>
    <f7-block inner>
      <f7-chip text="Example Chip"></f7-chip>
      <f7-chip text="Another Chip" bg="red"></f7-chip>
      <f7-chip text="One More Chip" bg="green"></f7-chip>
      <f7-chip text="Fourth Chip" bg="orange"></f7-chip>
      <f7-chip text="Last Chip"></f7-chip>
    </f7-block>

    <f7-block-title>Icon Chips</f7-block-title>
    <f7-block inner>
      <f7-chip text="Add Contact" media='<i class="icon f7-icons">add_round</i>'></f7-chip>
      <f7-chip text="London" media='<i class="icon f7-icons">compass</i>'></f7-chip>
      <f7-chip text="John Doe" media='<i class="icon f7-icons">person</i>'></f7-chip>
    </f7-block>

    <f7-block-title>Contact Chips</f7-block-title>
    <f7-block inner>
      <f7-chip text="Jane Doe" media='<img src="http://lorempixel.com/100/100/people/9/"/>'></f7-chip>
      <f7-chip text="Jane Doe" media='<img src="http://lorempixel.com/100/100/people/3/"/>'></f7-chip>
      <f7-chip text="Adam Smith" media='<img src="http://lorempixel.com/100/100/people/7/"/>'></f7-chip>
      <f7-chip text="Jennifer" mediaBg="pink" media='J'></f7-chip>
      <f7-chip text="Chris" mediaBg="yellow" mediaColor="black" media='C'></f7-chip>
      <f7-chip text="Kate" mediaBg="red" media='K'></f7-chip>
    </f7-block>

    <f7-block-title>Deletable Chips / Tags</f7-block-title>
    <f7-block inner>
      <f7-chip text="Example Chip" deleteable @delete="onChipDelete"></f7-chip>
      <f7-chip text="Chris" mediaBg="orange" mediaColor="black" media='C' deleteable @delete="onChipDelete"></f7-chip>
      <f7-chip text="Jane Doe" media='<img src="http://lorempixel.com/100/100/people/9/"/>' deleteable @delete="onChipDelete"></f7-chip>
      <f7-chip text="One More Chip" deleteable @delete="onChipDelete"></f7-chip>
      <f7-chip text="Jennifer" mediaBg="pink" media='J' deleteable @delete="onChipDelete"></f7-chip>
      <f7-chip text="Adam Smith" media='<img src="http://lorempixel.com/100/100/people/7/"/>' deleteable @delete="onChipDelete"></f7-chip>
    </f7-block>

  </f7-page>
</template>
<script>
  export default {
    methods: {
      onChipDelete: function (event){
        console.log('chip-delete');
      }
    }
  }
</script>