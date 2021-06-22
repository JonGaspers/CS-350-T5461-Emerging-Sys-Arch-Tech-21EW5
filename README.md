# CS-350-T5461-Emerging-Sys-Arch-Tech-21EW5

# Milestone 3

### Summarize the project and what problem it was solving.

For milestone 3, I was tasked to create a state machine that looped SOS and OK in morse code using the LEDs on the CC3220S LAUNCHXL microcontroller. If the user presses a button, the board was supposed to finish the word it was on (SOS or OK) and then switch to the other word. This milestone was to learn how to use button interrupts, state machines, GPIO, and timers. 

### What did you do particularly well?

I feel that I did really well on making the state machine finish one word before switching to the other word. I decided to use bit fields to hold the sequence for the LEDs turning on and off to represent the SOS or OK. This saved on space and ensured that the word would finish before switching to the other word or repeating itself. 

### Where could you improve?

I could improve how I used the timer, I don't feel I used it correctly in this project and I would like to learn more about timer interrupts.

### What tools and/or resources are you adding to your support network?

After this milestone, I have added using bit fields to set up sequences that are binary (on/off) as I found them very useful and efficient. 

### What skills from this project will be particularly transferable to other projects and/or course work?

Learning how to use GPIO, State Machines and Timers are all really great skills that can be transferred to future projects that use microcontrollers.

### How did you make this project maintainable, readable, and adaptable?

I made sure to follow a consistent naming convention when naming variables and functions so they are clearly labeled and not confusing to anyone that reads the code. I also made sure to add comments that explained what the code was doing in various sections.

# 7-1 Project

### Summarize the project and what problem it was solving.

This was the final project for the course. In this project, I was supposed to turn the CC3220S LAUNCHXL microcontroller into a simulated smart thermostat. The board would need to use I2C to read the temperature of the TMP-006 temperature sensor on the board, detect button input to know if the user turned down/up the temperature, activate and LED if the heater is turned on, count seconds since activation, and finally, report to the "server" via UART.

### What did you do particularily well?

On this assignment, I felt I did particularily well with setting up the task scheduler that controlled the functionality of the simulated smart thermostat. 

### Where could you improve?

I originally wanted to setup task structs to better organize each of the tasks into a list then use a for loop to iterate through the list to activate various functions for the tasks. When working on the project, I couldn't figure out how to get this to properly work with the timer, so I would like to improve on this and try to get it working.

### What tools and/or resources are you adding to your support network?

I plan to add reading the technical documentation for the hardware I'm using to my support network. After reading through the board's user guide, I was better equiped to handle this project.

### What skills from this project will be particularly transferable to other projects and/or course work?

After working on this project, I feel that knowing how to set up a working task scheduler is a great skill to have for future projects. Not only would it be helpful on other microcontroller projects, but any application could need a task scheduler and knowing how to set them up would be very helpful. 

### How did you make this project maintainable, readable, and adaptable?

As with every programming assignment I work on, I make sure to properly name all variables and functions in a consistent naming convention so no one reading my code will be confused on what a variable is used for, or what a function is doing, or why it needed to be called. I also make sure to comment all of my code to provide context on what functions are doing, why and how they do it that way.
