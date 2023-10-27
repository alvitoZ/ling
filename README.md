https://stackoverflow.com/questions/66193180/how-to-read-the-output-tensor-tflite-in-android-studio

https://www.tensorflow.org/lite/guide/inference?hl=id

https://www.tensorflow.org/lite/android/play_services?hl=id#kotlin_2

https://www.tensorflow.org/lite/android/delegates/gpu?hl=id


https://www.tensorflow.org/lite/android/delegates/gpu?hl=en


    implementation("org.tensorflow:tensorflow-lite:2.7.0")
    implementation("org.tensorflow:tensorflow-lite-support:0.1.0")
    implementation("org.tensorflow:tensorflow-lite-metadata:0.1.0")
    implementation("org.tensorflow:tensorflow-lite-gpu:2.3.0")

// import org.tensorflow.lite.DataType
// import org.tensorflow.lite.Interpreter
// import org.tensorflow.lite.gpu.GpuDelegate
// import org.tensorflow.lite.gpu.CompatibilityList
// import org.tensorflow.lite.support.tensorbuffer.TensorBuffer
// import java.io.File
// fun main(): Unit {
//     val compatlist = CompatibilityList()

//     val options = Interpreter.Options().apply {
//         if(compatlist.isDelegateSupportedOnThisDevice){
//             val delegateOptions = compatlist.bestOptionsForThisDevice
//             this.addDelegate(GpuDelegate(delegateOptions))
//         }else{
//             this.setNumThreads(4)
//         }
//     }
//     val interpreter = Interpreter(File("../ml/model4.tflite"), options)
//     val inputFeature0 = TensorBuffer.createFixedSize(intArrayOf(1, 10), DataType.FLOAT32)
//     val input =  inputFeature0.loadArray(floatArrayOf(566F, 12F, 12F, -12F, 1F, 7F, 1F, 1F, 1F, -1F))
//     val output = interpreter.getOutputTensor(1)
//     interpreter.run(input,output)

//     println("kita ikuyo")

// }
