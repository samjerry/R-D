# R-D
int timer = 75; // Higher number = longer scan... adjust the meeting in middle to look in time if you change this number
int indLED = 75; //This is the delay on the meet in the middle sequence, updated to use an integer function


void setup() {
  // use a for loop to initialize each pin as an output, this also takes care of digital output set-up:
  for (int thisPin = 0; thisPin < 7; thisPin++)  {
    pinMode(thisPin, OUTPUT);      
  }
}

void loop() {
  // loop from right to left:
  for (int thisPin = 0; thisPin < 7; thisPin++) { 
    // turn the pin on:
    digitalWrite(thisPin, HIGH);   
    delay(timer);                  
    // turn the pin off:
    digitalWrite(thisPin, LOW);    
  }

  // loop from left to right:
  for (int thisPin = 7; thisPin >= 0; thisPin--) { 
    // turn the pin on:
    digitalWrite(thisPin, HIGH);
    delay(timer);
    // turn the pin off:
    digitalWrite(thisPin, LOW);
  } 
  
  // This is where it will start on each side, meet in middle, and go back
digitalWrite(7, HIGH);   // set the LED on
  digitalWrite(0, HIGH);
  delay(indLED);              
  digitalWrite(7, LOW);
  digitalWrite(0,LOW);  // set the LED off
  delay(0);              
  digitalWrite(6, HIGH);   // set the LED on
  digitalWrite(1, HIGH);
  delay(indLED);              
  digitalWrite(6, LOW);
  digitalWrite(1,LOW);  // set the LED off
  delay(0);              
  digitalWrite(5, HIGH);   // set the LED on
  digitalWrite(2, HIGH);
  delay(indLED);              
  digitalWrite(5, LOW);
  digitalWrite(2,LOW);  // set the LED off
  delay(0);              
  digitalWrite(4, HIGH);   // set the LED on
  digitalWrite(3, HIGH);
  delay(indLED);             
  digitalWrite(4, LOW);
  digitalWrite(3,LOW);  // set the LED off
  delay(0);                        
  digitalWrite(4, HIGH);   // set the LED on
  digitalWrite(3, HIGH);
  delay(indLED);              
  digitalWrite(4, LOW);
  digitalWrite(3,LOW);  // set the LED off
  delay(0);             
  digitalWrite(5, HIGH);   // set the LED on
  digitalWrite(2, HIGH);
  delay(indLED);              
  digitalWrite(5, LOW);
  digitalWrite(2,LOW);  // set the LED off
  delay(0);             
  digitalWrite(6, HIGH);   // set the LED on
  digitalWrite(1, HIGH);
  delay(indLED);             
  digitalWrite(6, LOW);
  digitalWrite(1,LOW);  // set the LED off
  delay(0);             
  digitalWrite(7, HIGH);   // set the LED on
  digitalWrite(0, HIGH);
  delay(indLED);             
  digitalWrite(7, LOW);
  digitalWrite(0,LOW);  // set the LED off
  delay(0);              

// loop left to right
 for (int thisPin = 7; thisPin >= 0; thisPin--) { 
    // turn the pin on:
    digitalWrite(thisPin, HIGH);
    delay(timer);
    // turn the pin off:
    digitalWrite(thisPin, LOW);
  } 
 // loop right to left:
  for (int thisPin = 0; thisPin < 7; thisPin++) { 
    // turn the pin on:
    digitalWrite(thisPin, HIGH);   
    delay(timer);                  
    // turn the pin off:
    digitalWrite(thisPin, LOW);    
  }
 
  // meet in middle again and then go back
 digitalWrite(7, HIGH);   // set the LED on
  digitalWrite(0, HIGH);
  delay(indLED);              
  digitalWrite(7, LOW);
  digitalWrite(0,LOW);  // set the LED off
  delay(0);            
  digitalWrite(6, HIGH);   // set the LED on
  digitalWrite(1, HIGH);
  delay(indLED);             
  digitalWrite(6, LOW);
  digitalWrite(1,LOW);  // set the LED off
  delay(0);              
  digitalWrite(5, HIGH);   // set the LED on
  digitalWrite(2, HIGH);
  delay(indLED);             
  digitalWrite(5, LOW);
  digitalWrite(2,LOW);  // set the LED off
  delay(0);              
  digitalWrite(4, HIGH);   // set the LED on
  digitalWrite(3, HIGH);
  delay(indLED);              // wait for a second
  digitalWrite(4, LOW);
  digitalWrite(3,LOW);  // set the LED off
  delay(0);              
    
  digitalWrite(4, HIGH);   // set the LED on
  digitalWrite(3, HIGH);
  delay(indLED);              
  digitalWrite(4, LOW);
  digitalWrite(3,LOW);  // set the LED off
  delay(0);                        
  digitalWrite(5, HIGH);   // set the LED on
  digitalWrite(2, HIGH);
  delay(indLED);             
  digitalWrite(5, LOW);
  digitalWrite(2,LOW);  // set the LED off
  delay(0);              
  digitalWrite(6, HIGH);   // set the LED on
  digitalWrite(1, HIGH);
  delay(indLED);              // wait for a second
  digitalWrite(6, LOW);
  digitalWrite(1,LOW);  // set the LED off
  delay(0);             
  digitalWrite(7, HIGH);   // set the LED on
  digitalWrite(0, HIGH);
  delay(indLED);              
  digitalWrite(7, LOW);
  digitalWrite(0,LOW);  // set the LED off
  delay(0);              
 } 
