# cosweal-intern-project
cosweal project
![Untitled (1)](https://user-images.githubusercontent.com/44186682/65585539-97cb3200-dfbd-11e9-8efe-64e7de842b7d.png)



vuetify 설치

cmd 콘솔창에

$ vue add vuetify

[](https://www.notion.so/e594ebf1ac364926a92c3a76f92e015a#10719c7e727448cbb322f9990a275a4f)

설치하는 도중에 나오는 화면입니다 화면과 같이 입력해주시면 됩니다

3가지 선택하는 부분이나오면 advanced를 선택하면 다음화면이 나오게 됩니다

그대로 따라해주시면 됩니다

[](https://www.notion.so/e594ebf1ac364926a92c3a76f92e015a#19b2c0c88a4544a496f920097cc09d58)

plugins 디렉터리에 vuetify.js 추가됨

$ npm run serve 

로컬에 서버르 띄운다

[](https://www.notion.so/e594ebf1ac364926a92c3a76f92e015a#502f7bec43ee4985aead379881ea8db7)

빌드후에 dist 디렉터리가 추가된다.

App.vue와서 template script만 남기고 지운다 다음코드 작성

[](https://www.notion.so/e594ebf1ac364926a92c3a76f92e015a#b7b427e13a6243d4967f51d50bca5edb)

그리고 뷰티파이에 접속해보자.

[https://vuetifyjs.com/en/getting-started/pre-made-layouts](https://vuetifyjs.com/en/getting-started/pre-made-layouts) 

에 접속후 centered 소스를 템플릿안에 넣어줍니다.

[](https://www.notion.so/e594ebf1ac364926a92c3a76f92e015a#b06e19f41f5843f9ab92660cddaecf02)

다음화면에서 playground에서 버튼을 원하는 모양으로 만들어줍니다.

버튼색은 color="primary" 로 지정해줍니다.

그이후 폰트를 조절하기위해 폰트를 다운받아줍니다.

$ npm install @mdi/font -D

패키지가 설치되면 간단히 **`vuetify.js`**플러그인 폴더 의 파일 로 가져 오십시오 .

    // src/plugins/vuetify.js
    
    import '@mdi/font/css/materialdesignicons.css' // Ensure you are using css-loader
    import Vue from 'vue'
    import Vuetify from 'vuetify/lib'
    
    Vue.use(Vuetify)
    
    export default new Vuetify({
      icons: {
        iconfont: 'mdi', // default - only for display purposes
      },
    })

다양한 지원 iconfonts 및 고급 구현에 대한 자세한 내용을 보려면 [Icons로](https://vuetifyjs.com/customization/icons) 이동하십시오. 페이지.

### cosweal 코스윌이란 로고에 대한 내용입니다

<div class="display-4">

<div class="font-weight-black" >

C O S W E A L

</div>

</div>

위와 같이 폰트 크기와 스타일을 지정해줍니다.

Enter your e-mail and password to Log in

사이즈는 h2로 지정해주고 폰트 스타일은 같은거로 지정해줍니다.

<div class="font-weight-black">

<h2> Enter your e-mail and password to Log in

</h2>

</div>

배경넣기

맘에 드는 이미지를 src/assets 폴더에 이미지를 넣어줍니다.

template 밑에 v-app모든 화면을 감싸고 있기에 id 값을 넣어주고 

<v-app id="inspire"> 맨밑 <style>안에

#inspire{

background-image: url('./assets/bg1.png.png')

}

넣어줍니다.

about cosweal과 아이콘

우선 아이콘을 띄워주기 위해 cmd창에

npm install material-design-icons-iconfont -D

[](https://www.notion.so/e594ebf1ac364926a92c3a76f92e015a#1cf71d81147e4c8e89c279470cee4874)

그이후 main.js파일로가서 추가해줍니다.

[](https://www.notion.so/e594ebf1ac364926a92c3a76f92e015a#b7e9dbb474774086b671d9e84abcca92)

import Vue from 'vue'

import App from './App.vue'

import router from './router'

import store from './store'

import vuetify from './plugins/vuetify';

import '@babel/polyfill'

import 'material-design-icons-iconfont/dist/material-design-icons.css' // Ensure you are using css-loader

import Vuetify from 'vuetify/lib'

Vue.config.productionTip = false

new Vue({

router,

store,

vuetify,

render: h => h(App)

}).$mount('#app')

Vue.use(Vuetify)

export default new Vuetify({

icons: {

iconfont: 'md',

},

})

와 같이 기본 구성을 해줍니다. 그이후 vuetify에서 제공되는 아이콘의 이름을 쓰면  모두 이용할수있습니다.

checkbox

input을 넣어주고 checkbox를 만들어줍니다.

<input class = "rember" color =black type="checkbox" checked v-model="selected" ><span class="rember" > remember id/password </span>

?아이콘과 forget id/password에 링크 걸어주기

<a href를 이용하여 링크를 걸어줍니다.

<a class="link" href="[http://www.cosweal.com/main/main.php](http://www.cosweal.com/main/main.php)">

이용하하다보면 밑줄이 생기게 됩니다 밑줄을 지우기위해 클래스 값을 지정해주고

<style> .클래스안에 text-decoration:none; 를 넣어주면 밑줄이 지워지게 됩니다.

  

[](https://www.notion.so/e594ebf1ac364926a92c3a76f92e015a#69cdececc393449b9e54eb520c831bb7)
