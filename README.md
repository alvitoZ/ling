<svg
        width="20"
        height="22"
        viewBox="0 0 20 22"
        stroke="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M0.500397 7.86013L9.5004 13.0601C9.65242 13.1479 9.82486 13.1941 10.0004 13.1941C10.1759 13.1941 10.3484 13.1479 10.5004 13.0601L19.5004 7.86013C19.6515 7.77287 19.7772 7.64758 19.8649 7.49671C19.9526 7.34584 19.9993 7.17464 20.0004 7.00013C20.0011 6.82392 19.9552 6.65065 19.8674 6.49787C19.7796 6.3451 19.653 6.21823 19.5004 6.13013L10.5004 0.940127C10.3484 0.852359 10.1759 0.806152 10.0004 0.806152C9.82486 0.806152 9.65242 0.852359 9.5004 0.940127L0.500397 6.13013C0.347792 6.21823 0.221178 6.3451 0.133375 6.49787C0.0455716 6.65065 -0.000302856 6.82392 0.000396711 7.00013C0.00145008 7.17464 0.0481556 7.34584 0.135871 7.49671C0.223587 7.64758 0.349259 7.77287 0.500397 7.86013ZM10.0004 3.00013L17.0004 7.00013L10.0004 11.0001L3.0004 7.00013L10.0004 3.00013ZM18.5004 10.1701L10.0004 15.0001L1.5004 10.1301C1.38626 10.064 1.26018 10.0211 1.1294 10.0039C0.998619 9.98676 0.865733 9.99561 0.738393 10.03C0.611053 10.0644 0.491775 10.1236 0.387428 10.2043C0.283081 10.285 0.195727 10.3855 0.130397 10.5001C2.43336e-05 10.7297 -0.0342419 11.0016 0.0350749 11.2564C0.104392 11.5112 0.271665 11.7282 0.500397 11.8601L9.5004 17.0601C9.65242 17.1479 9.82486 17.1941 10.0004 17.1941C10.1759 17.1941 10.3484 17.1479 10.5004 17.0601L19.5004 11.8601C19.7291 11.7282 19.8964 11.5112 19.9657 11.2564C20.035 11.0016 20.0008 10.7297 19.8704 10.5001C19.8051 10.3855 19.7177 10.285 19.6134 10.2043C19.509 10.1236 19.3897 10.0644 19.2624 10.03C19.1351 9.99561 19.0022 9.98676 18.8714 10.0039C18.7406 10.0211 18.6145 10.064 18.5004 10.1301V10.1701ZM18.5004 14.1701L10.0004 19.0001L1.5004 14.1301C1.38626 14.064 1.26018 14.0211 1.1294 14.0039C0.998619 13.9868 0.865733 13.9956 0.738393 14.03C0.611053 14.0644 0.491775 14.1236 0.387428 14.2043C0.283081 14.285 0.195727 14.3855 0.130397 14.5001C2.43336e-05 14.7297 -0.0342419 15.0016 0.0350749 15.2564C0.104392 15.5112 0.271665 15.7282 0.500397 15.8601L9.5004 21.0601C9.65242 21.1479 9.82486 21.1941 10.0004 21.1941C10.1759 21.1941 10.3484 21.1479 10.5004 21.0601L19.5004 15.8601C19.7291 15.7282 19.8964 15.5112 19.9657 15.2564C20.035 15.0016 20.0008 14.7297 19.8704 14.5001C19.8051 14.3855 19.7177 14.285 19.6134 14.2043C19.509 14.1236 19.3897 14.0644 19.2624 14.03C19.1351 13.9956 19.0022 13.9868 18.8714 14.0039C18.7406 14.0211 18.6145 14.064 18.5004 14.1301V14.1701Z"
          fill={`${onClick ? color : "#131613"}`}
        />
      </svg>

https://www.figma.com/file/RtZSvvmrGzYHdDbSnfyG3H/WEDDING-ORGANIZER?type=design&node-id=7%3A463&mode=design&t=ekMU9VSAUj3w2Rho-1

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
