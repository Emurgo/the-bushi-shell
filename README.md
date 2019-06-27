## CAD Comparison Analysis

Name | Price | Capabilities | Pros | Cons | Possible Uses 
---- | ----- | ------------ | ---- | ---- | -------------
Autodesk AutoCAD/Inventor | Free for students or 30-Day Free Trial | Modeling, assembling, and drafting prototypes as well as test product's durabilites using stress and dynmaic simulations | * Easy-to-Use / * Effective stuctual analysis system / * Short learning curve / * Installed STL file conversion | * Requires a lot of data / * At random times it crashes completely | Run accurate stuctural simulations on large assemblies
Onshape | Free for Students or 30-Free Trial | An online cloud-based CAD program that utilizes the same functions as other CAD programs such as Modeling, assembly, drafting and analysis | * All progress is saved in a private server so all work is automatically saved. / * Can be worked on any computer like Google docs. / * Community of professionals readibly accessible / * Easy to share to public | * Low graphic quality / * File inflexiblity (Cannot use files but you can store and redownload them) | Store copies of files created for future reference or to share in the public domain.
Fusion 360 | Free for Students, Hobbists and start-up companies* ; Other: $60/month or 30-Day Free Trial | A cloud-based CAD software that allows multiple users to work on a single project | * Keeps track of changes to a project / * Excellent graphics / * Able to run multiple structure tests simultaneously / * Ability to select individual components to export as STL files | * Difficult to customize software | Running a linked CAD file for easier visualization of progress made
Solidworks | Free for Students | Modeling, assembling, and drafting prototypes as well as test product's durabilites using stress and dynmaic simulations | * Short learning curve / * Built-in cost estimation feature / * Able to view complex surfaces | * Poor ergonomics / * Cannot handle large assemblies well | Calculate the cost of production for the project and what materials would be financially beneficial to use 
ThinkerCAD | Free for All | Modify geometric shapes to created complex designs | * Very easy to use / * Can import/export STL files at ease / * Can be used on any computer | * Requires consistant internet connection / * No structural analysis features / * Limited functions | Quick geometric edits to STL files 
FreeCAD | Free for All | Modeling, assembling, and drafting prototypes with unique features. | * Import and Export various CAD file formats / * Runs primarily on C++ / * Open-Source / * Multi-plaform usability / * Built-in Python Interpeter | * Not Suitable for production use / * Difficult to Use / * Intermidiate-Advanced learning curve / * No structural analysis features | Designing and assembling parts utilizing python for add-ons if necessary. 
Blender | Free for All | A software designed to create detailed 3D models for multi-purpose use | * Versatile / * Ability to model complex features / * Open-Sourced | * Steep learning curve / * No structual analysis tools | Create and edit detailed 3D models 

**Company must make <$100,000/yr or equivalent in foreign currency on goods and services*

## Pi Case Anaylsis 
 ### Steps for building a pi case: 
      
      1.) Plan 
          - Draw a model of the Pi with dimensions
          - Analyze what components will be used for the project 
          - Think about what material you would like to use because that could influence the strucutre of your design
                 
                 Here is an analysis of different material properies for the constuction of the outer casing:
                    
                    3D Printed Plastics: 
                          
                     ABS:
                     
                           Pros:
		                         - A thermoplastic that can be used in industrial applications
                             - Cheapest thermoplastic on the market
		                         - Semi-Flexable and shock resistant
		                         - Can withstand temps btwn -20°C to 80°C

                           Cons:
                             - Shrinks on contact with air
                             - Relieases fumes that causes headaches if not ventilated well
	                    
                      PLA: 
                      
                           Pros:
		                          - Biodegradable
		                          - Easiest to use
		                          - Can deteriorate in contact with water

                           Cons:
                             - Brittle 
                             - Attracts water easily which caused difficulty printing
	                    

	                    Carbon fiber:
                           
                           Pros:
		                         - High strength 
		                         - Lightweight
		                         - Can be mixed with other plasics to increase strength
                             - Prints very well
 
                           Cons:
                             - Very expensive 
                             - Abrasive to the printer (Can cause damage if not tuned to take abrasive material)
                             
                      Nylon:
                           
                           Pros:                      
                             - Lightweight
                             - Strong
                             - Wearproof 
                             - Flexable
                             - Thermo-resistant

                           Cons:
                             - WARNING: Nylon emits TOXIC fumes. DO NOT INHALE! May cause heavy irritation to the throat and lungs.
                             - Requires high temprature to melt plastic (>240°C)
                             
                      Polycarbon: 
                           
                           Pros:                      
                             - Shatter Resistant
                             - Heavy impact resistance
  
                           Cons:
                             - Requires a lot of heat (>= 300°C) to print
                             
                      Flexable PLA:
                           
                           Pros:                      
                             - Durable
                             - Extremely Flexable 

                           Cons:
                             - Must print slow to prevent clogs
                             - Very difficult to print with
          
      2.) Design
          - Integrate every aspect that would improve the performance of the item enclosed
          - Take into consideration the size of the case should have clearance of AT LEAST 0.4mm 
          - Model the whole case first then split it in two and if possible, try designing a snapfits for connecting the two
          - IMPORTANT: Always add ventilation to the case to prevent overheating
          
      3.) Test
          - Conduct internal structual analysis to ensure that the case can withstand a certain amount of force without damaging internal components
          - Export your model as an STL file or whichever file your tool can translate to construct the prototype
          - Configure the internal properties of the system
              - For 3D Printers: 
                  - For the strongest and most economical option, try printing with 15% infill and 4 Shells
                  - The more shells, the longer it takes to print but the stronger the product will become
                  
 ### Notes from other Designs
      - All current stakeboxes are simlar in design. These cases gives access to all the ports in the pi. 
      - The Casa node includes a interchangable power connection so people can use their device anywhere in the world. 
      - Some designs, such as the casa node, contains an external hard drive to increase diskspace for extra storage of transactions. 
 
 ## Case Design Ideas
    - The RockPi 4 has a power button but does not have a computing button, so in the design may include slots where we will manually add an LED light to indicate the status of the mechanism. 

## Objective
    
         
