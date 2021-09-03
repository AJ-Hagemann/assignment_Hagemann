# assignment_Hagemann
	//AJ Hagemann
	//Operating Systems
	//Project 6, Sum Square Difference
	
	#include <stdio.h>
	#include <math.h>
	
	//This is the funciton that squares the number input
	int squared(int tempnum)
	{
	    int results;
	    results = tempnum * tempnum;
	    return results;
	}
	
	int main()
	{
	    int whilecount = 0;
	    int sumofsqu = 0;
	    int squofsum = 0;
	    int squofsumnum = 0;
	    int finalres = 0;
	    int squtemp;
	    int sumtemp;
	    
	    //while loop that houses both the for loops that cycle 100 times and calculate the square sum and sum squared
	    while(whilecount < 1){
	        for(int squtemp = 1; squtemp <= 100; squtemp++){
	            squofsum = squofsum + squared(squtemp);
	            if(squtemp == 100){
	                printf("squofsum is: %d\n",squared(squtemp));
	            }
	            else{
	                continue;
	            }
	        }
	        for(int sumtemp = 1; sumtemp <= 100; sumtemp++){
	            sumofsqu = sumofsqu + sumtemp;
	            if(sumtemp == 100){
	                printf("sumofsqu is: %d\n", sumofsqu);
	            }
	        }
	        //Ends the while loop and squares the the sum to get the final number
	        whilecount = whilecount + 1;
	        squofsumnum = squared(sumofsqu);
	    }
	    //Print and return statments
	    printf("Square of the sum number: %d\n", squofsumnum);
	    finalres = squofsumnum - squofsum;
	    printf("Difference between to two: %d\n", finalres);
	    return 0;
	}

