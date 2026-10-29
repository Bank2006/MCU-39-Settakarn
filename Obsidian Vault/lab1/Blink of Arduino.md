ກະກຽມອຸປະກອນ:
- LED
- jumper wire
- breadboard
- Arduino UNO
- Resistor(220ໂອມ)(red, red, black, black, brown)
ການທົດລອງ:
ການຕໍ່ວົງຈອນ: ຕໍ່ຫຼອດໄຟ LED ແລະ ຕົວຕ້ານທານເຂົ້າ breadboard ເຊິ່ງຕົວຕ້ານທານຈະສຽບເຂົ້າຢູ່ຂາບວກຂອງຫຼອດໄຟ ຈາກນັ້ນສຽບສາຍເຂົ້າຂາລົບຂອງດອກໄຟແລ້ວສຽບເຂົ້າ breadboard ແລ້ວສຽບເຂົ້າໄປໃນຂາ ground(GND in Arduino) ໃນສ່ວນຂອງຕົວຕ້ານທານເເມ່ນສຽບສາຍໄຟເຂົ້າໄປໃນຂາ PIN 13 ຢູ່ບອດ Arduino 

ການຂຽນໂປຣແກຣມ(coding):
void setup() {
 pinMode(LED_BUILTIN, OUTPUT); // (ເປັນການບອກຄ່າຂອງໄຟ LED)
}

void loop() {
 digitalWrite(LED_BUILTIN, HIGH); //  (ເປັນສະຖານະເປີດດອກໄຟ)
 delay(1000); // (ໄລຍະເວລາ 1000​ milisecond = 1s )
 digitalWrite(LED_BUILTIN, LOW); //  (ເປັນສະຖານະປີດດອກໄຟ)
 delay(1000); 
}

ຜົນການທົດລອງເຫັນວ່າເມື່ອອັບໂຫລດໂຄດແລ້ວ ຫຼອດໄຟຈະມີການຮຸ່ງເປັນເວລາ 1 ວິ ແລະ ດັບ ເປັນເວລາ 1 ວິ ສະແດງໃຫ້ເຫັນເຖິງການກະພິບຂອງດອກໄຟ