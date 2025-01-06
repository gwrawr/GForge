# GForge

                    ********************************************************************************************************************
                          first time users please run ;gforge --setup or ;gforge --bag+BAGNOUN for at least two bags                                         
                    ********************************************************************************************************************
                                                                                                                                        
                                                                                                                                        
                      FLAGS   --help              display this                                                                          
                      *****   --setup             enter setup GUI                                                                       
                              --options                                                                                                 
                              --configure                                                                                               
                              --gui                                                                                                     
                                                                                                                                        
                              --nobuy             do not allow buying                                                                   
                              --material=XYZ      set material to XYZ                                                                   
                              --mithril           set material to mithril                                                               
                              --metal=                                                                                                  
                              --wood=                                                                                                   
                                                                                                                                        
                              --product=abcXYZ    set product to abcXYZ                                                                 
                                                  eg --product=shortsword                                                               
                                                                                                                                        
                              --handle            make handles ON                                                                       
                              --shaft                                                                                                   
                              --hilt                                                                                                    
                              --haft                                                                                                    
                                                                                                                                        
                              --head              make heads/blades ON                                                                  
                              --blade                                                                                                   
                                                                                                                                        
                              --iterations=X      complete X iterations                                                                 
                              --i=X               eg:     --handle --i=4      will make 4 best handles                                  
                               -i=X               eg:     --iterations=4      will make 4 of each handle and head                       
                                                                                                                                        
                              --vise              combine handles and heads ON (OFF by default with no args)                            
                              --combine                                                                                                 
                                                  eg  -vise --i=2 will attempt to create 1 perfect from up to 2 handles and hafts       
                                                                  that are already made                                                 
                                                      --handle --haft --vise attempts to make 1 perfect from scratch, with 1 attempt    
                                                                                                                                        
                              --make=             only valid with vise/combine flag, attempt to make this many perfects                 
                                                  eg --vise --i=10 --make=2 will attempt to create 2 perfects with 10 combines          
                                                     --vise     will attempt to make 1 perfect from all available components            
                                                                                                                                        
                              --dump              trash products                                                                        
                                                                                                                                        
                              --bag+              eg --bag+cloak will add the noun cloak to the list of containers                      
                              --bag-              eg --bag-cloak will remove the noun cloak from the...                                 
                                                                                                                                        
                              --appraise          appraise the quality of all compenents that match the product
                                                                                                                                        
                      BEGINNER Forgers:                                                                                                 
                      ********    1) Train crafting to 500 making bronze forging-hammer-heads and forging-hammer-handles                
                                  2) Make a few best magical hammer-heads and hammer-handles in equal numbers                           
                                  3) Combine your perfect forging-hammer using the vise flag or Forge: Weapons                          
                                  3) Train your weapon crafting skill to 500 using brozne with increasingly difficult glyphs            
                                                                                                                                        
                    ********************************************************************************************************************
                    ********************************************************************************************************************










- soon to be refactored into the following organization



# GForge module
- packages utility classes with the GForger class

## GForger class
- crafts, forges, and assembles 

## DProduct class
- stores data for each weapon, names of glyphs and componenerts

## Material class
- stores data for materials such as oil type

# GUtil module

## GShopper class
- buys materials and banks, exchanges

## GBagger class
- manipulates inventory

## GSettings class
- sets default, imports current, updates settings

## GInterface class
- parses command strings
- manages gui

## GIO class
- displays output and receives input from console
  gError method
  gWarn method
  gAlert method
  gDebug method
