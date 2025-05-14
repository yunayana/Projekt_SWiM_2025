# 🚗 Opracowanie modelu pojazdu autonomicznego wraz z realizacją oprogramowania sterującego 

### 🎓 Uczestnicy zespołu:
- **Yana Trotsenko** – 21232 🐱  
- **Zofia Głowacka** – 21234 🐻   
- **Valeriia Khylchenko** – 21279 🐿️ 

---

## 🎯 Cel projektu

Zaprojektowanie, zbudowanie oraz zaprogramowanie **modelu pojazdu autonomicznego** z wykorzystaniem mikrokontrolera **STM32**.

---

## 🔧 Założenia konstrukcyjne pojazdu

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

## 🔌 Schemat elektryczny

📷 **Serce projektu - STM32F303RET6**:  
<p align="center">
  <img src="https://github.com/yunayana/Projekt_SWiM_2025/blob/main/img/Plytka.png?raw=true" alt="Użyta płytka" width="400"/>
</p>


> W repozytorium umieść plik w folderze `docs/` jako np. `schemat.jpg` i użyj:  
> `![Schemat elektryczny](docs/schemat.jpg)`

---

## ⚙️ Połączenia

### 🔁 Koła i silniki:
