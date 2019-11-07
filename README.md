

// This #include statement was automatically added by the Particle IDE.
#include <InternetButton.h>



#include <InternetButton.h>

InternetButton button = InternetButton();


int counter = 0;
int seconds = 20; 

void setup() {

button.begin();
}
void loop() {
    
    
button.ledOn(4, 0, 0, 255);
 button.ledOn(5, 0, 0, 255);
 button.ledOn(6, 0, 0, 255);
 button.ledOn(7, 0, 0, 255);
 button.ledOn(8, 0, 0, 255);
 counter = counter + 1;

 for (int i = 0; i < 11; i++) {
     
     
     
if((counter % 60 == 0) &&(seconds >= 0)){
    seconds = seconds - 1;
           
           // button.allLedsOn(50,50,50);
            
            button.ledOff(4);
            button.ledOff(8);
          
            
            button.ledOff(5);
            button.ledOff(7);
            delay(1000);
            
            button.ledOff(6);
            delay(1000);
            
          
              //Particle.publish("abc", "HELLO WORLD!", 60, PUBLIC);
    
    
             
   }  
    //   button.allLedsOn(255,0,0);
    //   delay(400);
    //   button.allLedsOff();
            
    
    // allLedsOn(255,0,0);
    //   delay(200);
    //   button.allLedsOff();
    // counter = counter + 1;
    // if((counter % 60 == 0) &&(seconds >= 0)){
    //     seconds = seconds - 1;
    //     for(int i = 0; i >= 6 ; i ++){
    //                  button.ledOn(i,255,255,255); 
    //                  delay(200);
    //                  }
    // }
  

}

