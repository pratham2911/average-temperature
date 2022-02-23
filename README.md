    //find number of days the temperature is above average temmp
import java.util.*;
    class  TEMP_ABOVE_AVERAGE{
        public static void main(String[] args) {
            Scanner console = new Scanner(System.in);
            System.out.print("How many days the temperature is to be find: ");
            int numdays = console.nextInt();
            int[] temp =new int[numdays];
            int sum =0;
            for(int i = 0 ; i<numdays; i++){
                System.out.println("day's" +(i+1)+"temperature:");
                temp[i]=console.nextInt();
                sum+=temp[i];
            }
            double average = sum/numdays;

            int above =0;
            for(int i = 0;i<temp.length; i++){
                if(temp[i]>average){
                    above++;
                }

            }
            System.out.println("the average temperature is "+ average);
            System.out.println("the temperature above average temperature is "+ above);
        }
    }
