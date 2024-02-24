#define trigPin 9           // Trig Pin Of HC-SR04
#define echoPin 10      // Echo Pin Of HC-SR04
#define MLa 5                   //left motor 1st pin
#define MLb 7                  //left motor 2nd pin
#define MRa 8               //right motor 1st pin
#define MRb 6               //right motor 2nd pin
#define touchpin 3
long TravelTime, distance;

void setup() {
  Serial.begin(9600);
  pinMode(MLa, OUTPUT);     // Set Motor Pins As O/P
  pinMode(MLb, OUTPUT);
  pinMode(MRa, OUTPUT);
  pinMode(MRb, OUTPUT);
  pinMode(trigPin, OUTPUT);       // Set Trig Pin As O/P To Transmit Waves
  pinMode(echoPin, INPUT);        //Set Echo Pin As I/P To Receive Reflected Waves
  pinMode(touchpin, INPUT);
}
void loop()
{
  Serial.begin(9600);

 digitalWrite(trigPin , LOW);
  delayMicroseconds (2);
  digitalWrite(trigPin , HIGH);
  delayMicroseconds(10);
  digitalWrite(trigPin , LOW);

  TravelTime = pulseIn (echoPin , HIGH);
  //Speed = distacne/TravelTime;        //السرعة  = المسافة مقسومة على الزمن
  distance = 0.034 * TravelTime / 2;     // المسافة = السرعة مضروبة في * الزمن
 
  if (distance >= 15)               // Condition For Absence Of Obstacle
  {
    digitalWrite(MRb, HIGH);       // Move Forward
    digitalWrite(MRa, LOW);
    digitalWrite(MLb, HIGH);
    digitalWrite(MLa, LOW);
  }
  else if (distance < 15)          // Condition For Presence Of Obstacle
  {
    digitalWrite(MRb, LOW);     //Stop
    digitalWrite(MRa, LOW);
    digitalWrite(MLb, LOW);
    digitalWrite(MLa, LOW);
  }

}
