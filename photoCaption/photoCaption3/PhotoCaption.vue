<template>
  <div>
    <div class="contain">
      <div
        class="col"
        :style="{ backgroundColor: this.photoCaption.color.bgColor1, color: this.photoCaption.color.textColor1 }"
      >
        <h2>{{ this.photoCaption.text.title1 }}</h2>
        <div class="caption">
          <p>{{ this.photoCaption.text.subTitle1 }}</p>
          <router-link tag="button" :to="'/' + this.photoCaption.path.path1">{{
            this.photoCaption.text.btnText
          }}</router-link>
        </div>
        <img
          :src="'_nuxt/static/image/' + photoCaption.image.img1 + '.png'"
          :alt="this.photoCaption.text.title1"
        />
      </div>
      <div
        class="col"
        :style="{ backgroundColor: this.photoCaption.color.bgColor2, color: this.photoCaption.color.textColor2 }"
      >
        <h2>{{ this.photoCaption.text.title2 }}</h2>
        <div class="caption">
          <p>{{ this.photoCaption.text.subTitle2 }}</p>
          <router-link tag="button" :to="'/' + this.photoCaption.path.path2">{{
            this.photoCaption.text.btnText
          }}</router-link>
        </div>
        <img
          :src="'_nuxt/static/image/' + photoCaption.image.img2 + '.png'"
          :alt="this.photoCaption.text.title2"
        />
      </div>
      <div
        class="col"
        :style="{ backgroundColor: this.photoCaption.color.bgColor3, color: this.photoCaption.color.textColor3 }"
      >
        <h2>{{ this.photoCaption.text.title3 }}</h2>
        <div class="caption">
          <p>{{ this.photoCaption.text.subTitle3 }}</p>
          <router-link tag="button" :to="'/' + this.photoCaption.path.path3">{{
            this.photoCaption.text.btnText
          }}</router-link>
        </div>
        <img
          :src="'_nuxt/static/image/' + photoCaption.image.img3 + '.png'"
          :alt="this.photoCaption.text.title3"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    photoCaption: {
      required: false,
    },
  },
};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  font-family: "Popins", sans-serif;
}

.contain {
  width: 1000px;
  height: 400px;
  background-color: #ccc;
  margin: 120px auto;
  display: flex;
}

.col {
  height: 100%;
  flex: 1;
  color: #fff;
  box-sizing: border-box;
  padding: 25px;
  position: relative;
  transition: 0.6s;
}

.col:nth-child(1) {
  background: #283491;
}
.col:nth-child(2) {
  background: #f18684;
}
.col:nth-child(3) {
  background: #6ee2f1;
}

h2 {
  text-align: center;
  font-size: 22px;
  font-weight: 600;
}

.caption {
  max-width: 230px;
  font-size: 12px;
  margin: 28px 0;
  display: none;
}

.caption button {
  border: 1px solid rgb(240, 240, 240);
  background: transparent;
  outline: none;
  padding: 8px 18px;
  color: rgb(240, 240, 240);
  border-radius: 30px;
  margin-top: 20px;
  cursor: pointer;
  font-size: 12px;
}

.col img {
  width: 200px;
  position: absolute;
  right: 0;
  bottom: 0;
}
.caption button:hover {
  background-color: transparent;
  border: none;
  -webkit-box-shadow: -10px 14px 43px -13px rgba(0, 0, 0, 0.75);
  -moz-box-shadow: -10px 14px 43px -13px rgba(0, 0, 0, 0.75);
  box-shadow: -10px 14px 43px -13px rgba(0, 0, 0, 0.75);
}
@media only screen and (min-width: 1180px) {
  .col:hover {
    flex-grow: 2.5;
  }

  .col:hover .caption {
    display: block;
  }

  .col:hover h2 {
    text-align: left;
  }
}

@media only screen and (min-width: 701px) and (max-width: 1180px) {
  .contain {
    width: 100%;
    margin: 55px auto;
  }
  .col:hover {
    flex-grow: 2.5;
  }

  .col:hover .caption {
    display: block;
  }

  .col:hover h2 {
    text-align: left;
  }
}

@media only screen and (min-width: 451px) and (max-width: 700px) {
  .contain {
    width: 100%;
    margin: 55px auto;
    display: block;
    margin-bottom: 800px;
  }
  .caption {
    display: block;
  }
}

@media only screen and (min-width: 321px) and (max-width: 450px) {
  .contain {
    width: 100%;
    margin: 55px auto;
    display: block;
    margin-bottom: 800px;
  }
  .caption {
    display: block;
  }
}
@media only screen and (max-width: 320px) {
  .contain {
    width: 100%;
    margin: 75px auto;
    display: block;
    margin-bottom: 800px;
  }
  .caption {
    display: block;
  }
}
</style>