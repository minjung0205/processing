# 2주차 위에서 밑으로 반복해서 내려오는 배너
## 
```

PFont f;     //한글 나타내기
void setup() {     //한번실행하는것
  size(800,400);    //결과 화면 가로 세로 사이즈
  f = createFont("굴림", 64);   //글씨체,크기
  textFont(f);
}
int i, dir=1, sp=1; 
void draw() {  //반복실행 실행하는것
  fill(127,127,0);    //글씨 색깔 노란색
  background(0);    //바탕 색깔 검정색
  text("안녕하세요", i,200);  //텍스트 출력
  if(i>width) dir=-1; // i>800이 되면 오른쪽에서 왼쪽으로 가도록
  if(i<0) dir=1;  //i<0이 되면 왼쪽에서 오른쪽으로 가도록
  i= i+dir;
  i = i+dir*sp; //누르는 숫자에 따라 움직이는 속도가 달라진다
  if(keyPressed)
  sp = key- '0';
}

```
