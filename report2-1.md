# report 2-1

```

void setup() {
  size(800, 300);
  textSize(128);
}
int i,a=1;
void draw() {
  background(127,127,127);
  text("Graphics", i=i+a, 200);
  fill(0);
  if(i>800) i=0;
}
void keyPressed(){
  a = key-'0'; 
}

```
