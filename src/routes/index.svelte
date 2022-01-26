<script lang=ts>
  import { colorParsley } from 'colorparsley'
  import { calcAPCA } from 'apca-w3'
   let colorOne:string = ''
   let colorTwo:string = ''

   console.log(calcAPCA('#000','#fff'))
</script>

<div>
  <div class="box" style:background-color={colorOne}></div>
  <label for="color-one">Color One: {colorOne}</label>
  <input type="text" name="color-one" bind:value={colorOne}>

  <div class="box" style:background-color={colorTwo}></div>
  <label for="color-two">Color Two: {colorTwo}</label>
  <input type="text" name="color-two" bind:value={colorTwo}>
</div>

<style>
  .box {
    width: 150px;
    height: 150px;
  }

</style>
