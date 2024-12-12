# spminv

Simple IGBT motor inverter

Initial idea was independent but in 2024 when I started I borrowed
idea of heatsink from from STMBL project.

There are differences from STMBL, only one MCU located on power N potential,
1xCAN,2xRS422 RX and 2xRS485 RX/TX for encoder/communications and separated
by galvanical isolators.

Flyback power supply for 15V/3V3 on N side and 5V for isolated side. Thus only
input is 90-350V DC.
This is because my main usage is for spindle motors where driver is located near
spindle and not in remote cabinet.

Why not use STMBL ? I wanted to use different IPM, integrate it into CAN network
of my homemade CNC and to play with FOC by myself.

