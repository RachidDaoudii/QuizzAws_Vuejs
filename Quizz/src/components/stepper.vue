<template>
  <div class="row">
    <div class="col-xs-12 col-md-8 offset-md-2 block">
      <div class="wrapper-progressBar">
        <ul class="progressBar">
          <li class="active">Info</li>
          <li :class="{active:stp}">Quiz</li>
          <li :class="{active:stp == 2 }">Result</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped>
.wrapper-progressBar {
    width: 100%
}

.progressBar li {
    list-style-type: none;
    float: left;
    width: 33%;
    position: relative;
    text-align: center;
}

.progressBar li:before {
    content: " ";
    line-height: 30px;
    border-radius: 50%;
    width: 30px;
    height: 30px;
    border: 1px solid #ddd;
    display: block;
    text-align: center;
    margin: 0 auto 10px;
    background-color: white
}

.progressBar li:after {
    content: "";
    position: absolute;
    width: 100%;
    height: 2px;
    background-color: #ddd;
    top: 15px;
    left: -50%;
    z-index: -1;
}

.progressBar li:first-child:after {
    content: none;
}

.progressBar li.active {
    color: dodgerblue;
}

.progressBar li.active:before {
    border-color: dodgerblue;
    background-color: dodgerblue
}

.progressBar li.active:after {
    background-color: dodgerblue;
}

</style>
<script>
export default {
  props: ['stp']
}
</script>
