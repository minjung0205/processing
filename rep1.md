# 1주차 펜 만들기 
## 안동대학교 김민정

```

void setup(){         //한번만 실행하는것
  size(500,500);      //결과 화면의 크기
  stroke(125,125,0);    //색깔 노란색
  strokeWeight(12);   //굵기
} 
void draw(){           //반복 실행 
  if(mousePressed)      //마우스를 누를때마다
      line(pmouseX,pmouseY,mouseX,mouseY);   //선이 생기는것
}

```
