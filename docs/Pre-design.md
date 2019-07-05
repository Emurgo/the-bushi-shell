# Pre-Design Notes

- One of the major criteria for making this case open-sourced is to ensure that the whole case can be printed by any 3D printer. 

- To make this case 3D printer friendly, this design must be: 

      1.) Economical (Filament Use)
      2.) Structurally stable 

## Economics

- There are different ways to reduce the amount of filament on a project such as area reduction, infill vs shelling evaluations, and more. However, the method to save the most about of money and time would be by avoiding supports as much as possible. 

    - To avoid supports we must follow the YHT rule:

        - Y : Anything with this shape's angle (45° from vertical) can be printed normally and does not require supports. 
        - H : This would require bridging which will lead to complications depending on the size of the gap.
             > 36mm or less: Droops 0-0.5mm 

             > 36-60mm: Droops 0.5-2mm
             
             > 60mm or more: Droops 2-5mm 
        - T : Creating a shape like this will result in overhangs which means it would not be physically possible to print this properly without support. 

        *Note: **Avoid overhangs** as much as physically possible* 
- Ensure if your system does have overhangs you can:
         
         - a.) Insert a <= 45° chamfer 
         - b.) Insert a filet to the edge of the overhang
         - c.) Anchor to the main body 

     - All methods work but it depends on the type of design you are going for.  

## Physical Stability & Error Prevention

- With any design, it is important to ensure that it can withstand a large amount of stress and strain to prevent fractures. 

- To do this we need to conduct structural analysis and find weak points in our project. Common weakpoints may include:
   - Sharp corners or edges 
   - Large size transitions
   - Consistant radii 
- Solving these issues will improve the quality of your product and prevents any fractures from occurring.