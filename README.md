
const int movePins[] = {2, 3, 4, 5};

void moveDir(){
  
}


void setup() {
 for(int i = 0; i <= 4; i++){
  pinMode(i, INPUT);
 }
}


void loop() {
  int buttonState[4];
  for(int i = 0; i <= 4; i++){
    buttonState[i] = digitalRead(movePins[i + 2]);
   if(i == 1){
    while( buttonState[i] == HIGH){
      moveDir();
    }
   }else if(i == 1){
    buttonState[i] = digitalRead(movePins[i]);
   }else if(i == 2){
    buttonState[i] = digitalRead(movePins[i]);
   }else if(i == 3){
    buttonState[i] = digitalRead(movePins[i]);
   }
  }
}
