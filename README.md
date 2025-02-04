# NASSCOM-VSD-SoC
To run Openlane flow using 'picorv32a' design and calculate the flop ratio.
 To run the Openlane flow with the picorv32a design and calculate the flop ratio, follow these steps:
1.	Change the directory to Openlane
2.	Create an alias for running Docker
3.	Invoke OpenLane in interactive mode
4.	Write the Package require
•	cd Desktop/work/tools/openlane_working_dir/openlane
•	docker
•	./flow.tcl -interactive
•	package require openlane 0.9 

![image](https://github.com/user-attachments/assets/623edeff-fbe2-4190-bd37-ed196b950a7c)
![image](https://github.com/user-attachments/assets/310df91a-82ee-42be-a673-fd74348f37b9)
Now run synthesis using following command
run_synthesis
![image](https://github.com/user-attachments/assets/8535894e-bac9-4217-9c88-25a31c3f1a37)
Calculate the flop ratio
Flop ratio= Number of D Flip flops/ Total number of cells
percentage of DFF's = flop ratio x 100
Here Number of DFF is 1613 and total number of cells is 14876. My flop ratio is 10.842
![image](https://github.com/user-attachments/assets/0c9cf4b6-c934-4adf-9bbf-655f45c7cda6)
![image](https://github.com/user-attachments/assets/a02ff241-3106-4915-94d1-724b2716d86c)
Task-2
Calculate Die area in microns
Die area = (Die width x Die height)
Die width in microns=660685/1000=660.685 Microns
Die height in microns=671405/1000=671.405Microns
Area of die in microns=660.685∗671.405=443587.212Square Microns
![image](https://github.com/user-attachments/assets/85770105-2d4a-44d8-971f-3f4be1a5f94b)
![image](https://github.com/user-attachments/assets/22ad925e-1199-47ac-84d8-0a0c373afea0)
Once the MAGIC GUI opens, you should see the floorplan layout displayed in the tool.
We can now use the visualization tools in MAGIC (zoom, center, select cells, etc.) to inspect and analyze the floorplan.
•	Center the design: Press S to select the entire design and V to align it vertically on the screen.
•	Zoom in: Left-click and drag to select a specific area, then press Z to zoom in on that region.
![image](https://github.com/user-attachments/assets/50b3a3e0-bb67-42b7-91a8-8772ccd81b87)
Task-4
Run placement and run placement def in magic tool
Placement in VLSI Design
Placement involves deciding where to physically place standard cells (logic elements) within a chip. Placement can be broken down into two stages:
Global Placement: This assigns rough locations to cells, allowing some overlap. The goal is to create an initial layout that adheres to area constraints.
Detailed Placement: This refines the locations, ensuring there is no overlap and that cells are placed on legal sites, which directly impacts the routing stage. Use the following comamand to run the placement
run_placement
![image](https://github.com/user-attachments/assets/72b84845-d494-4e86-860e-02df7e49fff0)
![image](https://github.com/user-attachments/assets/0a15edfb-2a13-4d4f-aa81-c146e337db51)
![image](https://github.com/user-attachments/assets/92ed3912-92f5-468c-bcc0-999616cc6f3b)
![image](https://github.com/user-attachments/assets/84be5684-7998-49e4-821a-f1549b4de59e)
![image](https://github.com/user-attachments/assets/1645546f-b9d6-456a-9461-1f4710c4abf8)
![image](https://github.com/user-attachments/assets/92949ef3-45b0-4c83-aad1-2d7eae345d33)
![image](https://github.com/user-attachments/assets/a78df9a3-6755-4db0-bad0-f91a0a79e3c2)
![image](https://github.com/user-attachments/assets/84359a82-9adf-495e-80db-cc9c7c49a3d8)
![image](https://github.com/user-attachments/assets/1e48bd57-d8cd-4b42-9413-667d2586a515)



