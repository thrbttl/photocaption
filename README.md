# photocaption
NuxtJs photo caption gallery component
 ````nuxt.js
 <PhotoCaption :photoCaption="photoCaption" />
 ````
 ````nuxt.js
   data() {
    return {
      photoCaption: {
        color: {
          bgColor1: "red", // color , Hex, rgb, rgba
          bgColor2: "#bebe22", // color , Hex, rgb, rgba
          bgColor3: "rgba(255, 134, 5, 0.29)", // color , Hex, rgb, rgba
          textColor1: "yellow", // color , Hex, rgb, rgba
          textColor2: "#ccc", // color , Hex, rgb, rgba
          textColor3: "rgba(255, 34, 5, 0.29)", // color , Hex, rgb, rgba
        },
        text: {
          btnText: "Devamı...", // button in text
          title1: "Javasctip",
          title2: "Vue Js",
          title3: "Nuxt Js",
          subTitle1: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
          subTitle2: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
          subTitle3: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
        path: {
          path1: "js", 
          path2: "vue",
          path3: "nuxt",
        },
      },
    };
  },
  ````
