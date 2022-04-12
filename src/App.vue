<template>
    <div>

      <div id="FormGear-loader" class="bg-gray-200  dark:bg-[#181f30] ">
        
        <div class=" md:max-w-6xl mx-auto md:px-8 md:py-8">
          <div class="bg-gray-50 dark:bg-gray-900 dark:text-white text-gray-600 flex overflow-hidden text-sm font-montserrat rounded-lg shadow-xl dark:shadow-gray-800">
            <div class=" flex-grow flex flex-col bg-white dark:bg-gray-900 z-0" >
              
              <div class="relative  md:flex   ">

                <div class="bg-gray-50 dark:bg-gray-900 w-72 flex-shrink-0  dark:border-gray-800 h-full  p-5 space-y-4
                absolute inset-y-0 left-0 transform -translate-x-full transition-transform duration-500 ease-in-out md:relative md:translate-x-0 z-10">

                <div class="animate-pulse flex space-x-4">
                  <div class="flex-1 space-y-3 py-1">
                    <div class="w-full  shadow-2xl rounded-lg">
                                  
                      <div class="h-32 bg-gray-100 rounded-tr-lg rounded-tl-lg animate-pulse"></div>

                      <div class="p-5">
                        <div class="h-20 px-2 rounded-lg bg-gray-100 animate-pulse mb-4"></div>
                        <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-10 mb-4"></div>
                        <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-4 mb-4"></div>
                        <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-4 mb-4"></div>
                        
                        <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-10 mb-4"></div>
                        <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-4 mb-4"></div>
                        <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-4 mb-4"></div>

                        <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-10 mb-4"></div>
                        <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-4 mb-4"></div>
                        <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-4 mb-4"></div>
                        
                        <div class="h-20 px-2 rounded-lg bg-gray-100 animate-pulse mt-10 mb-4"></div>
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
                          <div class="min-h-screen flex items-start justify-start bg-gradient-to-br from-gray-200 to-gray-400">
                            
                            <div class="w-full bg-white  shadow-2xl rounded-lg">
                              
                              <div class="h-32 bg-gray-100 rounded-tr-lg rounded-tl-lg animate-pulse"></div>

                              <div class="p-5">
                                <div class="h-20 px-2 rounded-lg bg-gray-100 animate-pulse mb-4"></div>
                                <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-10 mb-4"></div>
                                <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-4 mb-4"></div>
                                <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-4 mb-4"></div>
                                
                                <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-10 mb-4"></div>
                                <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-4 mb-4"></div>
                                <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-4 mb-4"></div>

                                <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-10 mb-4"></div>
                                <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-4 mb-4"></div>
                                <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-4 mb-4"></div>
                                
                                <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-10 mb-4"></div>
                                <div class="h-6 rounded-lg bg-gray-100 animate-pulse mt-4 mb-4"></div>
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
import template from "./data/template"
import preset from "./data/preset.json"
import response from "./data/response.json"
import validation from "./data/validation.json"
import remark from "./data/remark.json"

function initForm(template, preset, response, validation, remark){

    let config = {
    clientMode: 1, // CAWI = 1, CAPI = 2
    token: `aeyJ0eXA`,
    baseUrl: `https://api-survey.bps.go.id/designer/api/lookup-data/json`,
    lookupKey: `key%5B%5D`,
    lookupValue: `value%5B%5D`,
    username: 'AdityaSetyadi',
    formMode: 1 // 1 => OPEN ; 2 => REJECTED ; 3 => SUBMITTED ; 4 => APPROVED ;  
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

    let uploadHandler = function (setter) {
    // console.log('camera handler', setter);
    // cameraFunction = setter;
    // openCamera();
    }

    let GpsHandler = function (setter, isPhoto) {
    // console.log('camera handler', setter);
    // isPhoto = true,
    // cameraGPSFunction = setter;
    // openCameraGPS(isPhoto);
    }

    let onlineSearch = async (url) =>
    (await fetch(url, setBearer())
        .catch((error) => {
        return {
            success: false,
            data: {},
            message: '500'
        }
        }).then((res) => {
        if (res.status === 200) {
        let temp = res.json();
        return temp;
        } else {
        return {
            success: false,
            data: {},
            message: res.status
        }
        }
        }).then((res) => {
        return res;
        }
    ));

    let setResponseMobile = function (res, rem) {
    // respons = res
    // remarks = rem

    // console.log('respons', respons)
    // console.log('remarks', remarks)
    }

    let setSubmitMobile = function (res, rem) {
    // respons = res
    // remarks = rem

    // console.log('respons submit', respons)
    // console.log('remarks submit', remarks)
    }

    let openMap = function (koordinat) {
    // koordinat = koordinat

    // console.log('coordinat ', koordinat)
    }

    let form = FormGear(template, preset, response, validation, remark, config, uploadHandler, GpsHandler, onlineSearch, setResponseMobile, setSubmitMobile, openMap);

    return form;
}

const data = Promise.all([
    template, preset, response, validation, remark
]);

data.then(([template, preset, response, validation, remark]) => initForm(template, preset, response, validation, remark));

</script>