# Atari Punk Synthesizer 
Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!

You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:
```HTML 
<!--- This is an HTML comment in Markdown -->
<!--- Anything between these symbols will not render on the published site -->
```

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Grace G | Lynbrook High School | Mechanical Engineering | Incoming Senior

**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**

![Headstone Image](logo.svg)
  
# Final Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/watch?v=eSRVPmxoq2w" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE



# Second Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/y3VAmNlER5Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your second milestone, explain what you've worked on since your previous milestone. You can highlight:
- Technical details of what you've accomplished and how they contribute to the final goal
- What has been surprising about the project so far
- Previous challenges you faced that you overcame
- What needs to be completed before your final milestone 

# First Milestone

<iframe width="860" height="484" src="https://www.youtube.com/embed/eSRVPmxoq2w" title="Grace G. Milestone 1" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Description 
For my first milestone, I built the basic version of the Atari Punk Synthesizer on the breadboard.
"pls insert picture here grace"

### Tinkercad Schematic 
"pls insert picture here grace"

Before building the physical circuit, I recreated the entire design in Tinkercad. This allowed me to verify that the circuit worked before assembling it on the breadboard. To keep the schematic easy to read, I color-coded all of the wires. Red wires are connected to positive power, black wires are connected to ground, and blue wires represent all other signal connections.

The goal of this milestone was to create a functioning synthesizer that could generate different electronic tones using analog circuits. Building the circuit on a breadboard also allowed me to easily test, troubleshoot, and modify the design before creating a permanent version.

## Components 

### 556 Timer 
The Atari Punk Synthesizer is built around a 556 timer integrated circuit, which contains two 555 timers inside a single chip. These timers work together to generate square-wave signals that produce the sound. The first timer works as an oscillator that generates square waves at a specific frequency which is determined by the connected capacitors and resistors. The second timer is also set up as an oscillator and works by modulating the first timer, creating the electronic sounds that the Atari Punk Synth is known for.

* add picture

### Potentiometers
The synthesizer uses three potentiometers:

* Two 500kΩ potentiometers control different aspects of the oscillator frequencies, allowing the pitch and tone to be changed 
* One 5kΩ potentiometer controls the output volume by adjusting the signal sent to the speaker.

### Capacitors
The capacitors are used to determine the timing of the oscillators, while the speaker converts the electrical square-wave signal into audible sound. Together, these components create a simple but versatile analog synthesizer capable of producing a wide range of electronic tones.

## Challenges
One of the biggest challenges I faced was learning how to use both Tinkercad and breadboard circuits, since I had very little experience with either before starting this project. So this challenge came with troubleshooting the circuit when it initially failed to produce any sound. 

During troubleshooting, we used an oscilloscope which lets us see the electrical signals in the circuit. The oscilloscope displays how voltage changes over time. This helped us check whether the 556 timer was producing the expected square wave output.  

We also used a function generator, which produces electrical signals such as square, sine, and triangle waves. It can be used to inject known signals into a circuit to test individual places and help find the source of the problem.

Eventually, I discovered that the speaker wires were not making good contact with the breadboard. After fixing that connection, the synthesizer immediately started working. This experience taught me that even a small connection issue can prevent an entire circuit from functioning and the importance of carefully checking every component during troubleshooting.

## Next Steps

For my next milestone, I plan to transfer the breadboard circuit onto a soldered perfboard to create a more permanent version of the synthesizer. I also want to start thinking and planning about how to expand the synthesizer by adding additional components that will provide more control over its sound.

# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```c++
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  Serial.println("Hello World!");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```

# Bill of Materials
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |

# Other Resources/Examples
- [Build an Atari Punk Circuit on a Breadboard](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

