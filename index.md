# Atari Punk Synthesizer 
My project is an Atari Punk Synthesizer, an analog electronic instrument that generates a variety of retro-style sounds using a 556 timer chip. The user can adjust the pitch, tone, and volume with  potentiometers to create different sound effects.

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Grace G | Lynbrook High School | Mechanical Engineering | Incoming Senior

![Headstone Image](logo.svg)
  
# Final Milestone

<iframe width="560" height="315" src="https://www.youtube.com/watch?v=eSRVPmxoq2w" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Description 
For my final milestone, I transformed my breadboard prototype into a much more permanent and portable synthesizer. I transferred the entire circuit onto a solderable perfboard, which replaced the temporary jumper-wire connections with soldered electrical connections. I also designed and 3D modeled a custom enclosure using CAD to organize and protect the electronics.

![Milestone Image](m3image.jpeg)
![Milestone Image](m3image2.jpeg)

## Final Design

### Perfboard Assembly
The largest change was transferring every component from the breadboards onto solderable breadboards and a perfboard.

Unlike a breadboard, where components can simply be plugged in, every electrical connection on a perfboard must be made manually using solder. This required carefully planning the layout before soldering to avoid crossing wires and to keep the circuit organized.

Moving to a perfboard also reduced the number of loose jumper wires, making the synthesizer much easier to transport.

![Milestone Image](m3perf.jpeg)
![Milestone Image](m3perf2.jpeg)
![Milestone Image](m3perf3.jpeg)


### CAD

After completing the electronics, I designed a custom enclosure using CAD software.

The enclosure holds the perfboards securely while providing openings for the potentiometers, push buttons, switches, LEDs, and speaker. Creating the enclosure required measuring the dimensions of every component and arranging the layout so the controls were easy to reach while keeping the overall design compact.

![CAD Image](556cad.png)
![CAD Image](LFOcad.png)

## Challenges

The biggest challenge during this milestone was soldering the circuit onto the perfboard. Unlike the breadboard, where mistakes could be corrected in seconds, every solder joint was a permanent electrical connection. Planning where each wire should go, especially the shared ground connections, was much more difficult than I expected.

I also discovered that soldering itself requires practice. Sometimes the solder would not flow properly or would create weak joints that had to be removed and redone before the circuit would work reliably.

Although the synthesizer functions, some of the potentiometer connections are still mechanically weak, causing the circuit to work only intermittently. Debugging these problems taught me that a reliable electronic device depends not only on the circuit design but also on the quality of the physical construction.

## Future Improvements

Although the synthesizer is complete, there are still several improvements I would like to make.

First, I want to strengthen the potentiometer connections so the circuit operates more reliably. I would also like to redesign parts of the wiring layout to make the internal connections cleaner and easier to maintain.

In the future, I'd also like to expand the synthesizer by adding a keyboard, additional oscillators, and more sound effects to create an even wider variety of sounds.

# Second Milestone
<iframe width="844" height="475" src="https://www.youtube.com/embed/k7cU7gvNjDI" title="Grace G. Milestone 2" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Description 
For my second milestone, I expanded the original Atari Punk Synthesizer by adding several new modules that give me more control over the sound. Other than simply producing electronic tones, the synthesizer can now generate modulation effects, amplify its audio output, and offer much greater control over how the sound is changed.

### Updated Circuit Diagram
Unlike the first milestone, this stage involved integrating multiple independent circuits into one system. Because of the increased complexity, I switched from Tinkercad to Fritzing, which offers a wider selection of electronic components and makes it easier to represent my circuit accurately.

![Milestone Image](fritizing.png)

## Overall Design
The synthesizer now consists of three main subsystems: the original 556 timer circuit that generates the sound, the XR2206 low-frequency oscillator that modulates the sound, and the LM386 amplifier that boosts the output.

![Milestone Image](m2project.png) 

## Components 
### LM386 Audio Amplifier
One of the largest additions was an LM386 audio amplifier, which strengthens the audio signal produced by the synthesizer before sending it to the speaker.

The audio signal enters pin 3 through the 5 kΩ volume potentiometer. The LM386 amplifies this signal, which then exits through pin 5, passes through a coupling capacitor, and finally reaches the speaker. Several capacitors were also added around the amplifier to improve power stability and reduce unwanted noise. Because the amplifier is powered by its own battery, I also added an LED to indicate when it is receiving power.

![Milestone Image](amplifier.jpeg)

### XR2206 Low-Frequency Oscillator (LFO)
Another major addition was an XR2206 function generator, which works as a Low-Frequency Oscillator (LFO).

Unlike the 556 timer, which creates audible frequencies, the XR2206 generates frequencies below approximately 20 Hz. Since these frequencies are below the range of human hearing, they are not heard directly. Instead, the LFO changes the frequency of the 556 oscillators, producing modulation effects such as vibrato.

I have a total of 3 potentiometers. The first potentiometer is connected to pin 7 which then controls the LFO speed, allowing the modulation to range from slower to much faster oscillations.

The LFO signal leaves pin 2 of the XR2206 and is divided into two independent paths. Each path contains its own **100 kΩ potentiometer** followed by a **10 kΩ resistor** before connecting to one of the two control inputs on the 556 timer(pins 3 and 11). This allows me to independently adjust how much modulation each oscillator receives, giving me much more control over the synthesizer's sound. 

LFOimage.jpeg

## Challenges

The biggest challenge during this milestone was integrating all of the new components together. Although there were many tutorials explaining the audio amplifier, the function generator, and the 556 timer individually, I could not find instructions showing how to combine them into a single synthesizer. Because of this, I spent much of my time reading datasheets to understand the purpose of each pin instead of simply following tutorials. I experimented with different resistor values, wiring configurations, and modulation methods until the individual modules finally worked together.

Testing also proved more difficult than I expected. Since everything was still assembled on breadboards, every work session began by checking that each jumper wire was fully inserted. Even one loose connection could prevent the entire synthesizer from working. To improve this, I replaced several jumper wires with flatter connections that fit more securely into the breadboard.

Overall, this milestone taught me that building electronics is not only about assembling circuits—it is also about understanding how different systems communicate and learning how to interpret datasheets when no complete instructions exist.

## Next Steps 
For my final milestone, I plan to solder the complete circuit onto a perfboard/solderable breadboard to create a more permanent version of the synthesizer. I also plan to design a custom CAD enclosure that organizes the electronics into a portable case instead of an exposed breadboard. Finally, I plan to improve the overall layout of the synthesizer by organizing the wiring.

# First Milestone

<iframe width="860" height="484" src="https://www.youtube.com/embed/eSRVPmxoq2w" title="Grace G. Milestone 1" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Description 
For my first milestone, I built the basic version of the Atari Punk Synthesizer on the breadboard.

![Milestone Image](m1_project.jpg) 

### Tinkercad Schematic 
![Milestone Image](m1_tinkercad.png) 


Before building the physical circuit, I recreated the entire design in Tinkercad. This allowed me to verify that the circuit worked before assembling it on the breadboard. To keep the schematic easy to read, I color-coded all of the wires. Red wires are connected to positive power, black wires are connected to ground, and blue wires represent all other signal connections.

The goal of this milestone was to create a functioning synthesizer that could generate different electronic tones using analog circuits. Building the circuit on a breadboard also allowed me to easily test, troubleshoot, and modify the design before creating a permanent version.

## Components 

### 556 Timer 
The Atari Punk Synthesizer is built around a 556 timer integrated circuit, which contains two 555 timers inside a single chip. These timers work together to generate square-wave signals that produce the sound. The first timer works as an oscillator that generates square waves at a specific frequency which is determined by the connected capacitors and resistors. The second timer is also set up as an oscillator and works by modulating the first timer, creating the electronic sounds that the Atari Punk Synth is known for.

![Milestone Image](556timer_image.png)

### Potentiometers
The synthesizer uses three potentiometers:

* Two 500kΩ potentiometers control different aspects of the oscillator frequencies, allowing the pitch and tone to be changed 
* One 5kΩ potentiometer controls the output volume by adjusting the signal sent to the speaker.

### Capacitors
The capacitors are used to determine the timing of the oscillators because the speaker converts the electrical square-wave signals into actual sound. Together, these components create an analog synthesizer that can produce a wide range of electronic tones.

## Challenges
One of the biggest challenges I faced was learning how to use both Tinkercad and breadboard circuits, since I had very little experience with either before starting this project. So this challenge came with troubleshooting the circuit when it initially failed to produce any sound. 

During troubleshooting, we used an oscilloscope which lets us see the electrical signals in the circuit. The oscilloscope displays how voltage changes over time. This helped us check whether the 556 timer was producing the expected square wave output.  

We also used a function generator, which produces electrical signals such as square, sine, and triangle waves. It can be used to inject known signals into a circuit to test individual places and help find the source of the problem.

Eventually, I discovered that the speaker wires were not making good contact with the breadboard. After fixing that connection, the synthesizer immediately started working. This experience taught me that even a small connection issue can prevent an entire circuit from functioning and the importance of carefully checking every component during troubleshooting.

## Next Steps

For my next milestone, I plan to transfer the breadboard circuit onto a soldered perfboard to create a more permanent version of the synthesizer. I also want to start thinking and planning about how to expand the synthesizer by adding additional components that will provide more control over its sound.

# Starter Project 

<iframe width="860" height="484" src="https://www.youtube.com/embed/EVD8lXy4kp4" title="Grace G. Starter Project" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Description 


** image 

## Challenges 

## Next Steps 

# Bill of Materials

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| A500K Potentiometers | What the item is used for | $9.99 | <a href="[https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/](https://www.amazon.com/gp/aw/d/B0FS4T2ML7/?_encoding=UTF8&pd_rd_plhdr=t&aaxitk=21158059054e5e22ef3df0e1f43514c2&hsa_cr_id=0&qid=1785531890&sr=1-2-9e67e56a-6f64-441f-a281-df67fc737124&i=aps&aref=aBBqfD5aNB&ref_=sbx__sbtcd_asin_1_title&pd_rd_w=f66Wu&content-id=amzn1.sym.8de9b3d5-f5c5-40e9-9b39-d65f08d6ea68%3Aamzn1.sym.8de9b3d5-f5c5-40e9-9b39-d65f08d6ea68&pf_rd_p=8de9b3d5-f5c5-40e9-9b39-d65f08d6ea68&pf_rd_r=BK1D6ZDM0Z03XTNXD623&pd_rd_wg=x0u1P&pd_rd_r=c04424b2-953e-4b3c-a43b-93fbf1aff35c&th=1)"> Link </a> |
| 556 Timer | What the item is used for | $5.99 | <a href="[https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/](https://www.amazon.com/HUABAN-10PCS-NE556N-DIP-14-Timers/dp/B0H35ZZLVT/ref=sr_1_7?crid=3G1CR8S31687X&dib=eyJ2IjoiMSJ9.l2fZ3jrj-p3mM3q6er9HjeCNHd9bnzpVuQyzyEwj1Yvz_DG56Al3dnOCGGmO6ebosqqxtRGDOibOV28Ad-Nq_uiSUPJ_A4UJ_0JcSN2vTOPkyz_S7jc-7V1c5sRVoDNNw4oVZQ7Wa52M7KU06xTs7w.UcCIleFKo1rgZz8zUPkm5NAYCg_OxX3202atKWhoos0&dib_tag=se&keywords=556+timer+chip&qid=1785532286&sprefix=556+timer%2Caps%2C175&sr=8-7)"> Link </a> |
| XR2206CP | What the item is used for | $5.37 | <a href="[https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/](https://www.amazon.com/XR2206CP-DIP16-XR2206-2206CP-DIP-16/dp/B0BGR97PKC/ref=sr_1_3?crid=3DOI4ZDC5CUQM&dib=eyJ2IjoiMSJ9.GUzKZXrExOXuV3JEdEQe3Jjiz7UBFkHg9Yl0fBf9QK8A1HdXT8Sy9rMxVhYyTAvd2KKhtTHoxZkdaFVPHeGJDmTPoSR8Ycy2QD2It8lD2k91gLknbJ9RWlb_JrIu9qc2.nJ_bp-fCreSgH3ypljlTtwNN-iTyzkVPP63zraszzok&dib_tag=se&keywords=XR2206+chip&qid=1785532056&sprefix=xr2206+chip%2Caps%2C194&sr=8-3)"> Link </a> |
| LM386N Audio Power Amplifier  | What the item is used for | $6.99 | <a href="[https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/](https://www.amazon.com/BOJACK-LM386N-Voltage-Amplifier-semiconductor/dp/B07WQWR89Q/ref=sr_1_1_sspa?crid=3M6CZDC26I9LX&dib=eyJ2IjoiMSJ9.5nylNsAnC-rLn9JojTvHSk66ldr7pgP8v8OtGpzvgYGnI3Zki9N0vnc2qhxKN9-1y3G68pRSgrPGLuMijqUzEh6X3lZsncKkRH5DROT86AyjbtmGkNSX8LMXNeXlMqxCzhPLL7RTbXuaLUzW-EoUlrmFif2S4zPxx-PP5yo20QI1Nm1tyKbI72wAbp2KYwMXFt46CvMOVtQGQn1fapqsI_wqPH4Rzgyq1D-Jjn39j5Y.bgd6cv__BsDGPnnisikwRG5wZW7mlyE15LYDLbnNpvY&dib_tag=se&keywords=lm386&qid=1785532110&sprefix=lm3%2Caps%2C196&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1)"> Link </a> |
| 10k Resistors | What the item is used for |
| 5k Potentiometer | What the item is used for |
| Solderable Breadboard | What the item is used for |
| Perfboard | What the item is used for |
| 8ohm Speaker | What the item is used for | $6.99 | <a href="amazon.com/Speaker-Speakers-Compatible-Loudspeaker-Player/dp/B0C49QZ99X/ref=sxin_16_pa_sp_search_thematic_sspa?content-id=amzn1.sym.292df443-b323-44ae-8b40-9a666975b8b5%3Aamzn1.sym.292df443-b323-44ae-8b40-9a666975b8b5&crid=1EMP3LBHF1QI2&cv_ct_cx=8+ohm+speaker&keywords=8+ohm+speaker&pd_rd_i=B0C49QZ99X&pd_rd_r=90f93b48-6bc2-49b6-a5c8-828d97dc38d9&pd_rd_w=j6Mfb&pd_rd_wg=In2zB&pf_rd_p=292df443-b323-44ae-8b40-9a666975b8b5&pf_rd_r=22RKHH7J93W0AV496CW4&qid=1785533087&sbo=RZvfv%2F%2FHxDF%2BO5021pAnSA%3D%3D&sprefix=8ohm+spekae%2Caps%2C168&sr=1-1-6024b2a3-78e4-4fed-8fed-e1613be3bcce-spons&aref=a2589Gplrr&sp_csd=d2lkZ2V0TmFtZT1zcF9zZWFyY2hfdGhlbWF0aWM&psc=1"> Link </a> |
| Toggle Switch | What the item is used for |
| 9V Battery | What the item is used for | $8.99 | <a href="https://www.amazon.com/PKCELL-9V-Batteries-Battery-Detector/dp/B00ZTS55Y4/ref=sr_1_1_sspa?crid=RNX79Q7YHA6L&dib=eyJ2IjoiMSJ9.LzVLI_Okv1aX44UDnl3M2-RS4ssR57PghTC3OPi9-RcyeCPVkGbxCnf_hdsU6ckWZYZtaYQ0z9cdWUxbIPKxL_8--2HJnpuac4xQ2g6v9VZvO8l9Hwf4Irc-JhhuJwBOMD8waBPYtzrCgzHibz2T4G5bcZXnysWjDl2QameNTvevaikkIW_0sUj7uy2p2N86H6UvNVYaJvicOqSgWdwIcwBIXcvmWaSw5AlBmaYFSQeV-xmeCVo6Gk18vxF6vgy3Oiy12ofGkv7MIM_lKcKvstWEQqR9-cA8O3FYOx3icEY.P3byZaG0E1jxYHfdnqy6Z57GiRkDCZr6cSJf-h0VQ3Q&dib_tag=se&keywords=9v+batteries&qid=1785533254&rdc=1&sprefix=9v+b%2Caps%2C212&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1)"> Link </a> |
| 100k Potentiometers | What the item is used for | $6.99 | <a href="[https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/](https://www.amazon.com/Ferwooh-Adjustment-Single-Linear-Potentiometer/dp/B0CZ74CL2T/ref=sr_1_3?crid=2UMRRASFYYDZN&dib=eyJ2IjoiMSJ9.S1or234AqZVS13T9PN1sC2zoUMMVc1wryzrpYzjzpgyR6v_k-SskTkRmMHhiJ7vDGQmbbbl0skwQu-WchAH0LfKPV-mN_k4hand60FSawSgHhNdLpiAdGZLBcyoaoDwmuDVWBOT8_SbxyHZhn4UHxIhkpJenyQ9y4PBdxSgkDmQOdYoiO5owhc3t25UBfYzDaKrF1tfTsyRkpfKtCfZy7zQqx6kEqZh3uCYE1UXEzyk.atFbSvIAHfPHMsj6OzX1QWDbHkT2VjEeX4uVGv8cjXw&dib_tag=se&keywords=100k%2Bpotentiometer&qid=1785533231&sprefix=100k%2Bpo%2Caps%2C222&sr=8-3&th=1)"> Link </a> |
| 10u Capacitors | What the item is used for |
| 100u Capacitors | What the item is used for |
| 1000u Capacitor | What the item is used for |

# Other Resources/Examples
- [Build an Atari Punk Circuit on a Breadboard](https://www.instructables.com/Build-an-Atari-Punk-circuit-on-a-breadboard/)
- [Let's Build (Analogue Synth)](https://www.instructables.com/Lets-Build-Analogue-Synth/)
- [XR-2206 - Monolithic Function Generator](https://cdn.sparkfun.com/assets/8/a/b/3/9/XR2206.pdf)

