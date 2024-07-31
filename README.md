# java-array-questions
class swap{
    public static void main(String[] args) {
        int[] v={1,3,23,9,10};
        //swap(v,1,3);
        reverse(v);
        System.out.println(Arrays.toString(v));
    }
    // swaping values in an array
     static void swap(int[] v, int index1, int index2)
     {
         int temp=v[index1];
         v[index1]=v[index2];
         v[index2]=temp;
     }
     //reverse the array
     static void reverse(int[]v){
        int start=0;
        int end=v.length-1;
        while (start<=end){
        swap(v,start,end);
                start++;
                end--;

         }


