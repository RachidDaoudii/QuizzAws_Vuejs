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
                          <h4>AWS - Quiz</h4><span>( 10 of 10)</span>
                        </div>
                    </div>
                    <div class="question bg-white p-3 border-bottom">
                      <div class="ans ml-2">
                        <p>
                          We have prepared AWS Cloud Practitioner (CLF-C01) certification sample questions to make you aware of actual exam properties. This sample question set provides you with information about the Cloud Practitioner exam pattern, question formate, a difficulty level of questions and time required to answer each question. To get familiar with AWS Certified Cloud Practitioner exam, we suggest you try our <b>Sample AWS CLF-C01 Certification Practice Exam</b> in simulated AWS certification exam environment.
                          To test your knowledge and understanding of concepts with real-time scenario based AWS CLF-C01 questions, we strongly recommend you to prepare and practice with <b>Premium AWS Cloud Practitioner Certification Practice Exam</b>. The premium AWS Cloud Practitioner certification practice exam helps you identify topics in which you are well prepared and topics in which you may need further training to achieving great score in actual AWS     Certified Cloud Practitioner exam.
                        </p>
                        
                      </div>
                    </div>
                    <div class="d-flex flex-row justify-content-center align-items-center p-3 bg-white">
                      <button class="btn btn-primary border-success align-items-center btn-success"
                      @click="execute"
                      >Start
                      </button>

                    </div>
                </div>
            </div>
        </div>
    </div>
  </template>

<script >
export default {
    props: {
      callback: {
        type: Function
      }
    },

    methods: {
      execute() {
        if (this.callback) {
          this.callback()
        }
      },
    //   handleClick() {
    //   console.log('Button clicked!');
    // },

    // autoClickButton() {
    //   this.$nextTick(() => {
    //     this.$refs.myButton.click();
    //   });
    // }
    }
}
</script>