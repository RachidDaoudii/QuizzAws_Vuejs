<template>
    <div class="container mt-5 start">
        <div class="d-flex justify-content-center row">
              <div class="logo d-flex justify-content-center">
                <img class="w-25" src="../assets/img/logo.png"  alt="">
              </div>
            <div class="col-md-10 col-lg-10">
                <div class="border">
                    <div class="question bg-white p-3 border-bottom">
                        <div class="d-flex flex-row justify-content-between align-items-center mcq">
                          <h4>Quiz</h4><span>(  of 10)</span>
                        </div>
                    </div>
                    <div class="question bg-white p-3 border-bottom"
                    
                    >
                        <div class="d-flex flex-row align-items-center question-title"
                     @click="Start()">
                            <h3 class="text-danger px-4">Q.mkùmk</h3>
                            <h5 class="mt-1 ml-2">kjh</h5>
                        </div>
                        <div class="ans ml-2"
                        >
                            
                        </div>
                    </div>
                    <div class="d-flex flex-row justify-content-center align-items-center p-3 bg-white">
                      <button class="btn btn-primary border-success align-items-center btn-success"
                      
                     @click="Start()"
                    
                      >Start
                      </button>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </template>

  <script setup>
const Start = ()=>{
    seen: true
}
</script>