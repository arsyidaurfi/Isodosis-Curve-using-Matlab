# Isodosis-Curve-using-Matlab

Isodose curve is a curve that relates the same doses to a certain depth under the skin. Isodose curve serves to see how much radiation will be received at the target volume or critical organs. The steps for making an isodose curve are as follows: 

Step 1. Interpolate dose and PDD data, in a range according to field area and scale on PDD.

Step 2. Normalize the data (with excel). The dose data was normalized in the range of 0 to 1 with the Min-Max transformation. PDD data is transformed into % or multiplied by 100. 

Step 3. Calculation of xi (position x at a depth of n cm). The value of xi is calculated by projecting to xn (position x at depth d). Here are the equations:
        xi=  (f x)/(f+d), where f is the SSD (source to surface distance)
        
Step 4. Interpolate the dose on xi
Step 5. Calculation of D value (with excel). D is the product of PDD with the dose profile on the surface (OA). The following formulates the formula D at point P which is at depth d, and the horizontal distance is xn.
        D = PDDd x OAn
        Where PDDd is the dose inside d, while OAxi is the dose with a distance of xi on the surface dose profile.

Step 6. Making Isodosis Curve

