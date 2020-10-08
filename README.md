# photocaption
NuxtJs photo caption gallery component
 ````nuxt.js
 <PhotoCaption :photoCaption="photoCaption" />
 
 import PhotoCaption from "../node_modules/photocaption/photoCaption3/PhotoCaption";
 ````
 
 ````nuxt.js
   data() {
    return {
      photoCaption: {
        color: {
          bgColor1: " ", // color , Hex, rgb, rgba
          bgColor2: " ", // color , Hex, rgb, rgba
          bgColor3: " ", // color , Hex, rgb, rgba
          textColor1: " ", // color , Hex, rgb, rgba
          textColor2: " ", // color , Hex, rgb, rgba
          textColor3: " ", // color , Hex, rgb, rgba
          textColor4: " ", // color , Hex, rgb, rgba
        },
        text: {
          btnText: " ", // button in text
          title1: "Javascript",
          title2: "Vue Js",
          title3: "Nuxt JS",
          title4: "Node Js",
          subTitle1: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
          subTitle2: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
          subTitle3: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
          subTitle4: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
        path: {
          path1: "javascript", 
          path2: "vuejs",
          path3: "nuxtjs",
          path4: "nodejs",
        },
      },
    };
  },
  ````
 ### images
 static folder in create new folder name: 'image' > image in new folder name: 'photoCaption' > photoCaption in your image.
