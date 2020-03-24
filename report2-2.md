```

PFont f;
void setup() {
  size(800,400);
  f = createFont("굴림", 64);
  textFont(f);
}
int i, dir=1, sp=1;
void draw() {
  fill(0);
  background(127,127,127);
  text("안동대 컴공 사랑합니다", 50, i);
  if(i>height) i=0;
  i = i+dir*sp;
  if(keyPressed)
  sp=key-'0';
}

```
