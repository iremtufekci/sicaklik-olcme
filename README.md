# sicaklik-olcme
int lm35=A0;
 int okunandeger=0;
 float sicaklikgerilim=0;
 float sicaklik=0;
void setup() {

Serial.begin(9600);
}

void loop() {
okunandeger=analogRead(lm35);
sicaklikgerilim=(5000.0/1023)*okunandeger;
sicaklik=sicaklikgerilim/10.0;
Serial.println(sicaklik);
delay(1000);


}
