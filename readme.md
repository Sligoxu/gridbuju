# GRID布局

### 描述：对网页图片部分进行布局排版

html部分

![grid.html](gridhtml.png)

css部分

```css
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }
  .image{
    max-width: 100%;
  } 
  .container{
    border: 1px solid blue;
    display: grid;
    width: 500px;
    grid-template-columns: 250px 250px;
    grid-template-rows: 240px 120px 120px 120px 120px;
    grid-template-areas: 
      "big mid1"
      "big mid2"
      "sm1 mid2"
      "sm2 mid3"
      "sm3 mid3";
      margin-left: auto;
      margin-right: auto;
  }
  .image:first-child{
    grid-area: big;
    border: 1px solid red;
  }
  .image:nth-child(2){
    grid-area: sm1;
    border: 1px solid red;
  }
  .image:nth-child(3){
    grid-area: sm2;
    border: 1px solid red;
  }
  .image:nth-child(4){
    grid-area: sm3;
    border: 1px solid red;
  }
  .image:nth-child(5){
    grid-area: mid1;
    border: 1px solid red;
  }
  .image:nth-child(6){
    grid-area: mid2;
    border: 1px solid red;
  }
  .image:nth-child(7){
    grid-area: mid3;
    border: 1px solid red;
  }
  ```

  ### 网页运行效果

  [我的网页地址](https://jsbin.com/kalecodesa/edit?html,css,output)