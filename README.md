# Two-Sum-II
We are provide with a sorted array and we need to take a target and print an output in an order that it adds upto target.
class Solution {
    public int[] twoSum(int[] numbers, int target) {
        int[] count = new int[2];
        int i = 0; //start pointer
        int j=numbers.length -1;// end pointer
        while(i<j){
            if(numbers[i]+numbers[j] == target){
                count[0] = i + 1;
                count[1] = j + 1;
                return count;
            }
            else if(numbers[i]+numbers[j]>target){
                j--;
            }
            else{
                i++;
                    
            }
        }
        return new int[1];
    }
}
