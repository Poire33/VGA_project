---
layout: home
title: FPGA VGA Driver Project
tags: fpga vga verilog
categories: demo
---

I am using the Artix-7 FPGA board to display a French flag on a VGA monitor.

## **Template VGA Design**
### **Project Set-Up**
This project is not very complicated. It does not involve any delays; it's just a static image.

<img src="https://raw.githubusercontent.com/Poire33/VGA_project/refs/heads/main/docs/assets/images/VGAPrjSum.png">

### **Code**
In the ColourStripes Verilog file, the French flag is constructed with `red_next`, `green_next`, and `blue_next`. Which color is displayed depends on the column pixels. Fom column 0 to 214, red and green is switched off and blue is fully on. From column 215 to column 429, all of red, green, and blue are all fully on to display white. Finally, from column 430 to 640, only the red is activated.

### **Simulation**
<img src="https://raw.githubusercontent.com/Poire33/VGA_project/refs/heads/edits/docs/assets/images/Simulation%202.png">
The simulation process displays the waveforms seen above in software on a graph. It demonstrates how each of the red, green, and blue signals are timed.

### **Synthesis**
<img src="https://raw.githubusercontent.com/Poire33/VGA_project/refs/heads/edits/docs/assets/images/Synthesis.png">
Among other things, the synthesis process genereates a low-level circuit diagram, seen above, as well as a netlist.

### **Demonstration and code adaptation**
<img src="https://raw.githubusercontent.com/Poire33/VGA_project/refs/heads/edits/demo.jpg">

I modified the code related to the red, green, and blue values inside the if statements in the `always@*` begin to make a blue, white, and red stripe on the left, center, and right columns of the display respectively.
### **Schematic**
<img src="https://raw.githubusercontent.com/Poire33/VGA_project/refs/heads/edits/docs/assets/images/Schematic.png">

## **More Markdown Basics**
This is a paragraph. Add an empty line to start a new paragraph.

Font can be emphasised as *Italic* or **Bold**.

Code can be highlighted by using `backticks`.

Hyperlinks look like this: [GitHub Help](https://help.github.com/).

A bullet list can be rendered as follows:
- vectors
- algorithms
- iterators

Images can be added by uploading them to the repository in a /docs/assets/images folder, and then rendering using HTML via githubusercontent.com as shown in the example below.

<img src="https://raw.githubusercontent.com/melgineer/fpga-vga-verilog/main/docs/assets/images/VGAPrjSrcs.png">
