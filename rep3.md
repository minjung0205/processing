# 3주차 examples (Patterns)
## 안동대학교 김민정


```

void setup() { //한번만 실행하는것
  size(640, 360); // 결과창 가로 세로 사이즈
  background(102);  //배경색깔
}

void draw() {
  variableEllipse(mouseX, mouseY, pmouseX, pmouseY);
} //함수생성


void variableEllipse(int x, int y, int px, int py) {  //함수 호출
  float speed = abs(x-px) + abs(y-py); // abs는 절댓값
  stroke(speed); //속도
  fill(127,127,0); //노란색
  ellipse(x, y, speed, speed);
}

```
