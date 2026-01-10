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
       
# BOM
    
- PCB ~ $40 [JLCPCB](https://jlcpcb.com/) (For 5)
- I/O Pins ~ $4 + Shipping [AliExpress](https://www.aliexpress.us/item/3256807199266132.html?spm=a2g0o.productlist.main.4.b2eerDecrDecFT&aem_p4p_detail=20260109185732753301892571030012625217&algo_pvid=d6666beb-37c8-4955-94b1-210e04b2dabe&algo_exp_id=d6666beb-37c8-4955-94b1-210e04b2dabe-3&pdp_ext_f=%7B%22order%22%3A%22168%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21USD%213.20%213.04%21%21%2122.21%2121.10%21%402101e07217680138522445737eae12%2112000040529096976%21sea%21US%210%21ABX%211%210%21n_tag%3A-29910%3Bd%3Ac04e790%3Bm03_new_user%3A-29895&curPageLogUid=dwaYiwHq2kqp&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005007385580884%7C_p_origin_prod%3A&search_p4p_id=20260109185732753301892571030012625217_1) (For 10 1x40 Breakeable 2.54mm Male Pins)
- LED (SK6812mini-e)(3mA) ~ $3 + Shipping [AliExpress](https://www.aliexpress.us/item/3256806781745425.html?spm=a2g0o.productlist.main.2.30f32c52NpVRiA&algo_pvid=19ea0063-2bd2-4e94-b170-fb60ab4e0a6e&algo_exp_id=19ea0063-2bd2-4e94-b170-fb60ab4e0a6e-1&pdp_ext_f=%7B%22order%22%3A%226%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21USD%212.23%212.23%21%21%2115.48%2115.48%21%40210328db17680140383654328ef58e%2112000038888086591%21sea%21US%210%21ABX%211%210%21n_tag%3A-29910%3Bd%3Ac04e790%3Bm03_new_user%3A-29895&curPageLogUid=fUqIvQ2YwTf7&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005006968060177%7C_p_origin_prod%3A) (For 20)
    
# THE END
     
So yeah thats it really
    
I spent about 19-20 hours on this. I learnt A LOT about Schematic/PCB design on KICAD specificaly. I also learnt how to get a project to manufacturing (Which I cant wait to get my first Devboard design to play with)
     
I do not plan to return to this project, I will probably at some point in the near future make another board but with a more specific use and maybe a diferent MCU so I can get more experience

# Thanks

- Myself (For all the time I put into this)
- [Kai Pereira](https://kaipereira.com/) (For the Guide)
- [HackClub](https://hackclub.com/) / [Blueprint](https://blueprint.hackclub.com/home) (For the opportunity to do a project like this)
- You (For reading this)
