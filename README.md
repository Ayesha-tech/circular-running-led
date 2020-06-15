# circular-running-led




#include<avr/io.h>
#include<util/delay.h>
void POV_toy(uint8_t onebyte){
  PORTD =onebyte;
  _delay_ms(10);
}
  
int main(void){
  DDRD = 0xFF;
  
  while(1){
  POV_toy(0b00000001);
  _delay_ms(100);
  POV_toy(0b00000010);
  _delay_ms(100);
  POV_toy(0b00000100);
  _delay_ms(100);
  POV_toy(0b00001000);
  _delay_ms(100);
  POV_toy(0b00010000);
  _delay_ms(100);
  POV_toy(0b00100000);
  _delay_ms(100);
  POV_toy(0b01000000);
  _delay_ms(100);
  POV_toy(0b10000000);
  _delay_ms(100);
  POV_toy(0b01000000);
  _delay_ms(100);
  POV_toy(0b00100000);
  _delay_ms(100);
  POV_toy(0b00010000);
  _delay_ms(100);
  POV_toy(0b00001000);
  _delay_ms(100);
  POV_toy(0b00000100);
  _delay_ms(100);
  POV_toy(0b00000010);
  _delay_ms(100);
  POV_toy(0b00000001);
  _delay_ms(100);
  POV_toy(0b11111111);
  _delay_ms(100);

     
  }
}
