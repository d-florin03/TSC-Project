

#  OpenBook – Dispozitiv e-book reader open-source

##  Descriere general

**OpenBook** este un e-book reader ieftin și complet open-source, dezvoltat în cadrul unui start-up care își propune să ofere o alternativă accesibilă și personalizabilă pentru cititul digital. Acest proiect este realizat în echipă, iar scopul este dezvoltarea completă a hardware-ului, de la specificații inițiale până la prototip pregătit pentru producție în masă.
## Diagrama bloc
   
![diagr](https://github.com/user-attachments/assets/c25fb030-52d3-49d0-8d1c-37574f988e0c)

## 📦 Componente hardware utilizate

    -> Senzor BME688 (senzor multifunctional)
    -> Buton tactil
    -> ESP32-C6-WROOM-1 (modulul principal care contine microcontrolerul ESP32-C6 si o memorie flash SPI de 8 MB)
    -> LED indicator (ADAFRUIT_CHIP-LED0603)
    -> Port USB (USB4110GFA)
    -> Conector JST de 1 mm (JST04_1MM_RA)

## ⚡ Calcul estimativ consum de energie

| Componentă             | Curent estimat | Observații                                   |
|------------------------|----------------|----------------------------------------------|
| ESP32-C6               | ~80-120 mA     | În regim activ cu WiFi                       |
| WS2812B                | ~300 mA        | La luminozitate maximă, toate LED-urile aprinse |
| Senzori proximitate    | ~10-20 mA/senzor| În funcție de tehnologia senzorului          |
| LED-uri statice        | ~10 mA/LED     | În funcție de câte sunt aprinse simultan     |

🔋 **Total estimat**: ~500–600 mA în regim activ continuu. Suficient pentru alimentare USB standard (5V, 1A).



## 📂 Fișiere utile

- `Schematic.png` – Schema electrică completă
- `PCB.png` – Randare PCB + layout
- `README.md` – Acest fișier

---

🛠️ Proiect realizat ca parte a inițiativei **OpenBook**, pentru dezvoltarea unui e-book reader ieftin și open source.
