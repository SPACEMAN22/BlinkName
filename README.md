# BlinkName

int led1 = D6;

int led2 = D7;


void setup() {
    
    pinMode(led1,OUTPUT);
    pinModr(led2,OUTPUT);

}

int unit = 100;

void dot()
{
    digitalWrite(led1,HIGH);
    digitalWrite(led2,HIGH);
    delay(unit);
    digitalWrite(led1,LOW);
    digitalWrite(led2,LOW);
    delay(unit);
}

void dash()
{
    digitalWrite(led1,HIGH);
    digitalWrite(led2,HIGH);
    delay(unit*3);
    digitalWrite(led1,LOW);
    digitalWrite(led2,LOW);
    delay(unit);
}

void new_char()
{
    delay(unit*2);
}

void new_word()
{
    delay(unit*6);
}
void loop() {
    
    //s
    dot();
    dot();
    dot();
    new_char();
    
    //h
    dot();
    dot();
    dot();
    dot();
    new_char();
    
    //a
    dot();
    dash();
    new_char();
    
    //n
    dash();
    dot();
    new_char();
    

}
