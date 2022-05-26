<template>
    <div>

  <div id="FormGear-loader" class="bg-gray-200  dark:bg-[#181f30]">

    <div class=" md:max-w-6xl mx-auto md:px-8 md:py-8">
      <div
        class="bg-gray-50 dark:bg-gray-900 dark:text-white text-gray-600 flex overflow-hidden text-sm font-montserrat rounded-lg shadow-xl dark:shadow-gray-800">
        
        
        <div class=" flex-grow flex flex-col bg-white dark:bg-gray-900 z-0">

          <div class="relative  md:flex   ">

            
            <div class="block">
              <div class=" backdrop-blur-sm col-span-12 overflow-x-hidden overflow-y-auto fixed inset-0 z-50 outline-none focus:outline-none flex justify-center items-center">
                <svg class="w-20 h-20 animate-spin" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 94.53 98.372"><circle cx="23.536" cy="16.331" r="8.646" style="fill:#0a77e8"/><circle cx="8.646" cy="36.698" r="8.646" style="fill:#0f9af0"/><circle cx="8.646" cy="61.867" r="8.646" style="fill:#0f9af0"/><circle cx="23.536" cy="82.233" r="8.646" style="fill:#13bdf7"/><circle cx="47.361" cy="89.726" r="8.646" style="fill:#13bdf7"/><circle cx="71.282" cy="82.233" r="8.646" style="fill:#18e0ff"/><circle cx="85.884" cy="61.867" r="8.646" style="fill:#65eaff"/><circle cx="85.884" cy="36.698" r="8.646" style="fill:#b2f5ff"/><circle cx="47.361" cy="8.646" r="8.646" style="fill:#1d4970"/></svg>
                <!-- <img src="./src/assets/loading.png" alt="Loading..." class="w-20 h-20 animate-spin" loading="lazy" />    -->
              </div>
              <!-- <div class="col-span-12 overflow-x-hidden overflow-y-auto fixed inset-0 z-50 outline-none focus:outline-none flex justify-center items-center text-center font-extralight text-xs">
                Mohon menunggu,<br> data sedang dalam proses
              </div> -->
            </div>

            <div
              class="bg-gray-50 dark:bg-gray-900 w-72 flex-shrink-0  dark:border-gray-800 h-full  p-5 space-y-4
              absolute inset-y-0 left-0 transform -translate-x-full transition-transform duration-500 ease-in-out md:relative md:translate-x-0 z-10">

              <div class="animate-pulse flex space-x-4">
                <div class="flex-1 space-y-3 py-1">
                  <div class="w-full  shadow-2xl rounded-lg">

                    <div class="h-32 bg-gray-200 rounded-tr-lg rounded-tl-lg animate-pulse"></div>

                    <div class="p-5">
                      <div class="h-20 px-2 rounded-lg bg-gray-200 animate-pulse mb-4"></div>
                      <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-10 mb-4"></div>
                      <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-4 mb-4"></div>
                      <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-4 mb-4"></div>

                      <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-10 mb-4"></div>
                      <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-4 mb-4"></div>
                      <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-4 mb-4"></div>

                      <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-10 mb-4"></div>
                      <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-4 mb-4"></div>
                      <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-4 mb-4"></div>

                      <div class="h-20 px-2 rounded-lg bg-gray-200 animate-pulse mt-10 mb-4"></div>
                    </div>

                  </div>
                </div>
              </div>

            </div>

            <div class="flex-grow bg-white dark:bg-gray-900 transition duration-500 ease-in-out z-10 p-5 space-y-4
              ">

              <div class="flex-grow bg-white dark:bg-gray-900 ">
                <div class=" w-full mx-auto">
                  <div class="animate-pulse flex space-x-4">
                    <div class="flex-1 space-y-3 py-1">
                      <div
                        class="min-h-screen flex items-start justify-start bg-gradient-to-br from-gray-200 to-gray-400">
            
                        <div class="w-full bg-white  shadow-2xl rounded-lg">

                          <div class="h-32 bg-gray-200 rounded-tr-lg rounded-tl-lg animate-pulse"></div>

                          <div class="p-5">
                            <div class="h-20 px-2 rounded-lg bg-gray-200 animate-pulse mb-4"></div>
                            <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-10 mb-4"></div>
                            <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-4 mb-4"></div>
                            <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-4 mb-4"></div>

                            <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-10 mb-4"></div>
                            <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-4 mb-4"></div>
                            <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-4 mb-4"></div>

                            <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-10 mb-4"></div>
                            <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-4 mb-4"></div>
                            <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-4 mb-4"></div>

                            <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-10 mb-4"></div>
                            <div class="h-6 rounded-lg bg-gray-200 animate-pulse mt-4 mb-4"></div>
                          </div>

                        </div>

                      </div>

                    </div>
                  </div>
                </div>
              </div>

            </div>



          </div>

        </div>
      </div>
    </div>

  </div>

      <div id="FormGear-root"></div>

    </div>
</template>

<script type="module">
import { FormGear } from "form-gear"
import "form-gear/dist/style.css"
import reference from "./data/reference"
import template from "./data/template"
import preset from "./data/preset.json"
import response from "./data/response.json"
import validation from "./data/validation.json"
import remark from "./data/remark.json"

function initForm(reference,  template, preset, response, validation, remark){

//variable config
let config = {
  clientMode: 1, // 1 => CAWI ; 2 => CAPI ;
  //both token and baseUrl are used for data lookup from the api (for selectInput, multiselect Input, and listSelectInput)
  token: ``, //for authentication such as bearer token 
  baseUrl: `https://jsonplaceholder.typicode.com/users/`, // endpoint to fetch
  lookupKey: `key%5B%5D`, //optional 
  lookupValue: `value%5B%5D`, //optional
  lookupMode : 1, // 1 => ONLINE ; 2 => OFFLINE
  username: 'AdityaSetyadi', //
  formMode: 1, // 1 => OPEN ; 2 => REJECTED ; 3 => SUBMITTED ; 4 => APPROVED ;
  initialMode: 2 // 1=> INITIAL ; 2 => ASSIGN
}
    
//some variables initiation
var cameraFunction = null;
var cameraGPSFunction = null;
var responseGear = null;
var remarkGear = null;
var principalGear = null;
var referenceGear = null;
    
    let uploadHandler = function (setter) {
    // console.log('camera handler', setter);
    // cameraFunction = setter;
    // openCamera();
    }

    let offlineSearch = function (id, version, dataJson, setter) {
  
  let condition = JSON.stringify(dataJson)

  //here we use jquery to retrieve data from the local device
  $.ajax({
    url: `http://localhost:9090/lookup?id=${id}&v=${version}&c=${condition}`,//specify localhost endpoint to fetch
    type: "GET",
    crossDomain: true,
    dataType: "json",
    data: null,
    success: function(d) {
        console.log(d.hasil)
        setter(d)

        },
    error: function(XMLHttpRequest, textStatus, errorThrown) {

    }
});

}

    let GpsHandler = function (setter, isPhoto) {
    // console.log('camera handler', setter);
    // isPhoto = true,
    // cameraGPSFunction = setter;
    // openCameraGPS(isPhoto);
    }

        const setBearer = () => {
    return ({
        method: 'GET',
        headers: {
        "Content-Type": "application/json",
        "Authorization": "Bearer " + config.token
        }
    })
    }

    //custom function to trigger setResponsMobile to run from outside form-gear, you can custom the function name 
let mobileExit = (fun) => {
  // fun()
}

    // pencarian online
//online lookup
let onlineSearch = async (url) =>
(await fetch(url, setBearer())
  .catch((error) => {
    return {
      success: false,
      data: {},
      message: '500'
    }
  }).then((res) => {
    /*the return format must in object of 
      {
        success: false, => true or false
        data: {}, --> the data property must in format array of object [{value: {value}, label : {label}}, ...]
        message: status (200, 400 ,500 , etc )
      }
    }*/
  return {
    success: true,
    data: [{}],
    message: 200
  }

  }));



//function to get response, remark, principal and reference
let setResponseMobile = function (res, rem, princ, ref) {
  // responseGear = res
  // remarkGear = rem
  // principalGear = princ
  // referenceGear = ref

  // console.log('----------', new Date(), '----------');

  // console.log('response', responseGear)
  // console.log('remark', remarkGear)
  // console.log('principal', principalGear)
  // console.log('reference', referenceGear)
}

let setSubmitMobile = function (res, rem, princ, ref) {
  // responseGear = res
  // remarkGear = rem
  // principalGear = princ
  // referenceGear = ref
  
  // console.log('----------', new Date(), '----------');

  // console.log('response', responseGear)
  // console.log('remark', remarkGear)
  // console.log('principal', principalGear)
  // console.log('reference', referenceGear)
}


    let openMap = function (koordinat) {
    // koordinat = koordinat

    // console.log('coordinat ', koordinat)
    }

    let form = FormGear(reference, template, preset, response, validation, remark, config, uploadHandler, GpsHandler, offlineSearch, onlineSearch, mobileExit, setResponseMobile, setSubmitMobile, openMap);

    return form;
}

const data = Promise.all([
    reference, template, preset, response, validation, remark
]);

data.then(([reference, template, preset, response, validation, remark]) => initForm(reference, template, preset, response, validation, remark));

</script>