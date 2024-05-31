# CP2K_to_DEEPMDKIT : A Collection of Python Scripts to convert CP2K output to DEEPMD-KIT input. 


1. To obtain the box.raw file -
   Run the script named `convert_to_box_raw_from_cp2k.py` and input `5` for the number of rows, `19.00` for X, `19.00` for Y, and `19.00` for Z when prompted, the script will create a DataFrame with 5 rows, each containing the values (19.00, 19.00, 19.00) and save it to `box.raw'.

```sh
Enter the number of rows: 5
Enter the value for X: 19.00
Enter the value for Y: 19.00
Enter the value for Z: 19.00
```

2. To obtain the coord.raw file -
   Run the script named `convert_to_coord_raw_from_cp2k.py` and input the required values when prompted. For example, if you input `test.xyz` for the input file path, `5` for the number of atoms per frame, `0` for the starting snapshot number, and `5` for the ending snapshot number, the script will create a `.raw` file named `coord.raw`.

```sh
Enter the path to the input file: test.xyz
Enter the number of atoms per frame: 5
Enter the starting snapshot number: 0
Enter the ending snapshot number: 5
```
   
3. To obtain the `force.raw` and `energy.raw` files -
   Run the script named `convert_forces_and_energy_to_raw.py` and input the required values when prompted. For example, if you input `md-5.for` for the input file path, `120` for the number of atoms per frame, `0` for the starting snapshot number, and `5` for the ending snapshot number, the script will create two `.raw` files named `force.raw` and `energy.raw`.

```sh
Enter the path to the input file: md-5.for
Enter the number of atoms per frame: 120
Enter the starting snapshot number: 2000
Enter the ending snapshot number: 16000


