# 2025-03-20 vue 수업 내용 정리

## 01_html

1. 보간법

보간법: 두 값 사이의 중간값을 계산하는 방식.
데이터 바인딩.
문자열의 데이터 삽입, 동적으로 값을 추가하는 맥락에서 보간.

<img src="./image.png" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

<pre>
<code>

    <script type="text/javascript">
      const { createApp } = Vue;

      let vm = createApp({
        name: 'App',
        data() {
          return {
            message: '메시지 적용 부분',
            text1: '사용자',
          };
        },
      });
      vm.mount('#app');
    </script>

  </body>
</html>
</code>
</pre>

message에서 렌더링이 진행되기 전까지 적용이 안되는 것을 확인할 수 있음.

## 02.html

<img src="./image-1.png" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

<pre><code>
  <body>

    <script type="text/javascript">
      const { createApp } = Vue;

      let vm = createApp({
        name: 'App',
        data() {
          return {
            message: '',
            article: '<h2> <b>중제목</b>입니다.</h2>',
            svgIcon:
              '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 18c-4.41 0-8-3.59-8-8s3.59-8 8-8 8 3.59 8 8-3.59 8-8 8zm-2-12h4v8h-4z"/></svg>',
          };
        },
      });
      vm.mount('#app');
    </script>

  </body>
</code></pre>

html directive는 관리자 용도로만 사용하는 것이 적합함.

## 03.html

- https://picsum.photos/ 랜덤 사진 사이트.

![alt text](image-5.png)
![alt text](image-6.png)
![alt text](image-4.png)

## 04.html
