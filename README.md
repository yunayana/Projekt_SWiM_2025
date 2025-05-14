# Opracowanie modelu pojazdu autonomicznego wraz z realizacją oprogramowania sterującego 

### Uczestnicy zespołu:
- **Yana Trotsenko** – 21232 🐱  
- **Zofia Głowacka** – 21234 🐻   
- **Valeriia Khylchenko** – 21279 🐿️ 

---

## Cel projektu

Zaprojektowanie, zbudowanie oraz zaprogramowanie **modelu pojazdu autonomicznego** z wykorzystaniem mikrokontrolera **STM32**.

---

## Założenia konstrukcyjne pojazdu

| Komponent                           | Opis                                      |
|-------------------------------------|-------------------------------------------|
| STM32F303RET6                       | Płytka główna                             |
| L298N                               | Dwukanałowy sterownik silników            |
| LM7805                              | Stabilizator napięcia                     |
| Silniki 5V                          | Napęd                                     |
| Baterie 3.7V × 3                    | Zasilanie                                 |
| HC-05                               | Moduł Bluetooth                           |
| HC-SR04                             | Ultradźwiękowy czujnik odległości         |

---

 **Serce projektu - STM32F303RET6**:  



![Użyta płytka](img/PLYTKA.png)

---

## Połączenia

### Koła i silniki:
- Motor A+ --> VIN
- Motor A- --> GND
- Motor B+ --> VIN
- Motor B- --> GND

### Sterownik L298N do płytki STM32:
- IN1 --> PA0 (A0)
- IN2 --> PA1 (A1)
- IN3 --> PA4 (A2)
- IN4 --> PB1 (A3)
- ENA --> PB9 (D14)
- ENB --> PA8 (D7)


### Stabilizator napięcia LM7805:
- VCC stabilizatora --> VMS (12V) na sterowniku
- GND stabilizatora --> GND sterownika
- GND sterownika --> GND płytki
- VCC stabilizatora --> VIN płytki
- GND stabilizatora --> GND płytki


### Czujnik odległości HC-SR04:
- Trig --> PA5 (D13)
- Echo --> PA6 (D12)
- VCC --> 5V
- GND --> GND


### Bluetooth HC-05:
- VCC --> VCC z LM7805
- GND --> GND (CN11 na płytce)
- TXD --> PA10 (D2)
- RXD --> PA9 (D8)


## Działanie w IdeCube

## Link do repozytorium 
[Zobacz repozytorium na GitHubie](https://github.com/yunayana/Projekt_SWiM_2025)

