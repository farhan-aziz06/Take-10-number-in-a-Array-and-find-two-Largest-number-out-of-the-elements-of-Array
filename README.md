# Take-10-number-in-a-Array-and-find-two-Largest-number-out-of-the-elements-of-Array
Input 10 number in a Array and find two Largest number out of the elements of Array



            import java.util.Scanner;

            public class arrays {
                public static void main (String [] args){
                    Scanner console = new Scanner(System.in);
                    int [] array = new int[10];
                    System.out.print("Enter Array Element:");
                    for (int i = 0; i<= args.length; i++){
                        array[i]= console.nextInt();
                    }
                    int largest = array[0];
                    for (int i =0; i<10; i++){
                        if (array[i]>largest)
                            largest=array[i];
                    }
                    int largest2;
                    if (array[0]==largest)
                        largest2=array[1];
                    else
                        largest2=array[0];
                    for (int i =0; i<10;i++){
                        if (array[i]!=largest)
                            if(array[i]>largest2)
                                largest2=array[i];

                    } 
                    System.out.println("Largest= "+largest);
                    System.out.println("2nd Largest= "+largest2);
                }
            }

