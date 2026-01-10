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
      
<img width="1132" height="776" alt="image" src="https://github.com/user-attachments/assets/f80bf173-b802-4dc1-8082-6b1175491458" />
       
# Prep For Manufacturing
         
Once I was sure I had finished the board I downloaded the necessary design files from KICAD (.gbr , BOM , CPL) I edited the BOM and CPL formats to fit JLCPCB and uploaded my design.
      
Once the files were uploaded, I chose the correct settings for my design and whent on to choosing what parts JLCPCB would buy and install for me.
          
ALL basic components I selected and most Extended components as they are far to complicated to solder myself but the I/O pins and LED I will add myself to save A LOT of money. (Almost 30 dollars)
      
I actually made an error originaly where my board was set up as "Standard PCBA" not "Economic PCBA" which is why I had to place the LED myself and why I saved $30.
        
<img width="1102" height="918" alt="image" src="https://github.com/user-attachments/assets/4f17f053-783e-4e9c-af44-7637e2c86bf8" />
         
<img width="1102" height="918" alt="image" src="https://github.com/user-attachments/assets/7abd0e89-c0d0-456e-8161-49921f451149" />
          
<img width="1102" height="918" alt="image" src="https://github.com/user-attachments/assets/8a069cdb-3813-49e0-b87a-7e5ee004d5ae" />
           
<img width="1403" height="918" alt="image" src="https://github.com/user-attachments/assets/baaa2aea-f51f-4384-aa1b-808658904a4b" />
          
# V1 vs V2
          
Honestly they are not too different but V2 was a complete restart for the pcb routing and component placement as V1 was full of errors that were easier to re-do than fix.
