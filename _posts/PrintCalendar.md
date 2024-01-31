public class PrintCalendar {
    public static void main(String[] args){
        int day = 1;
        
        System.out.println("S  M  T  W  R  F  S");
        
        while(day <= 30){
           
            if(day < 10){
            System.out.print(day + "  "); // If the day is one digit, add an extra space for alignment
            } else {
                System.out.print(day + " ");
            }
            
            if(day % 7 == 0){
                System.out.println(); // Every 7 days, add a new line for the next week
            }
            
            day++;
        }
    }
}