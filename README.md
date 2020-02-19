# Temperature and dissolved nutrient effects on coral larvae  
Kitchen RM, Piscetta M, Lenz EA, de Souza MR, Schar D, Gates RD, Wall CB (2020) Symbiont transmission and reproductive mode influence responses of three Hawaiian coral larvae to elevated temperature and nutrients. *Coral Reefs*  

The goal of this project was to understand how different temperature and nutrient concentrations affect the larvae of three Hawaiian reef coral taxa: *Lobactis scutaria* (broadcast spawner, aposymbiotic larvae), *Pocillopora acuta* (brooder, symbiotic larvae), and *Montipora capitata* (broadcast spawner, symbiotic larvae).  

## R files and Folders  
  **markdown files**  
    *Coral-larvae-temp-and-nutrients.Rproj* -- the R project, where Rmd file and all scripts executed  
    *Kitchen-et-al.-larvae-temp-nutr.html*  -- the html output from R markdown  
    *Kitchen et al. larvae temp nutr.Rmd* -- the R-markdown file with script-code chunks  

## Treatment and biological data  
 **data folder**  
  - *larval size.csv* -- larvae size  
       *columns*
       *Species* = 3 species tested  
       *Treatment* = initial (day 0 prior to exposure), and Treatment codes for nitrate (N), phosphate (P), ambient (A) and high temp (H)   
       *Heat.Treatment* = none (prior to exposure), ambient (27C) and heated (29C)   
       *Nutrient.Treatment* = none (prior to exposure), control (no addition), added nitrate (N), phosphate (P) or both (NP)  
       *Date* = date in m/dd/yy  
       *tube.no* = identifier for each tube, 1-40  
       *tube.rep* = identifier for each replicate per treatment, 1-5   
       *larvae.no* = arbitrary number for larvae  
       *Area* = planar area in mm2  
         
          
  - *larval survivorship.csv* -- larvae survivorship     
       *Species* = 3 species used  
       *Tube* = replicate number  
       *Day.0* = larvae in each replicate tube for each treatment at start of experiment  
       *Day.1*...*Day.5* = survivorship of larvae in tube over days 1-5  
       *Month* = first run (month 1, preliminary data not used in study) and second run (month 2, used in study)  
       *Final.Survivorship* = proportion of larvae surviving at end of experiment (4 or 5 days)  
         
           
  - *respiration slopes.csv* -- larvae respiration rates   
       *Replicate* =  treatment replicate number 1-5  
       *Vial.no* = respiration measurement identifier, used to normalize respiration measurement by background values  
       *larvae.no* = number of larvae in vial  
       *Time.min* = time in minutes respiration rates were measured for in each vial  
       *r.squared* = r-squared value for slope of line best fitted to respiration measurements in each vial  
       *y.intercept* = y intercept of best fit line for each vial  
       *umol.s* = change in oxygen levels measured in umol per second  
       *umol.h* = change in oxygen levels converted to umol per hours  
       *Blank.slope* = respiration slope of each vial run as a blank (i.e. background level)  
       *umol.h.edit* = respiration rates normalized by background levels for each vial  
       *umol.h.larvae* = respiration rates further normalized by number of larvae still alive in each vial post respiration trials  
       *nmol.min.larv* = respiration rates per larva converted to nmol per min  
       *nmol.min.larv.cons* = rates multiplied by -1 to convey oxygen consumption rather than generation  
         
         
   - *symbiont density.csv* -- symbiont densities  
       *Tube.rep* = replicate tube  
       *no.larvae* = larvae in tube  
       *Initial.vol.ul* = initial volume of liquid in each vial measured in ul  
       *Grids.counted* = number of grids counted on hemocytometer    
       *Grid.vol.ul* = volume of liquid in counted grid squares  
       *Counts 1-7* = number of algal cells counted in each subsequent hemocytometer replicate   
       *Total.Counts* = average number of algal cells per vial  
       *Total.vial.concentration* = number of algal cells in entire volume of liquid in each vial  
       *Conc.per.larv* = average concentration of algal cells per larva   
       
   - *temp data.csv* -- temperature data  
       *Time* = date and time recorded by HOBO logger
       *Day* = timepoint measured as ‘Reading’ divided by ‘Total_Hours’
       *Reading* = number identifying each temperature measurement across experiment  
       *Total_Hours* = total number of 15 minute intervals in a 24 hour period (96)
         
         
 **figures folder**   
    - *combined.daily.survivorship.pdf* -- larvae survivorship for 3 coral species:  **this is Figure 3**  
    - *combined.resp.pdf* -- larvae respiration for 2 coral species (sans *L. scutaria*)  **this is Figure 4ab**  
    - *combined.size.pdf* -- change in larvae size for 3 species:  **this is Figure 5**  
    - *combined.symbiont.counts.pdf* -- symbiont counts for 2 species (sans *L. scutaria*)  **this is Figure 4cd**  
    - *combined.temp.pdf* -- temperature plot for 3 species:  **this is Figure 2**  
    - *Fig 1_coral.jpg* -- the multipanel figure of adult corals and larvae: **this is Figure 1**  
  - "final figures" **folder** has publication formatted figures and tables  
  
  
**nutrients folder**  -- dissolved inorganic nutrient concentrations
   - *nutrients_nitrogen.csv* -- nitrogen in seawater analyses  
       *columns*  
       *Species* = coral species  
       *Date* = date of measurement in m/dd/yy  
       *Descript.* = identifier  
       *Treatment* = treatment levels: FSW (filtered seawater), AC (ambient temp, control nutrients), AN (ambient temp, high nitrate), AP (ambient temp, high phosphate), ANP (ambient temp, high nitrate and phosphate), and H for high temperature.  
       *Heat.Treatment* = FSW, ambient or high (27 vs. 29C)  
       *Nutrient.Treatment* = FSW, control, 5uM Nitrate (N) added, 1uM Phosphate (P) added, 5uM N + 1 uM P  
       *N+N..umol.L* = nitrate + nitrite in umol L-1  
       *NO2..umol.L* = nitrite in umol L-1  
       *NO3..umol.L* = nitrate in umol L-1  
       
  - *nutrients_phosphate.csv* -- phosphate in seawater analyses  
       *columns* same as 'nutrients_nitrogen.csv' except...  
       *SRP..umol.L* = soluble reactive phosphate in umol L-1  
       
  - *SLAB.water.csv* -- nutrients in stock solutions analyzed by SLAB at UH Mānoa  
       *columns*  
       *Total.N..umol.L* = total nitrogen in umol L-1  
       *Total.P..umol.L* = total phosphorous in umol L-1  
       *Phosphate..umol.L* = phosphate in umol L-1  
       *N+N..umol.L* = nitrate + nitrite in umol L-1  
      


