# Miguel-s-Custom-Devboard-RP2040
I started this project as a way to practice and learn some more about pcb design. This board is not perfect as it is my second pcb and my first devboard.
    
# Schematic Design
    
I followed the [Custom Devboard Guided Project](https://blueprint.hackclub.com/starter-projects/devboard) by [Kai Pereira](https://github.com/KaiPereira/build-a-devboard) so it was not my design but I did rout the PCB myself an added and LED.
     
The designs and components are directly from the guide but the LED I added once I realized how empty the board was at the pcb design section.
    
Components:
- RP 2040
- LED (SK6812-mini-e)
- USB-C-2.0
- Voltage regulator (MCP1700T-3302E/TT)
- Crystal Ocilater (12mhz)
- I/O (1x20)x2 (1x3)x1
- Flash Memory/Storage (W25Q16JVZPIQ) (16-Mbi)
     
<img width="1132" height="776" alt="image" src="https://github.com/user-attachments/assets/09a4f896-e33b-43ad-a975-9ce0514d7be8" />
     
# PCB Design
     
The board dimensions and I/O location are exact from the guide but the rest I ended up moving around to fit my routing. The LED I placed in the very empty bottom of the board above the 1x3 pins.
         
I routed the USB first then the Flash, followed by the crystal ocilator. Once the important connections were made I connected the I/O and LED, lastly I set up the ground pour and fixed any errors the ERC flaged.
         
<img width="1132" height="776" alt="image" src="https://github.com/user-attachments/assets/014409e6-99bc-4957-a592-48f74449c50f" />
