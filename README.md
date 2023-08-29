import java.util.Scanner; 
import java.lang.Math;
public class Circle {

protected double redius;
   public Circle(double x){
     redius= x;
   }  
    public double circleArea(){
        return Math.PI*redius*redius;
    } 
    } 
    class Cylinder extends Circle{
    
    protected double height;
    public Cylinder(double h,double x){
        super (x);
        height = h;
    }
    public double CylinderSurface (){ 
        return   2*Math.PI*redius*redius +  2*Math.PI*redius*height;
     
     }
}
class main{
   
    public static void main(String[] args){ 
        Scanner sc=new Scanner(System.in);
        System.out.println ("Enter the radius of Circle and Cylinder");
        int x = sc.nextInt();
        int y = sc.nextInt();

        System.out.println("Enter the height:"+x);
        Circle m = new Circle(x);
       
        Cylinder c=new Cylinder(x,y);
       
        System.out.println("Area of circler is="+m.circleArea());
        System.out.println("Area of Cylinder is="+c.CylinderSurface());
   
    }
   
}





    

