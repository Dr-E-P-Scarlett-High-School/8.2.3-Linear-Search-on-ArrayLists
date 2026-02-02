# 8.2.3-Linear-Search-on-ArrayLists
In this exercise, you will code a modified version of sequential search from the previous example.  Here you should implement a method to do sequential search on an ArrayList of doubles and return the index of the search double, or -1 if it isn’t found.



public void run()
    {
        int[] arr = {9, 5, 7, 6, 3, 1, 4, 8};
        
        int index1 = linearSearch(arr, 9);
        System.out.println(index1);
        
        int index2 = linearSearch(arr, 3);
        System.out.println(index2);
        
        int index3 = linearSearch(arr, 90);
        System.out.println(index3);
    }
    
    /**
     * This method takes an array called array and a 
     * key to search for, and returns the index of
     * key if it is in the array or -1 if it is not
     * found.
     */
    public int linearSearch(int[] array, int key)
    {
        for(int i = 0; i < array.length; i++)
        {
            int element = array[i];
            if(element == key)
            {
                return i;
            }
        }
        return -1;
    }
