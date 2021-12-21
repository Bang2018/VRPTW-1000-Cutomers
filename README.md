# VRPTW-1000-Cutomers
# Gehring & Homberger's 1000 customer instances
# Method: Machine Learning and Mixed Integer Programming (BigM and Subtour Elimination)

In Nov 2015, Quintiq shared the solution of the above problem instance using exact method. It is extremely difficult to use exact method for 1000 customers.
I have used an alternative approach to solve VRPTW problem with more customers. I have integrated Machine Learning technique with the traditional Mixed Integer Programming approach. I got same result.

You can download problem instance from https://www.sintef.no/projectweb/top/vrptw/homberger-benchmark/1000-customers/

You can download the resut from https://www.sintef.no/contentassets/51a833740c45438b99b2935fd1c057d1/c1_10_1.42478.95.sintef.txt

Method: Take subset of the above problem instance iteratively. Please check the .LP files I have created from each subset. Run LP files one after another and generate optimum route.

Computational Time: 14 secs to create LP file from each subset

                    Mip Gap: 0.01
                    
                    Max 2~10 secs to solve each LP file
                    
                    You can also use parallel processing to reduce computational time further
                    
Result :  
          C1_10_1_VRPTW_MIP_lAYER_0.lp :: 0->130->725->612->904->855->13->78->794->971->628->376->817->0
          
          C1_10_1_VRPTW_MIP_lAYER_1.lp :: 0->6->268->980->210->574->118->897->202->547->0
          
          Please run and verify the above results
         
               
