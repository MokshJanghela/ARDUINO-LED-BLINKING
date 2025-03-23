# ARDUINO-LED-BLINKING
Chasing effect left to right then right to left
int leds[] = {6, 7, 8, 9};

void setup() {
  for (int i = 0; i < 4; i++) {
    pinMode(leds[i], OUTPUT);
  }
}
 void loop(){
  for (int i = 0; i < 4; i++) {
    digitalWrite(leds[i], HIGH);
    delay(300);                                                  
    digitalWrite(leds[i], LOW);//left to right//
    }
    for (int i = 2; i >=0; i--) {
      digitalWrite(leds[i], HIGH);
      delay(300);                                                  
      digitalWrite(leds[i], LOW);//right to left//
      }
    }
