<template>
    <result-component>
      <div class="container mt-5">
        <div class="d-flex justify-content-center row">
              <div class="logo d-flex justify-content-center">
                <img class="w-50" src="../assets/img/logo.png" alt="">
              </div>
            <div class="col-md-10 col-lg-10">
                <div class="border">
                    <div class="question bg-white p-3 border-bottom">
                        <div class="d-flex flex-row justify-content-between align-items-center mcq">
                          <h4>Aws Quiz</h4><span>(10 of 10)</span>
                        </div>
                    </div>
                    <div class="question bg-white p-3 border-bottom">
                        <div class="ans ml-2">
                          <label class="radio"> <input type="radio" name="brazil" value="brazil"> <span>Brazil</span>
                          </label>    
                        </div>
                        <div class="ans ml-2">
                          <label class="radio"> <input type="radio" name="Germany" value="Germany"> <span>Germany</span>
                          </label>    
                        </div>
                        <div class="ans ml-2">
                          <label class="radio"> <input type="radio" name="Indonesia" value="Indonesia"> <span>Indonesia</span>
                          </label>    
                        </div>
                        <div class="ans ml-2">
                          <label class="radio"> <input type="radio" name="Russia" value="Russia"> <span>Russia</span>
                          </label>    
                        </div>
                    </div>
                    <!-- <div class="d-flex flex-row justify-content-center align-items-center p-3 bg-white">
                      <button class="btn btn-primary d-flex align-items-center btn-danger" type="button">
                        <i class="fa fa-angle-left mt-1 mr-1"></i>&nbsp;previous</button>
                      <button class="btn btn-primary border-success align-items-center btn-success" type="button">Next<i class="fa fa-angle-right ml-2"></i>
                      </button>
                    </div> -->
                </div>
            </div>
        </div>
    </div>
  </result-component>
</template>
<script>
export default {
  name: 'ChildComponent',
  props: {
    items: {
      type: Array,
      required: true
    }
  }
};
</script>

<style scoped>
.logo{
  width: 360px;
}
</style>