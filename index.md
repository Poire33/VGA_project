---
layout: home
title: FPGA VGA Driver Project
tags: fpga vga verilog
categories: demo
---

I am using the Artix-7 FPGA board to display a French flag on a VGA monitor.

## **Template VGA Design**
### **Project Set-Up**
Summarise the project set-up and design flow. Include a screenshot of your own set-up, for example see the image of my Project Summary window below. Guideline 1 short paragraph.

<img src="https://raw.githubusercontent.com/Poire33/VGA_project/refs/heads/main/docs/assets/images/VGAPrjSum.png">

### **Template Code**
In the ColourStripes Verilog file, the French flag is constructed with `red_next`, `green_next`, and `blue_next`. Which color is displayed depends on the column pixels.

### **Simulation**
Explain the simulation process. Reference any important details, include a well-selected screenshot of the simulation. Guideline: 1/2 short paragraphs.

### **Synthesis**
<img src="https://raw.githubusercontent.com/Poire33/VGA_project/refs/heads/edits/docs/assets/images/Synthesis.png">
Describe the synthesis and implementation processes. Consider including 1/2 useful screenshot(s). Guideline: 1/2 short paragraphs.

### **Demonstration**
<img src="https://raw.githubusercontent.com/Poire33/VGA_project/refs/heads/edits/demo.jpg">

## **My VGA Design Edit**
This project is not very complicated. It does not involve any delays; it's just a static image.
### **Code Adaptation**
I modified the code related to the red, green, and blue values inside the if statements in the `always@*` begin to make a blue, white, and red stripe on the left, center, and right columns of the display respectively.
### **Simulation**
Show how you simulated your own design. Are there any things to note? Demonstrate your understanding. Add a screenshot. Guideline: 1-2 short paragraphs.
### **Synthesis**
Describe the synthesis & implementation outputs for your design, are there any differences to that of the original design? Guideline 1-2 short paragraphs.
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
