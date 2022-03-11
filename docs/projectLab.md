# Project Lab Documentation & Guides

![](_media/project-lab.jpg)

## About

The project lab is a space for working on both in-school curriculum based projects and for personal computer science related projects such that you have access to the schools resources. Whether it be a programming project that needs some extra computing power or 3D printing a model you created for a project, this is the space to do that.

This lab is maintained by students with support from the computer science and IT department.

### Features available in the lab

The project lab has many technologies available for student use.

1. **High Performance Computing Cluster (HPC)** - for data science, modeling, machine learning etc.
2. **General purpose computing** - there is a workstation and a server available for general use, whether it be for programming, 3d modeling or testing out code
3. **3D Printers** - there are two 3d printers available in the project lab that can be used with permission for printing
4. **Networking equipment** - there is an assortment of network equipment that can be used in a lab environment

## General Info

Below is the front of the server rack, with each device and their respective roles listed below

![](_media/server-rack.jpg)

1. **Network Router** - responsible for the internet connection
2. **Main Network Switch** - responsible for connecting all of the devices, it also has a fibre link (blue and orange cables) to the switch on the desktop
3. **Domain controller** - responsible for DNS and storing files
4. **GPU / Compute Server** - This is the high performance server that is responsible for all of the heavy computation tasks
5. Misc other equipment for messing around with

## Network Topology

The following chart outlines the structure of the LAN in the project lab. This network has a full 100mbps connection but no wireless available.

[![](https://mermaid.ink/img/pako:eNqFklFPwjAUhf_KTZ80YYNN0LkYEmADH5AQp_GB8dB1RSbdOrsCMYz_bgclQoTQp-bk5jv33nM3iPCYIhd9CpzP4c0LM1CvM3nlS0mFC9ajbVr3juk4pjUFw2hDOeyMTvW63YSnSNTbkAv-RYk0GI5MxglmJXRveklBONw9tBorG5oOjLkPwTqRZA4GvOAkgyGOtHK79-9WTqU3CqAO_YRRCKhYJYQWJXiTGXZn2CiUQgV4PK0IPZ5JwRlTyr6T4_4aWouJ-a_B6ZEh9E_Zg_E77JzPUm2tEZ7maldX0M8aHWOJI1xQ8A6fiwaW1opvdhHu7-ADDWc4lzw3qkjhg4tFIbFMeHaG3dLa-q_qygD-aY4qcp3hHuTRYnGcIaqhlAqVTayOa1MpIZJzmtIQueobY7EIUZhtVd0yV0uhfpxILpAagxW0hvBS8uAnI8iVYkkPRV6C1aGmumr7C0YU1-c)](https://mermaid.live/edit/#pako:eNqFklFPwjAUhf_KTZ80YYNN0LkYEmADH5AQp_GB8dB1RSbdOrsCMYz_bgclQoTQp-bk5jv33nM3iPCYIhd9CpzP4c0LM1CvM3nlS0mFC9ajbVr3juk4pjUFw2hDOeyMTvW63YSnSNTbkAv-RYk0GI5MxglmJXRveklBONw9tBorG5oOjLkPwTqRZA4GvOAkgyGOtHK79-9WTqU3CqAO_YRRCKhYJYQWJXiTGXZn2CiUQgV4PK0IPZ5JwRlTyr6T4_4aWouJ-a_B6ZEh9E_Zg_E77JzPUm2tEZ7maldX0M8aHWOJI1xQ8A6fiwaW1opvdhHu7-ADDWc4lzw3qkjhg4tFIbFMeHaG3dLa-q_qygD-aY4qcp3hHuTRYnGcIaqhlAqVTayOa1MpIZJzmtIQueobY7EIUZhtVd0yV0uhfpxILpAagxW0hvBS8uAnI8iVYkkPRV6C1aGmumr7C0YU1-c)

<!-- https://mermaid.live/edit#pako:eNptkV9rwjAUxb_KJU8bWP90buvKELStMnAi68YerA-xva7BtrekqUOs332pVljBPIXDyTm_3HtkIUXIbPYjeR7DpxtkoM949UGlQmnD4MXsDp6srmV1B2swjBFU8_GirffMYQWTO0cUIcHD82N_b8LQgiV54P8KFcZgwDsXGcz5plHuLz2TOrFyFz70YCoSBB_lXoRYVOCuttzecqPQCkpwKa0THMqUpCTRyutG9kYtjv76Xyp4bSBzeIW5PHSx2N2AgWm7d7b80mwOpbmexxnvZrXZVHvnjFmTkfBcUW7UI4ZvkrtCcSVIGxuEQ8ZTEcLb8vyadViKUn8z0vs41krAVIwpBszW14jLXcCC7KR9ZR5xhV4kFEmmm5ICO4yXivxDFjJbyRKvJldwvdu0cZ3-AAaxlWo -->

## Server Management

There are two main servers, the gpu server shown below, and the domain controller which hosts project files, serves the internet connection and can be used to host projects. This server will almost never need to be logged into or maintained as it runs 24/7 during school time. There will be instructions to follow on how to shutdown, startup, login and diagnose problems in the network.

![](_media/server-1.jpg)

Above is the main compute server with a 10 Core Intel Xeon CPU, 56 GB of RAM and an NVIDIA TESLA K80 graphics card.

### Logging Into the server

> Physical server credentials can be obtained by speaking to an CS teacher / Finn Lestrange

> For SQL server credentials / RDP credentials, they can be created for you by speaking to a CS teacher.

## Miscellaneous Lab Info
