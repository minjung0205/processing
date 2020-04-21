# 5주차 PGraphics
## 안동대학교 김민정 

```
PGraphics pg;
void setup(){  //한번만 하는것
  size(400,400); //가로 세로 크기
  pg = createGraphics(200,200);  //가운데에 그려진다
}
void draw(){
  pg.beginDraw(); //그림 그릴때 필요
  pg.background(102); //배경 회색
  pg.stroke(125,125,0); //선 색상 노란색
  pg.strokeWeight(8); //선 굵기
  pg.line(100, pg.height*0.5,
    mouseX-100, mouseY-100); //마우스 위치에 따라서 그려진다
  pg.endDraw(); //그림 그릴때 마지막에 필요!
  image(pg, 100,100);
}

```
